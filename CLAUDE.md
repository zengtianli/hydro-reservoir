# hydro-reservoir — 梯级水库水电调度优化器

## Quick Reference

| 项目 | 路径/值 |
|------|---------|
| 入口 | `app.py` (Streamlit) |
| 核心逻辑 | `src/reservoir/` |
| 公共工具 | `src/common/` |
| 样例数据 | `data/sample/` |
| 线上 URL | https://hydro-reservoir.tianlizeng.cloud |
| Streamlit 配置 | `.streamlit/config.toml` |

## 常用命令

```bash
cd /Users/tianli/Dev/hydro-reservoir

# 本地启动
streamlit run app.py

# 安装依赖
pip install -r requirements.txt

# 查看 Streamlit 配置
cat .streamlit/config.toml
```

## 项目结构

```
app.py               # Streamlit 主入口
src/
  reservoir/         # 梯级调度核心算法
  common/            # 公共工具函数
data/sample/         # 样例 Excel 输入文件
docs/screenshots/    # 演示截图
```

## 功能说明

- **输入**：上传 Excel 工作簿（水库参数 + 入库流量）
- **调度**：支持日/旬/月三种时间步长的梯级联合优化
- **输出**：Plotly 交互图表（水位、流量、出力）+ 结果 Excel 下载
- **调试**：Parameter Preview 功能可在运行前检查水库参数

## 部署

项目部署在 VPS `/var/www/hydro-reservoir`，通过 Nginx + Cloudflare 提供服务。
更新线上版本：`ssh root@104.218.100.67`，进入项目目录 `git pull` 后重启 Streamlit 进程。
无需外部 API，不依赖 `~/.personal_env`。

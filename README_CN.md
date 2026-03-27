# ⚡ 水库群调度

[![GitHub stars](https://img.shields.io/github/stars/zengtianli/hydro-reservoir)](https://github.com/zengtianli/hydro-reservoir)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Python 3.9+](https://img.shields.io/badge/Python-3.9+-blue.svg)](https://python.org)
[![Streamlit](https://img.shields.io/badge/Streamlit-1.36+-FF4B4B.svg)](https://streamlit.io)

梯级水库水电调度优化工具，支持交互式 Plotly 图表。

![screenshot](docs/screenshot.png)

## 功能特点

- **梯级联合调度** — 多水库串联联合优化
- **灵活时间步长** — 支持逐日、旬、月计算
- **交互式图表** — Plotly 水位、流量、出力过程可视化
- **参数预览** — 计算前查看水库参数、来水系列和调度线
- **Excel 输入输出** — 上传输入工作簿，下载调度结果

## 快速开始

```bash
git clone https://github.com/zengtianli/hydro-reservoir.git
cd hydro-reservoir
pip install -r requirements.txt
streamlit run app.py
```

## 部署（VPS）

```bash
git clone https://github.com/zengtianli/hydro-reservoir.git
cd hydro-reservoir
pip install -r requirements.txt
nohup streamlit run app.py --server.port 8502 --server.headless true &
```

## Hydro Toolkit 插件

本项目是 [Hydro Toolkit](https://github.com/zengtianli/hydro-toolkit) 的插件，也可独立运行。在 Toolkit 的插件管理页面粘贴本仓库 URL 即可安装。

## 许可证

MIT

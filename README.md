# ⚡ Hydro Reservoir — Reservoir Scheduling

[![GitHub stars](https://img.shields.io/github/stars/zengtianli/hydro-reservoir)](https://github.com/zengtianli/hydro-reservoir)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Python 3.9+](https://img.shields.io/badge/Python-3.9+-blue.svg)](https://python.org)
[![Streamlit](https://img.shields.io/badge/Streamlit-1.36+-FF4B4B.svg)](https://streamlit.io)
[![Live Demo](https://img.shields.io/badge/Live%20Demo-hydro--reservoir.tianlizeng.cloud-brightgreen)](https://hydro-reservoir.tianlizeng.cloud)

Cascade reservoir hydropower scheduling optimizer with interactive Plotly charts.

![screenshot](docs/screenshot.png)

## Features

- **Cascade scheduling** — joint optimization of multiple reservoirs in series
- **Flexible time step** — daily, 10-day, or monthly calculation intervals
- **Interactive charts** — Plotly-based visualization of water levels, flow, and power output
- **Parameter preview** — inspect reservoir parameters, inflow series, and dispatch curves before computing
- **Excel I/O** — upload input workbook, download detailed scheduling results

## Quick Start

```bash
git clone https://github.com/zengtianli/hydro-reservoir.git
cd hydro-reservoir
pip install -r requirements.txt
streamlit run app.py
```

## Deploy (VPS)

```bash
git clone https://github.com/zengtianli/hydro-reservoir.git
cd hydro-reservoir
pip install -r requirements.txt
nohup streamlit run app.py --server.port 8502 --server.headless true &
```

## Hydro Toolkit Plugin

This project is a plugin for [Hydro Toolkit](https://github.com/zengtianli/hydro-toolkit) and can also run standalone. Install it in the Toolkit by pasting this repo URL in the Plugin Manager. You can also **[try it online](https://hydro-reservoir.tianlizeng.cloud)** — no install needed.

## License

MIT

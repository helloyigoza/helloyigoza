### Hi, I'm Yigoza 👋

**Full-stack quant developer** — Rust / Python / TypeScript. I build trading & market-microstructure systems end to end: data ingestion, footprint/order-flow analytics, backtesting engines, and the web UIs that make the output usable.

#### 🏗️ Escape Agent — core contributor

[Escape Agent](https://github.com/escape-system/escape-agent) is an autonomous AI coding agent & server written in Rust, with a SolidJS web client. I'm an active member (admin) of the [escape-system](https://github.com/escape-system) organization and one of its contributors.

[![release](https://img.shields.io/github/v/release/escape-system/escape-agent?label=release)](https://github.com/escape-system/escape-agent/releases/latest)
![platforms](https://img.shields.io/badge/platforms-linux%20%7C%20windows-lightgrey)
[![license](https://img.shields.io/badge/license-MIT-green)](https://github.com/escape-system/escape-agent/blob/main/LICENSE)

```sh
# Linux x86_64 — latest release
curl -LO https://github.com/escape-system/escape-agent/releases/latest/download/opencode-0.3.1-linux-x86_64.tar.gz
curl -LO https://github.com/escape-system/escape-agent/releases/latest/download/SHA256SUM
sha256sum -c SHA256SUM --ignore-missing
tar xzf opencode-0.3.1-linux-x86_64.tar.gz
./opencode-0.3.1-linux-x86_64/opencode --version
```

Windows x86_64 builds are published alongside; both ship `web/dist` inside the archive, next to the binary.

[All releases](https://github.com/escape-system/escape-agent/releases) · [Source](https://github.com/escape-system/escape-agent)

#### What I work on

- **Trading systems:** CQG / Binance / Hyperliquid feeds, footprint & absorption analytics, indicators, backtest runners.
- **Backend:** Rust (Tokio, Axum), SQLite/FTS storage, crash-resilient services.
- **Frontend:** SolidJS / React dashboards, real-time SSE charting.
- **Quant tooling:** Python research, feature pipelines, ML-based signal experiments.

> Proprietary trading code and credential-bearing repos stay private — the public work here is the open-source parts of that stack.

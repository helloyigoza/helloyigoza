### Hi, I'm Yigoza 👋

**I built [Escape Agent](https://github.com/escape-system/escape-agent)** — an autonomous AI coding agent and server written in Rust, with a SolidJS web client. I own and maintain it under the [escape-system](https://github.com/escape-system) organization.

**Full-stack quant developer** — Rust / Python / TypeScript. Trading systems, market microstructure, footprint/order-flow analytics, backtesting engines, and the web UIs that make the output usable.

#### Escape Agent — my project

- [escape-system/escape-agent](https://github.com/escape-system/escape-agent) — canonical repo (org I own/admin)
- [helloyigoza/escape-agent](https://github.com/helloyigoza/escape-agent) — my fork / working copy, visible in my repositories

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

- **Escape Agent:** Tokio/Axum runtime, subagents & lanes, tool sandbox, SQLite+FTS memory, observer loop, MCP/LSP, plugin host, SolidJS UI.
- **Trading systems:** CQG / Binance / Hyperliquid feeds, footprint & absorption analytics, indicators, backtest runners.
- **Backend:** Rust, crash-resilient services, real-time SSE APIs.
- **Frontend:** SolidJS / React dashboards, streaming chart UIs.
- **Quant tooling:** Python research, feature pipelines, ML signal experiments.

> Proprietary trading code and credential-bearing repos stay private — the public work here is the open-source parts of that stack.

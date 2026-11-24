<div align="center">

# Yigoza

**Full-stack quant developer — I build trading systems end to end, in Rust, Python and TypeScript.**

[![Escape Agent](https://img.shields.io/github/v/release/escape-system/escape-agent?label=escape%20agent&color=0b7285)](https://github.com/escape-system/escape-agent)
[![Rust](https://img.shields.io/badge/-Rust-000?logo=rust&logoColor=fff)](#stack)
[![Python](https://img.shields.io/badge/-Python-3776AB?logo=python&logoColor=fff)](#stack)
[![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?logo=typescript&logoColor=fff)](#stack)

Creator & maintainer of **[Escape Agent](https://github.com/escape-system/escape-agent)** · based in Türkiye
</div>

---

## What I do

I work on the full path from market data to a decision on screen:

```
exchange / broker feeds  →  normalisation  →  storage  →  analytics  →  API  →  UI
```

That means I own the unglamorous parts too: backpressure on live tick streams, gap detection
and backfill, idempotent aggregation, crash-safe persistence, and reconciling a feed that
silently stops sending.

## Stack

| Layer | What I actually use |
|---|---|
| **Systems / services** | Rust — Tokio, Axum, `serde`, `tower`; async pipelines, graceful shutdown, bounded channels |
| **Storage & data** | SQLite + FTS, Arrow/Parquet columnar segments, append-only WAL-style stores, gap/backfill tooling |
| **Market connectivity** | CQG (futures), Binance, Hyperliquid, CCXT; REST + WebSocket, order-book and tick normalisation |
| **Quant research** | Python — NumPy/Polars, PyTorch, LoRA fine-tuning of time-series transformers, quantile forecast heads |
| **Frontend** | TypeScript, SolidJS/React, real-time SSE streaming, canvas charting |
| **Engineering hygiene** | `clippy -D warnings`, `cargo fmt --check`, `deny.toml`, strict lints; test-heavy codebase |

## Projects

### 🏗️ Escape Agent — autonomous AI coding agent & server
Rust runtime + SolidJS client, wire-compatible with OpenCode protocols.

Multi-agent orchestration with hierarchy and execution lanes, sandboxed tool execution
(read/write/edit/patch/glob/grep/shell), SQLite+FTS5 persistent memory, goal/observer loop
that detects stalls and self-repairs, MCP (stdio/HTTP/OAuth), LSP, plugin host, SSE streaming.

→ [escape-system/escape-agent](https://github.com/escape-system/escape-agent) · [my fork](https://github.com/helloyigoza/escape-agent)

### 📈 Trading & market-microstructure systems *(private)*
An 11-crate Rust workspace (~520k lines of Rust, ~7.3k test functions) powering a live trading
stack: footprint/order-flow engine, indicators, backtesting, CQG + Binance + Hyperliquid
ingestion, vectorised analytics, a Telegram ops bot, and a 55-route Axum web layer with a
real-time charting UI. Versioned storage with manifest/segment layout instead of a monolithic database.

Private by design — it carries live credentials and proprietary analytics.

### 🔬 Quant research *(public)*
| Repo | What it is |
|---|---|
| [deeptrade-trainer](https://github.com/helloyigoza/deeptrade-trainer) | Cross-asset quantile forecasting (P10/P50/P90) — TTM-R3 backbone + LoRA, PyTorch |
| [adaptive_band_ai](https://github.com/helloyigoza/adaptive_band_ai) | GRU predicting asymmetric price bands from OHLCV |
| [ichimoku-python](https://github.com/helloyigoza/ichimoku-python) | Pandas-free Ichimoku engine on Polars |
| [harmonicpat-detector](https://github.com/helloyigoza/harmonicpat-detector) | Harmonic pattern detection over OHLC |
| [ccxt-multi-exchange-copy-trader](https://github.com/helloyigoza/ccxt-multi-exchange-copy-trader) | Leader/follower copy-trading across exchanges |
| [game-theory-llm](https://github.com/helloyigoza/game-theory-llm) | LLM agents playing Prisoner's Dilemma, Public Goods, Ultimatum |

### 🛡️ Network systems
[mtasa-firewall-rust](https://github.com/helloyigoza/mtasa-firewall-rust) — packet-level firewall
in Rust (`nfq`/`nftables`), and its [Python predecessor](https://github.com/helloyigoza/mtasa-firewall-python)
with TCP SYN-cookie anti-spoofing.

## How I work

- **Measure before claiming.** Benchmarks and tests, not vibes. If a number isn't verified, it doesn't go in the README.
- **Boring reliability beats clever.** Bounded queues, explicit timeouts, honest error states.
- **No fake features.** A UI control that doesn't change behaviour is a bug, not a placeholder.

<sub>Proprietary code and credential-bearing repos stay private.</sub>

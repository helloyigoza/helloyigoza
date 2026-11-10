### Hi, I'm Yigoza 👋

I build autonomous coding agents — and the guardrails that make them trustworthy.

#### [Escape Agent](https://github.com/escape-system/escape-agent)

An autonomous AI coding agent and server, written in Rust.

[![release](https://img.shields.io/github/v/release/escape-system/escape-agent?label=release)](https://github.com/escape-system/escape-agent/releases/latest)
![platforms](https://img.shields.io/badge/platforms-linux%20%7C%20windows-lightgrey)
[![license](https://img.shields.io/badge/license-MIT-green)](https://github.com/escape-system/escape-agent/blob/main/LICENSE)

```sh
# Linux x86_64
curl -LO https://github.com/escape-system/escape-agent/releases/latest/download/opencode-0.3.1-linux-x86_64.tar.gz
curl -LO https://github.com/escape-system/escape-agent/releases/latest/download/SHA256SUMS
sha256sum -c SHA256SUMS --ignore-missing
tar xzf opencode-0.3.1-linux-x86_64.tar.gz
./opencode-0.3.1-linux-x86_64/opencode --version   # opencode 0.3.1
```

Windows x86_64 builds are published alongside; both ship `web/dist` inside the archive, next to the binary.

[All releases](https://github.com/escape-system/escape-agent/releases) · [Source](https://github.com/escape-system/escape-agent)

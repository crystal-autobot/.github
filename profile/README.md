<p align="center">
  <img src="https://raw.githubusercontent.com/crystal-autobot/autobot/main/docs/assets/banner-circuit-hex.svg" alt="crystal-autobot" width="100%">
</p>

<p align="center"><b>Ultra-efficient personal AI assistant powered by Crystal</b></p>

<p align="center">
  <a href="https://github.com/crystal-autobot/autobot">
    <img src="https://img.shields.io/github/v/release/crystal-autobot/autobot?style=flat-square&color=blue" alt="Release">
  </a>
  <a href="https://github.com/crystal-autobot/autobot/actions">
    <img src="https://img.shields.io/github/actions/workflow/status/crystal-autobot/autobot/ci.yml?style=flat-square" alt="CI">
  </a>
  <a href="https://github.com/crystal-autobot/autobot/blob/main/LICENSE">
    <img src="https://img.shields.io/github/license/crystal-autobot/autobot?style=flat-square" alt="License">
  </a>
</p>

---

**Autobot** is a personal AI assistant framework written in [Crystal](https://crystal-lang.org) — inspired by [OpenClaw](https://openclaw.ai/), rebuilt from scratch with security and efficiency as first-class concerns.

### At a glance

- **2MB** binary, **~5MB** RAM, **<20ms** startup, **zero** runtime dependencies
- Multi-provider LLM — Anthropic, OpenAI, DeepSeek, Groq, Gemini, OpenRouter, AWS Bedrock, DuckAI, vLLM
- Chat channels — Telegram, Slack, WhatsApp, Zulip with allowlists and custom commands
- Kernel-enforced sandboxing — Docker/bubblewrap OS-level isolation with custom `Dockerfile.sandbox`
- Vision and voice — image analysis and Whisper transcription
- Builtin plugins — SQLite, GitHub, Weather; opt-out via config
- Persistent memory, cron scheduling, MCP servers, markdown skills
- Run dozens of isolated bots on a single machine

### Get started

```bash
brew tap crystal-autobot/tap && brew install autobot
autobot new optimus && cd optimus
autobot doctor
autobot gateway
```

### Repositories

| Repository | Description |
|---|---|
| [ark](https://github.com/crystal-autobot/ark) | Slack gateway for AWS Bedrock Agents via Socket Mode |
| [autobot](https://github.com/crystal-autobot/autobot) | Core framework — agent runtime, providers, channels, plugins, tools |
| [autobot-wasm](https://github.com/crystal-autobot/autobot-wasm) | WebAssembly plugin — write tools in any language, compile to `.wasm` |
| [blueprints](https://github.com/crystal-autobot/blueprints) | Ready-to-use templates — Optimus, Bumblebee, Blaster, Red Alert |
| [homebrew-tap](https://github.com/crystal-autobot/homebrew-tap) | Homebrew formula for macOS/Linux installation |

### Links

- [Documentation](https://crystal-autobot.github.io/autobot/)
- [Quick start guide](https://crystal-autobot.github.io/autobot/quickstart/)
- [Security architecture](https://crystal-autobot.github.io/autobot/security/)
- [Contributing](https://github.com/crystal-autobot/.github/blob/main/CONTRIBUTING.md)
- [Code of conduct](https://github.com/crystal-autobot/.github/blob/main/CODE_OF_CONDUCT.md)

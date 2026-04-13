# InnerZero: Free Private AI Assistant That Runs on Your PC

InnerZero is a free, local-first AI assistant that runs entirely on your machine. No cloud. No account. No data collection. Your conversations, your memory, your data, all staying on your hardware.

Built for anyone who wants a powerful AI assistant without giving up their privacy.

## Download

**Latest release: v0.1.2**

| Platform | Download | Size | Requirements |
|----------|----------|------|-------------|
| **Windows** | [InnerZero-Setup-v0.1.2.exe](https://github.com/zotex12/innerzero-releases/releases/latest) | ~239 MB | Windows 10/11 64-bit |
| **macOS** | [InnerZero-Setup-v0.1.2-mac.dmg](https://github.com/zotex12/innerzero-releases/releases/latest) | ~490 MB | macOS 12+ (Monterey or later) |
| **Linux** | [InnerZero-v0.1.2-x86_64.AppImage](https://github.com/zotex12/innerzero-releases/releases/latest) | ~356 MB | 64-bit, glibc 2.35+, libfuse2 |

**Recommended hardware:** 16GB+ RAM. GPU optional but recommended (NVIDIA 6GB+ VRAM, AMD, or Apple Silicon for faster responses).

InnerZero handles all setup automatically. It downloads and configures the right AI model for your hardware on first launch.

## What Is InnerZero?

InnerZero is a desktop AI assistant that processes everything locally using open-source AI models through [Ollama](https://ollama.com) or [LM Studio](https://lmstudio.ai). Unlike ChatGPT, Gemini, or other cloud AI services, InnerZero never sends your data to external servers.

It is completely free. Not a trial, not a freemium tier, not a limited version. The full application with all features runs on your hardware at no cost, forever.

## Key Features

**Private by design.** All AI processing runs on your hardware. No cloud servers, no API calls (unless you choose to enable optional cloud mode with your own API keys), no telemetry, no tracking. Your conversations are stored in a local database that never leaves your machine.

**Personal memory system.** InnerZero remembers your conversations, preferences, projects, and facts across sessions. It builds structured memory over time, so it knows your name, your work context, and your preferences without you repeating yourself. An offline sleep and reflection pipeline consolidates and refines memories automatically.

**Voice and text.** Full voice mode with local speech recognition (Whisper) and local text-to-speech (Kokoro). Talk to your AI assistant hands-free. All voice processing runs locally.

**30+ built-in tools.** Web search, file read/write, URL fetching, calculator, system info, clipboard, timers, reminders, notes, weather, dictionary, screen reading, and more.

**AI Specialists.** A modular agent system where specialist AI workers (starting with a coding agent) handle domain-specific tasks. The Director AI delegates work, specialists execute with sandboxed file access, and you approve changes through a two-gate review system.

**Hardware-aware setup.** InnerZero detects your CPU, GPU, and RAM on first launch and selects the best AI model for your system. Works on everything from laptops with no GPU to high-end workstations.

**Multiple AI backends.** Ollama (default, managed automatically) or LM Studio (connect to models you already have loaded). Optional cloud mode supports OpenAI, Anthropic, Google, DeepSeek, and Qwen with your own API keys, zero markup.

**Offline knowledge packs.** Download Wikipedia and reference databases for fully offline information retrieval. No internet required after setup.

## How It Works

1. **Download and install.** One installer, no dependencies to manage. InnerZero bundles everything it needs.
2. **Automatic configuration.** InnerZero detects your hardware and downloads the right AI model. Takes a few minutes on first launch.
3. **Start chatting.** Text or voice. Your private AI assistant is ready. Memory builds automatically over time.

## How InnerZero Compares

| | InnerZero | ChatGPT | GPT4All | LM Studio | Jan |
|---|---|---|---|---|---|
| Runs 100% locally | Yes | No | Yes | Yes | Yes |
| Personal memory across sessions | Yes (8-layer system) | Limited | No | No | No |
| Voice mode (local) | Yes | No (cloud) | No | No | No |
| Built-in tools (30+) | Yes | Yes (cloud) | No | No | Limited |
| AI agent system | Yes | Yes (cloud) | No | No | No |
| Sleep/reflection pipeline | Yes | No | No | No | No |
| Free forever | Yes | Freemium | Yes | Yes | Yes |
| No account required | Yes | No | Yes | Yes | Yes |

## Optional Cloud Mode

InnerZero works fully offline. If you want faster responses or access to premium models (Claude, GPT, Gemini, DeepSeek), you can:

- **Add your own API keys** from any supported provider. Free, zero markup. InnerZero never stores your keys on any server.
- **Subscribe to a managed cloud plan** starting at £9.99/month for hassle-free access to multiple providers.

Cloud mode is off by default. When enabled, your prompts are sent to the AI provider and returned. InnerZero never reads, logs, or stores your cloud conversations.

## System Requirements

**Minimum:** 8GB RAM, any 64-bit CPU (Intel or AMD on Windows/Linux, Apple Silicon or Intel on macOS). InnerZero will run but responses will be slower without a GPU.

**Recommended:** 16GB+ RAM, dedicated GPU with 6GB+ VRAM (NVIDIA, AMD, or Apple Silicon unified memory). This gives fast, responsive AI interactions.

**Storage:** ~500 MB for the application, plus 2-8 GB for AI models (downloaded automatically on first launch).

## Links

- [Website](https://innerzero.com)
- [Features](https://innerzero.com/features)
- [Pricing](https://innerzero.com/pricing)
- [Privacy Policy](https://innerzero.com/privacy)
- [Learn (Blog)](https://innerzero.com/blog)
- [Changelog](https://innerzero.com/changelog)
- [Discord Community](https://discord.gg/5XjCe2RNAJ)
- [Support Development on Ko-fi](https://ko-fi.com/innerzero)

## Licence

InnerZero is proprietary software by [Summers Solutions Ltd](https://summerssolutions.co.uk) (Company No. 16448945, Birmingham, UK). See [LICENSE](LICENSE) and [Terms of Service](https://innerzero.com/terms).

InnerZero uses open-source AI models and incorporates open-source components which retain their original licences. Full attribution is available within the application.

© 2025-2026 Summers Solutions Ltd. All rights reserved.

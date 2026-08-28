# InnerZero: Free Private AI Assistant That Runs on Your PC

InnerZero is a free, local-first AI assistant that runs entirely on your machine. No cloud. No account. No data collection. Your conversations, your memory, your data, all staying on your hardware.

Built for anyone who wants a powerful AI assistant without giving up their privacy.

## Download

**[Latest release](https://github.com/zotex12/innerzero-releases/releases/latest)** or go to [innerzero.com/download](https://innerzero.com/download) for guided platform detection.

Available for **Windows 10/11**, **macOS 14+**, and **Linux** (64-bit, glibc 2.31+, libfuse2).

**Latest release: v0.2.1**

| Platform | Download | Size | Requirements |
|----------|----------|------|-------------|
| **Windows** | [InnerZero-Setup-0.2.1.exe](https://github.com/zotex12/innerzero-releases/releases/download/v0.2.1/InnerZero-Setup-0.2.1.exe) | ~1.24 GB | Windows 10/11 64-bit |
| **macOS** | [InnerZero-Setup-0.2.1-mac.dmg](https://github.com/zotex12/innerzero-releases/releases/download/v0.2.1/InnerZero-Setup-0.2.1-mac.dmg) | ~775 MB | macOS 14+ (Sonoma or later, Apple Silicon) |
| **Linux** | [InnerZero-0.2.1-x86_64.AppImage](https://github.com/zotex12/innerzero-releases/releases/download/v0.2.1/InnerZero-0.2.1-x86_64.AppImage) | ~1.18 GB | 64-bit, glibc 2.31+, libfuse2 |

**macOS install note:** the DMG is signed with Developer ID, notarised by Apple, and stapled. It opens with a normal double click, with no Gatekeeper warning and no workaround needed.

Each release includes SHA256 checksums (`windows.sha256`, `macos.sha256`, `linux.sha256`) on the [release page](https://github.com/zotex12/innerzero-releases/releases/latest).

**Recommended hardware:** 16GB+ RAM. GPU optional but recommended (NVIDIA 6GB+ VRAM, AMD, or Apple Silicon for faster responses).

InnerZero handles all setup automatically. It downloads and configures the right AI model for your hardware on first launch.

## What's New in v0.2.1

A runtime update, better feedback, and a way in for machines that cannot run a local model.

- **Bundled Ollama updated from 0.22 to 0.32.** Vulkan GPU acceleration is on by default, so AMD and Intel GPUs work out of the box and the old experimental Vulkan toggle is gone. NVIDIA GPUs need driver 550 or newer for GPU acceleration, or 570 or newer for older Maxwell and Pascal cards (which may also run a little slower than before); older drivers fall back to the CPU. On Windows, AMD cards on the ROCm path need ROCm 7 drivers, and RDNA2 cards are now served by Vulkan instead. Machines with only an integrated GPU may need `OLLAMA_IGPU_ENABLE=1` in the environment, because Ollama 0.32 hides integrated GPUs by default.
- **Attach your app log to feedback.** The sidebar feedback box can include the last 15 minutes, hour, or day of InnerZero's own activity log, reduced to event names, labels, and sizes only (prompts, replies, file paths, and your username never leave the machine), with a preview before anything is sent. Settings > General gained an Open Logs Folder row.
- **Ask Zero about InnerZero itself.** Questions like "how do I change the theme" or "what can you do" are answered from a built-in guide to the app.
- **Network Ollama for low-spec machines.** If your PC cannot run a local model, point Settings > AI & Models at another computer on your network running Ollama and chat works from there. The chat banner, blocked messages, and the setup wizard offer three ways forward on that tier: a cloud plan or API key, choosing a tier yourself, or a network Ollama server.
- **Smaller improvements.** Office documents (.pptx, .docx, .xlsx and more) are recognised as files in chat; Settings > Hardware names every detected GPU; 32 GB machines that report 30 to 31 GB usable land on the right tier; the first-run GPU check survives a cold first load; voice follows your chosen cloud source; unvetted models are flagged in the voice and setup pickers.
- **Fixes.** A No Local Model machine no longer answers "hi" and then blocks every real question; updating on Windows removes the previous version's runtime libraries; deleting a Google-pushed calendar event keeps its link until you confirm; Unrestricted Mode's manual install instructions no longer vanish when you leave the Experimental tab.

See the full [changelog](https://innerzero.com/changelog).

## What Is InnerZero?

InnerZero is a desktop AI assistant that processes everything locally using open-source AI models through [Ollama](https://ollama.com), [LM Studio](https://lmstudio.ai), or your own [llama.cpp](https://github.com/ggml-org/llama.cpp) server. Unlike ChatGPT, Gemini, or other cloud AI services, InnerZero never sends your data to external servers.

It is completely free. Not a trial, not a freemium tier, not a limited version. The full application with all features runs on your hardware at no cost.

## Key Features

**Private by design.** All AI processing runs on your hardware. No cloud servers, no API calls (unless you choose to enable optional cloud mode with your own API keys), no telemetry, no tracking. Your conversations are stored in a local database that never leaves your machine.

**Speaks your language.** The entire interface is available in 26 languages, and Zero replies in the one you pick. Switch any time in Settings, with right-to-left support for Arabic, Hebrew, Persian, and Urdu. A one-time upgrade keeps your saved memories searchable across every language. Works fully offline.

**Personal memory system.** InnerZero remembers your conversations, preferences, projects, and facts across sessions. It builds structured memory over time, so it knows your name, your work context, and your preferences without you repeating yourself. Memory improves over time as InnerZero learns what matters to you, all without sending anything to the cloud.

**Voice and text.** Full voice mode with local speech recognition (Whisper) and local text-to-speech (Kokoro). Talk to your AI assistant hands-free, all processed locally. The Voice page also has standalone speech-to-text and text-to-speech panels, and you can dictate straight into the chat box.

**Prompt Library.** Save your best prompts in folders, mark favourites, and drop them into chat in one click.

**Files, images, and artifacts.** Attach documents or paste a screenshot in chat, with local text recognition on images. Document-style answers open in an artifacts panel you can read full screen, edit with the AI, and export to PDF, Word, Markdown, and more with real selectable text.

**30+ built-in tools.** Web search, file read/write, URL fetching, calculator, system info, clipboard, timers, reminders, notes, weather, dictionary, screen reading, and more.

**Slash commands.** Type `/help`, `/clear`, `/memory`, `/event`, and more for quick actions in chat.

**Proactive Assistant.** Schedule briefings and reminders so InnerZero brings information to you, not just on demand. Natural-language scheduling ("every weekday at 9am"), quiet hours, and an optional Telegram bridge for briefings on your phone.

**Action Hub.** An opt-in research and apply assistant. With your own Apify key, Zero gathers and summarises web sources; with your saved job profile, it can help fill in and submit job applications in a fresh, isolated browser, asking for your approval before it acts.

**AI Specialists.** Domain-specific helpers handle focused tasks like coding and automation. You stay in control with explicit approval before any file changes are written.

**Hardware-aware setup.** InnerZero detects your CPU, GPU, and RAM on first launch and selects the best AI model for your system. Works on everything from laptops with no GPU to high-end workstations.

**Multiple AI backends.** Ollama (default, managed automatically, or an Ollama server on your own network), LM Studio (connect to models you already have loaded), or your own llama.cpp llama-server with a GGUF model picker. Optional cloud mode supports 7 providers (OpenAI, Anthropic, Google, DeepSeek, Qwen, xAI Grok, Kimi) with your own API keys, zero markup.

**Privacy controls.** Offline mode blocks all outbound network requests. A single fail-closed egress guard checks every outbound connection, so Offline and Private modes hold even if a tool tries to reach out. Connection log shows every outbound request. Privacy blacklist scrubs sensitive terms from cloud messages before they leave your machine. My Privacy dashboard gives you centralised control over all privacy settings. A proxy box lets you reach the internet from behind a corporate or university proxy, while local AI traffic is never proxied.

**Telegram remote access.** Control Zero from your phone via a Telegram bot with encrypted token storage, chat ID whitelisting, and desktop chat mirroring. Separate from the Proactive Assistant Telegram bridge above; reuses the same bot setup.

**Offline knowledge packs.** Download Wikipedia and reference databases for fully offline information retrieval. No internet required after setup.

## How It Works

1. **Download and install.** One installer, no dependencies to manage. InnerZero bundles everything it needs.
2. **Automatic configuration.** InnerZero detects your hardware and downloads the right AI model. Takes a few minutes on first launch.
3. **Start chatting.** Text or voice. Your private AI assistant is ready. Memory builds automatically over time.

## How InnerZero Compares

| | InnerZero | ChatGPT | GPT4All | LM Studio | Jan |
|---|---|---|---|---|---|
| Runs 100% locally | Yes | No | Yes | Yes | Yes |
| Personal memory across sessions | Yes | Limited | No | No | No |
| Voice mode (local) | Yes | No (cloud) | No | No | No |
| Built-in tools (30+) | Yes | Yes (cloud) | No | No | Limited |
| AI agent system | Yes | Yes (cloud) | No | No | No |
| Memory that improves over time | Yes | No | No | No | No |
| Free | Yes | Freemium | Yes | Yes | Yes |
| No account required | Yes | No | Yes | Yes | Yes |

## Optional Cloud Mode

InnerZero works fully offline. If you want faster responses or access to premium models (Claude, GPT, Gemini, DeepSeek), you can:

- **Add your own API keys** from any supported provider. Free, zero markup. InnerZero never stores your keys on any server.
- **Subscribe to a managed cloud plan** starting at £9.99/month for hassle-free access to multiple providers.

Cloud mode is off by default. When enabled, your prompts are sent to the AI provider and returned. InnerZero never reads, logs, or stores your cloud conversations.

## System Requirements

**Minimum:** 8GB RAM, any 64-bit CPU (Intel or AMD on Windows/Linux, Apple Silicon on macOS). InnerZero will run but responses will be slower without a GPU.

**Recommended:** 16GB+ RAM, dedicated GPU with 6GB+ VRAM (NVIDIA, AMD, or Apple Silicon unified memory). This gives fast, responsive AI interactions.

**Storage:** ~500 MB for the application, plus 2-8 GB for AI models (downloaded automatically on first launch).

## Links

- [Website](https://innerzero.com)
- [Features](https://innerzero.com/features)
- [Pricing](https://innerzero.com/pricing)
- [Privacy Policy](https://innerzero.com/privacy)
- [Learn (Blog)](https://innerzero.com/blog)
- [Changelog](https://innerzero.com/changelog)
- [Discord Community](discord.gg/rn9SPXgThT)
- [Support Development on Ko-fi](https://ko-fi.com/innerzero)

## Licence

InnerZero is proprietary software by [Summers Solutions Ltd](https://summerssolutions.co.uk) (Company No. 16448945, Birmingham, UK). See [LICENSE](LICENSE) and [Terms of Service](https://innerzero.com/terms).

InnerZero uses open-source AI models and incorporates open-source components which retain their original licences. Full attribution is available within the application.

© 2025-2026 Summers Solutions Ltd. All rights reserved.

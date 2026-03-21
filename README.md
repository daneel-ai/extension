<p align="center">
  <img src="assets/icon-128.png" alt="Daneel AI" width="80" />
</p>

<h1 align="center">Daneel AI</h1>

<p align="center">
  <strong>Chat with any website or your own documents — 100% in your browser.</strong><br/>
  No API keys. No servers. No data leaves your machine.
</p>

<p align="center">
  <a href="#install">Install</a> ·
  <a href="#features">Features</a> ·
  <a href="#inference-backends">Backends</a> ·
  <a href="#faq">FAQ</a> ·
  <a href="https://github.com/daneel-ai/extension/issues/new/choose">Report Bug</a> ·
  <a href="https://github.com/daneel-ai/extension/issues/new/choose">Request Feature</a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Manifest-V3-blue" alt="Manifest V3" />
  <img src="https://img.shields.io/badge/License-Proprietary-lightgrey" alt="License" />
</p>

---

## What is Daneel AI?

Daneel AI is a Chrome extension that lets you **have conversations with web pages, entire websites, and your own documents** using AI that runs locally in your browser.

Unlike other AI extensions, Daneel requires **no API keys, no cloud accounts, and no external servers** after the initial model download. Your data never leaves your machine.

---

## Install

<!-- TODO: Replace with actual Chrome Web Store link -->
<a href="#">
  <img src="https://img.shields.io/badge/Chrome_Web_Store-Install-4285F4?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Install from Chrome Web Store" />
</a>

**Supported browsers:** Chrome, Edge, Brave, Arc (any Chromium-based browser with WebGPU support).

---

## Features

### Page Mode — Ask questions about the current page

Select any webpage and start chatting. Daneel extracts the page content, converts it to clean Markdown, and uses it as context for your questions.

- Instant page extraction (no crawling needed)
- Smart context selection for long pages
- Conversation history saved per URL
- Quick actions: Explain, Summarize, Key Concepts, Translate

### Site Mode — Index and search entire websites

Crawl an entire site using its sitemap, embed all pages, and ask questions across the full site content.

- Automatic sitemap discovery
- Configurable crawl depth and page limits
- GPU-accelerated cosine similarity search
- Persistent embeddings in IndexedDB (survives browser restarts)

### Document Vault — Chat with your own files

Import PDFs, DOCX, Markdown, and text files into organized vaults. Chat with individual documents or search across an entire vault.

- Three-column workspace: Vaults → Documents → Chat
- Built-in document viewer with side-by-side chat
- Per-document and per-vault conversation history
- Full-text search within vaults
- Import/export for data portability

### Privacy First

- **100% local inference** with WebGPU (default)
- No telemetry without explicit opt-in
- All data stored locally in your browser
- No accounts required

---

## Inference Backends

Daneel supports multiple AI backends — switch at any time in Settings:

| Backend | Privacy | Speed | Quality | Setup |
|---|---|---|---|---|
| **WebGPU** (default) | 100% local | Fast (GPU) | Good | None — auto-downloads model |
| **Chrome Built-in AI** | 100% local | Fast | Good | Enable in chrome://flags |
| **Ollama** | Local network | Fast | Excellent | Install Ollama separately |
| **Claude API** | Cloud | Fast | Best | Requires API key |

---

## Screenshots

<!-- TODO: Add screenshots -->

---

## FAQ

<details>
<summary><strong>How much disk space does the model need?</strong></summary>
The default WebGPU model (LFM2 1.2B, q4) is approximately 600 MB. It's downloaded once and cached by your browser.
</details>

<details>
<summary><strong>Does it work offline?</strong></summary>
Yes! After the initial model download, Page mode and Document Vault work fully offline. Site mode requires internet access to crawl pages.
</details>

<details>
<summary><strong>Which browsers are supported?</strong></summary>
Any Chromium-based browser with WebGPU support: Chrome 113+, Edge 113+, Brave, Arc. Firefox and Safari are not supported.
</details>

<details>
<summary><strong>Is my data sent anywhere?</strong></summary>
With the default WebGPU backend: no. All inference runs locally. With Claude API backend: your prompts are sent to Anthropic's API. Telemetry is opt-in only.
</details>

<details>
<summary><strong>Can I use my own models?</strong></summary>
Yes, via Ollama. Install any model locally and connect Daneel to it in Settings.
</details>

---

## Internationalization

Daneel is available in:
- English
- Français
- Español
- Deutsch
- Italiano

Language is auto-detected from your browser settings and can be changed in the onboarding wizard or settings.

---

## Support & Community

- **Bug reports**: [Open an issue](https://github.com/daneel-ai/extension/issues/new?template=bug_report.yml)
- **Feature requests**: [Open an issue](https://github.com/daneel-ai/extension/issues/new?template=feature_request.yml)
- **Questions & discussion**: [GitHub Discussions](https://github.com/daneel-ai/extension/discussions)
- **Website**: [daneel.injen.io](https://daneel.injen.io)

---

## License

Daneel AI is proprietary software. See the [license terms](https://daneel.injen.io/terms) for details.

A free plan is available with full functionality. Premium features are unlocked with a license key.

---

<p align="center">
  Built with ❤️ by <a href="https://injen.io">injen.io</a>
</p>

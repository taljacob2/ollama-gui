<p align="center">
  <img src=".github/header.png" alt="Ollama GUI logo">
</p>

<h1 align="center">Ollama GUI</h1>
<p align="center">A modern web interface for chatting with your local LLMs through Ollama</p>

<p align="center">
  <a href="https://ollama.ai">
    <img src="https://img.shields.io/badge/Powered%20by-Ollama-blue?style=flat-square" alt="Powered by Ollama">
  </a>
  <a href="https://github.com/HelgeSverre/ollama-gui/blob/main/LICENSE.md">
    <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square" alt="MIT License">
  </a>
  <a href="https://ollama-gui.vercel.app">
    <img src="https://img.shields.io/badge/Demo-Live-success?style=flat-square" alt="Live Demo">
  </a>
</p>

## ✨ Features

- 🖥️ Clean, modern interface for interacting with Ollama models
- 💾 Local chat history using IndexedDB
- 📝 Full Markdown support in messages
- 🌙 Dark mode support
- 🚀 Fast and responsive
- 🔒 Privacy-focused: All processing happens locally

## 🚀 Quick Start

### Prerequisites

1. Install [Ollama](https://ollama.ai/download)
2. Install [Node.js](https://nodejs.org/) (v16+) and [Yarn](https://classic.yarnpkg.com/lang/en/docs/install)

### Local Development

```bash
# Start Ollama server with your preferred model
ollama pull mistral  # or any other model
ollama serve

# Clone and run the GUI
git clone https://github.com/HelgeSverre/ollama-gui.git
cd ollama-gui
yarn install
yarn dev
```

### Using the Hosted Version

To use the [hosted version](https://ollama-gui.vercel.app), run Ollama with:

```bash
OLLAMA_ORIGINS=https://ollama-gui.vercel.app ollama serve
```

### Docker Deployment

```bash
# Pull and run the latest image
docker run -d -p 8080:80 ghcr.io/helgesverre/ollama-gui:main

# Access at http://localhost:8080
```

Or build the image locally, and run it:

```bash
# Build the image
docker build -t ollama-gui .

# Run the container
docker run -d -p 8080:80 ollama-gui

# Access at http://localhost:8080
```

## 🛣️ Roadmap

- [x] Chat history with IndexedDB
- [x] Markdown message formatting
- [x] Code cleanup and organization
- [ ] Model library browser and installer
- [ ] Mobile-responsive design
- [ ] File uploads with OCR support

## 🛠️ Tech Stack

- [Vue.js](https://vuejs.org/) - Frontend framework
- [Vite](https://vitejs.dev/) - Build tool
- [Tailwind CSS](https://tailwindcss.com/) - Styling
- [VueUse](https://vueuse.org/) - Vue Composition Utilities
- [@tabler/icons-vue](https://github.com/tabler/icons-vue) - Icons
- Design inspired by [LangUI](https://www.langui.dev/)
- Hosted on [Vercel](https://vercel.com/)

## 📄 License

Released under the [MIT License](LICENSE.md).

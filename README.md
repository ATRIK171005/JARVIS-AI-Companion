# 🛡️ JARVIS Personal AI Suite (`Obsidian Command Center V1.0`)

> An ultra-lightweight, high-speed, local neural AI voice and conversational operating studio engineered specifically for hardware resource efficiency (`<2 GB VRAM` on NVIDIA RTX 3050 & Intel i5-12500H).

![JARVIS Cyber-Obsidian UI](https://img.shields.io/badge/UI-Cyber--Obsidian%20Glassmorphism-00E5FF?style=for-the-badge)
![Ollama Acceleration](https://img.shields.io/badge/AI%20Engine-Ollama%20Qwen%202.5%203B%20%2F%207B-b76dff?style=for-the-badge)
![FastAPI Backend](https://img.shields.io/badge/Backend-FastAPI%20SSE%20Streaming-10B981?style=for-the-badge)
![Privacy 100% Local](https://img.shields.io/badge/Privacy-100%25%20Local%20Off--Grid-ffb0cd?style=for-the-badge)

---

## 🌟 Key Features

### 🌌 1. Interactive WebGL Background & Cyber-Obsidian UI
- **Live Digital Noise Shader:** A custom-engineered WebGL GLSL fragment shader running in real-time (`#051424` midnight navy base with glowing cyan pulse lines and scanlines) with zero frame drops.
- **Glassmorphism Architecture:** Custom glowing `glass-panel` cards with electric cyan borders (`cyber-border-cyan`) and animated voice waveforms (`waveform-bar`).

### 🧠 2. Neural Large Language Model Support (`GPU Acceleration`)
Seamlessly integrates with **Ollama (`http://localhost:11434`)** via clean FastAPI Server-Sent Events (SSE) streaming:
- **`qwen2.5:3b` (Primary Recommended — `~2.0 GB VRAM`):** Ultra-fast generation (`~50 tokens/sec`), leaving 2 GB VRAM completely free so desktop applications and browser rendering never stutter.
- **`qwen2.5:7b` (Deep Reasoning Hybrid Offloading — `~4.7 GB`):** Automatically distributes weights across GPU VRAM and System RAM.
- **`llama3.2:3b` (Meta Conversational Engine):** Fast instruction-following dialogue.

### ⚡ 3. Zero-Latency Native Python Engine (`Fallback Mode`)
- When Ollama is offline, JARVIS automatically engages a **built-in zero-latency Python heuristic engine (`<35 MB RAM`)** with local `sqlite3` **Knowledge Vault RAG memory retrieval**. Never crashes, always answers.

### 🎙️ 4. Full Hands-Free Voice Ecosystem
- **Speech-to-Text (`STT`):** Real-time microphone transcription via Webkit Speech Recognition.
- **Text-to-Speech (`TTS`):** Spoken neural audio using the local OS `SpeechSynthesisUtterance` (`en-US Neural / Natural voices`) with automatic markdown stripping for clean, natural cadence.
- **Continuous Walkie-Talkie Mode:** Automatically re-triggers microphone recognition immediately after JARVIS finishes speaking for hands-free dialogue.

### 📚 5. Persistent RAG Knowledge Vault & Hardware Dashboard
- **Knowledge Vault:** Store, edit, and delete permanent behavioral directives, personal notes, and coding preferences that JARVIS automatically injects into its system prompt on every turn.
- **Live Hardware Diagnostics:** Real-time KPI monitoring of `CPU Load`, `VRAM Allocation`, `Thermal Level (58°C)`, and `Inference Latency`.

---

## 🛠️ Quickstart & Local Setup

### 1. Requirements
- Python 3.10+
- [Ollama](https://ollama.com/) (optional, but recommended for full neural intelligence)

### 2. Installation & Startup
```powershell
# Clone repository
git clone https://github.com/ATRIK171005/JARVIS-AI-Companion.git
cd JARVIS-AI-Companion

# Install Python dependencies
pip install fastapi uvicorn

# Launch local server
python server.py
```
Open your browser to `http://localhost:8555`.

### 3. Enable Full Hardware-Accelerated Neural Intelligence
In a separate PowerShell or terminal window, download the recommended model:
```powershell
ollama run qwen2.5:3b
```
Once started, select `qwen2.5:3b` from the sidebar dropdown inside JARVIS Studio and enjoy ~50 tokens/sec live reasoning!

---

## 🏗️ Architecture & Tech Stack
- **Frontend:** Single-Page Application (`static/index.html`), Tailwind CSS via CDN, WebGL Shader Engine, Web Speech API, Marked.js.
- **Backend:** Python FastAPI (`server.py`), Uvicorn ASGI Server, SQLite 3 (`stitch_memory.db`), StreamingResponse (`text/event-stream`).

---
*Developed with ❤️ by Atrik Samanta for high-performance laptop optimization.*

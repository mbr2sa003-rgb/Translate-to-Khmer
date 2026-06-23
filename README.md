# 🎬 ប្រព័ន្ធបកប្រែភាពយន្តចិន → ខ្មែរ
## Chinese Movie → Khmer Voice Translation System

A web-based system to translate Chinese movie audio into Khmer (Cambodian) voice using AI.

🔗 **Live Demo:** `https://YOUR-USERNAME.github.io/khmer-translator/`

---

## ✨ Features

- 🎞️ Upload MP4, MKV, AVI, MOV, MP3, WAV files or paste a URL
- 👂 Chinese speech recognition (Whisper AI)
- 🌐 Chinese → Khmer translation (Claude AI)
- 🗣️ Khmer voice synthesis (Text-to-Speech)
- 📄 Download SRT subtitle files
- ⚙️ Adjustable voice speed, pitch, and gender
- 🎵 Background music preservation option

---

## 🚀 Quick Deploy to GitHub Pages

### Step 1 — Fork or Upload this repo

**Option A: Upload directly**
1. Go to [github.com](https://github.com) and sign in
2. Click **"+"** → **"New repository"**
3. Name it `khmer-translator`
4. Check **"Add a README file"**
5. Click **"Create repository"**
6. Click **"Add file"** → **"Upload files"**
7. Upload `index.html` and all files in this folder
8. Click **"Commit changes"**

**Option B: Use Git (command line)**
```bash
git clone https://github.com/YOUR-USERNAME/khmer-translator.git
cd khmer-translator
# copy your files here
git add .
git commit -m "Initial upload"
git push origin main
```

### Step 2 — Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** (top menu)
3. Scroll down to **"Pages"** in the left sidebar
4. Under **"Branch"**, select `main` and folder `/root`
5. Click **Save**
6. Wait 2–3 minutes
7. Your link will appear: `https://YOUR-USERNAME.github.io/khmer-translator/`

---

## 🔧 API Setup (for full functionality)

The demo works without API keys. For real translation, add these to your backend:

### Required API Keys

| Service | Purpose | Get Key |
|---------|---------|---------|
| OpenAI Whisper | Chinese speech recognition | [platform.openai.com](https://platform.openai.com) |
| Anthropic Claude | Chinese → Khmer translation | [console.anthropic.com](https://console.anthropic.com) |
| Google Cloud TTS | Khmer voice synthesis | [console.cloud.google.com](https://console.cloud.google.com) |

### Environment Variables (for backend)
```
OPENAI_API_KEY=sk-...
ANTHROPIC_API_KEY=sk-ant-...
GOOGLE_CLOUD_API_KEY=AIza...
```

---

## 📁 File Structure

```
khmer-translator/
├── index.html          # Main application
├── README.md           # This file
├── _config.yml         # GitHub Pages config
└── .github/
    └── workflows/
        └── deploy.yml  # Auto-deploy workflow
```

---

## 🛠️ How It Works

```
[Movie File]
     ↓
[Extract Audio] — FFmpeg
     ↓
[Speech Recognition] — OpenAI Whisper (Chinese)
     ↓
[Translation] — Claude AI (Chinese → Khmer)
     ↓
[Voice Synthesis] — Google TTS (Khmer voice)
     ↓
[Merge Audio + Video] — FFmpeg
     ↓
[Download MP4 / MP3 / SRT]
```

---

## 📞 Support

For questions, open an [Issue](../../issues) on this repository.

---

*Built with ❤️ for the Khmer community*

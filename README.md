# J.A.R.V.I.S. Web App

A cinematic full-stack Jarvis AI assistant with voice input, OpenAI TTS audio output, and a HUD-style frontend.

---

## Stack

- **Backend**: Python / Flask
- **Frontend**: Vanilla HTML + CSS + JS (no build step)
- **AI**: OpenAI GPT-4o-mini (chat), Whisper (speech-to-text), TTS-1 (text-to-speech)

---

## Setup

### 1. Install Python dependencies

```bash
pip install -r requirements.txt
```

### 2. Set your OpenAI API key

### 3. Run the server

```bash
python app.py
```

### 4. Open the app



## Features

| Feature | Description |
|
---

## Project Structure

```
jarvis_app/
├── app.py              # Flask backend (chat, TTS, Whisper)
├── requirements.txt
├── README.md
└── static/
    └── index.html      # Full frontend (HTML/CSS/JS)
```

---

## API Endpoints

| Method | Path | Description |
|---|---|---|
| GET | `/` | Serve the frontend |
| POST | `/chat` | Send a message, get JARVIS reply |
| POST | `/speak` | Convert text to audio (base64 MP3) |
| POST | `/transcribe` | Transcribe audio file via Whisper |
| POST | `/reset` | Clear conversation history |

---

## Notes

- The Arc Reactor in the UI glows **red** while listening and **gold** while JARVIS is speaking.
- After recording, your transcription is placed in the text field for review before sending.
- Voice is **OpenAI "onyx"** — the deepest, most authoritative voice available.
# Jarvis

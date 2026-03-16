# Delivery Coach

A mobile-first web app for improving interview delivery through daily practice. Record yourself answering questions, get instant speech analysis, and track your progress over time.

Built to fix four common interview habits: trailing off at the end of answers, overusing filler words, over-explaining instead of being concise, and not being comfortable with silence.

## How it works

The app runs on a 4-day cycle. Each day focuses on one habit:

1. **Land the ending** — practice finishing answers with a short, declarative sentence instead of dissolving into "so yeah..."
2. **Kill the fillers** — identify and replace filler words ("sort of", "I guess", "kind of") with deliberate pauses
3. **Make the point, stop** — say what you need to say and resist the urge to keep going
4. **Sit in silence** — get comfortable with a 5-second pause after your answer lands

Each session takes under 10 minutes: open the app, hit record, answer the question, review your results.

## Features

**Recording**
- Front-facing camera with live video preview
- Real-time speech-to-text transcription via Web Speech API
- Timer and live transcript overlay during recording

**Automated speech analysis**
- Filler word detection and count (tracks "sort of", "I guess", "kind of", "you know", "um", "uh", "like" and more)
- Trailing off detection — flags weak endings based on filler clustering in the last few words
- Word count, speaking pace (WPM), and duration tracking
- Pause detection between phrases
- Transcript with fillers highlighted in brackets

**AI-powered coaching (optional)**
- Connect a free Groq API key for deeper analysis after each recording
- Evaluates ending strength, flags repetition, catches fillers the regex misses
- Returns a one-line actionable coaching note per session

**Video playback**
- Watch yourself back after each recording for body language, posture, and energy
- Self-score on body language, energy, and confidence (1-5 scale)
- Video is never saved — only scores and transcripts persist

**Daily tracking**
- Automatic habit rotation on a 4-day cycle
- Streak counter and session history
- Question bank with 20 built-in questions plus the ability to add your own
- Notes field per session for personal observations

**Export and share**
- One-tap export generates a formatted progress report
- Native share sheet support (WhatsApp, Notes, email etc.)
- Designed to be pasted into a conversation with an AI coach for feedback on trends

**Notifications**
- Optional daily push reminder at a configurable time
- Works via service worker when installed as a PWA

## Tech stack

- Vanilla HTML, CSS, JavaScript — single file, no build step, no dependencies
- Web Speech API for real-time speech-to-text
- MediaRecorder API for video capture
- localStorage for persistent session data
- Service worker for offline caching and push notifications
- PWA manifest for native-like installation on iOS and Android
- Groq API (optional) for LLM-powered speech coaching using Llama 3.1 8B

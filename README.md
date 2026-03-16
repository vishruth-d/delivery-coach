# Delivery Coach

Daily interview delivery practice app. Record yourself answering questions, get instant speech analysis, track progress over time.

## Setup (5 minutes)

### 1. Create the repo

Go to [github.com/new](https://github.com/new) and create a repo called `delivery-coach`. Make it **public**.

### 2. Upload files

Upload all files from this folder to the repo:
- `index.html`
- `sw.js`
- `manifest.json`
- `icon-192.png`
- `icon-512.png`

### 3. Enable GitHub Pages

1. Go to repo **Settings** → **Pages**
2. Under "Source", select **Deploy from a branch**
3. Branch: **main**, folder: **/ (root)**
4. Click **Save**
5. Wait 1-2 minutes for deployment

### 4. Your app is live at:
```
https://vishruth-d.github.io/delivery-coach/
```

### 5. Add to iPhone home screen

1. Open the URL above in **Safari** (must be Safari, not Chrome)
2. Tap the **Share** button (box with arrow)
3. Scroll down, tap **Add to Home Screen**
4. Name it "Coach" or "Delivery"
5. Tap **Add**

Now it's on your home screen like a real app. Opens fullscreen, no browser bar.

## Features

- **Video recording** with front camera
- **Live speech-to-text** transcription
- **Automatic analysis**: filler count, trailing detection, word count, pause detection
- **AI analysis** (optional): add a free Groq API key for deeper coaching
- **4-day habit cycle**: endings → fillers → conciseness → silence
- **Custom questions**: add your own to the rotation
- **Daily notifications**: remind yourself to practice
- **Export**: copy progress report to send to Claude for feedback
- **Share**: use native share sheet to send results anywhere

## Groq AI (optional, free)

1. Go to [console.groq.com/keys](https://console.groq.com/keys)
2. Create a free account
3. Generate an API key
4. Paste it in the app's Settings page

This gives you AI-powered coaching notes after each recording.

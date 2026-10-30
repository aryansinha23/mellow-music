# mellow-music
Mellow: a calm, AI-powered web app that reads your facial expression through the webcam and suggests music to match your mood, in Hindi, English, Punjabi, Haryanvi or a mix.
# 🌿 Mellow – Emotion-Based Music Player

> Your face sets the mood. AI finds the music.

Mellow uses your webcam to read your facial expression in real time, shows the detected emotion with a matching emoji, and recommends music based on your mood, language and genre.

🔗 **Live demo:** https://YOUR-USERNAME.github.io/mellow-music/

## How it works
Webcam → Face detection → Expression analysis → Emotion + confidence → Emoji → Music recommendation → YouTube search

1. The browser reads the webcam stream.
2. A small neural network (face-api.js) finds the face and scores 7 expressions: happy, sad, angry, neutral, fear, surprise, disgust.
3. Results are smoothed over several frames, and an emotion is accepted only at 55% confidence or more.
4. The recommendation engine combines emotion, language, genre and your likes and skips.
5. It opens a matching YouTube search, such as "hindi happy dance songs".

## Features
- Live webcam with face landmarks and status badge
- Stable emotion detection with a confidence meter
- Animated emoji and a short mood message
- Language: Hindi, English, Punjabi, Haryanvi, Mix
- Genre filter: Bollywood, Pop, Rock, Lo-fi, Classical, Hip-Hop, Romantic, Party, Folk, Devotional, Trending
- Like and skip learning during the session
- "For You" recommendations and a mood timeline with session stats
- Attach a photo to analyse it instead of using the camera
- Manual mood selection as a fallback
- Search on YouTube or Brave, dark and light theme, keyboard shortcuts

## Privacy
Camera frames are processed in your browser. They are not stored or uploaded. Stop Camera ends processing immediately. Likes, skips and mood history exist only for the current session.

## Limitations
- The model reads facial expressions, not real feelings, and can be wrong.
- It is not a medical or psychological tool.
- Recommendations are YouTube searches. Playback happens on YouTube, not inside the app.

## Tech stack
HTML, CSS, JavaScript, face-api.js (TinyFaceDetector, expression and landmark models)

## Run locally
Serve the folder over a local server (for example `python -m http.server`) and open `http://localhost:8000`. The camera needs `https://` or `localhost`.

## Author
Your Name · Your College · Year

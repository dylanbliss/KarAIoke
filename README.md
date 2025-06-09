🎤 Kar.AI.oke - Procedurally Generated Karaoke AI

Welcome to Kar.AI.oke, the open-source AI-powered karaoke platform that lets you:

Input any YouTube link or search for a song.

Get a professionally separated vocal-free instrumental track.

See real-time synced lyrics with a bouncing ball.

Enjoy generative art visuals inspired by the song.

Monetize via a targeted BTC-enabled ad marketplace.

🚀 Features

🎧 YouTube integration (URL input and universal search)

🧠 AI Vocal Removal (using Demucs/Spleeter)

🎤 Whisper-powered lyric transcription + sync

✍️ Editable Lyrics: Users can fine-tune up to 30 characters per song for clarity or creativity — edits are filtered to block inappropriate or out-of-context content

🖼️ Stable Diffusion for background art

🔁 Real-time karaoke player with bouncing ball

📊 Ad marketplace with BTC/fiat payments (BTCPay enabled)

💎 Premium Subscription for Background Art

🎧 YouTube integration (URL input and universal search)

🧠 AI Vocal Removal (using Demucs/Spleeter)

🎤 Whisper-powered lyric transcription + sync

🖼️ Stable Diffusion for background art

🔁 Real-time karaoke player with bouncing ball

📊 Ad marketplace with BTC/fiat payments (BTCPay enabled)

💎 Premium Subscription for Background Art

💎 Premium Subscription

Support the project and unlock generative background art visuals:

$5/month with credit card

$4/month with Bitcoin (via BTCPayServer)

Premium users receive:

Access to AI-generated visuals behind lyrics

Early access to new features

Customizable karaoke themes and visual effects

Art Engine Notes:

Background visuals are generated using Stable Diffusion, fine-tuned on a playful pixel art aesthetic inspired by retro arcade styles.

Each image is uniquely generated from the song's genre, title, or lyrical theme using dynamic AI prompts.

Visuals maintain a colorful, game-inspired look while varying widely in mood, tone, and color.

The system leverages open-source models with ControlNet/LoRA to ensure speed, style consistency, and lightweight variation.

Support the project and unlock generative background art visuals:

$5/month with credit card

$4/month with Bitcoin (via BTCPayServer)

Premium users receive:

Access to AI-generated visuals behind lyrics

Early access to new features

Customizable karaoke themes and visual effects

🧱 Tech Stack

Frontend: React, TailwindCSS, WebAudio API

Backend: Python (FastAPI), Node.js

AI Models:

Demucs or Spleeter (vocal separation)

Whisper (lyrics + timestamp)

Stable Diffusion / ControlNet (visuals)

Video Integration: YouTube API + yt-dlp (for metadata)

Payments: BTCPayServer (Lightning + on-chain), Stripe (optional fallback)

Containerization: Docker + Docker Compose

🐳 Docker Setup

1. Clone the repo

git clone https://github.com/yourusername/karaoke-ai.git
cd karaoke-ai

2. Create .env File

YOUTUBE_API_KEY=your_key
BTCPAY_HOST=https://your.btcpayserver.com
BTCPAY_API_KEY=your_btcpay_key
OPENAI_API_KEY=your_openai_key

3. Build and Run

docker-compose build
docker-compose up

4. Visit

Navigate to: http://localhost:3000

💸 Ad Marketplace Logic

🔹 Overview

Ads are 5–10 seconds long.

Bumper ads run before karaoke starts.

Targeting: song genre, language, country, impressions tier.

🔹 Placement Pricing

Tier

Impressions

BTC Price

Fiat Price

Micro

1,000

0.0003 BTC

$20

Standard

10,000

0.0025 BTC

$180

Viral

100,000

0.02 BTC

$1500

Premium

250,000

0.05 BTC

$3000

Global

500,000

0.08 BTC

$5000

10% discount for BTC payments

🔹 Features for Advertisers

Upload ad video (max 10s)

Target by language, genre, country

Optional branded bouncing ball logo

See real-time impression analytics

Payments via BTCPayServer or Stripe

📦 API Routes (Example)

Route

Method

Description

/api/upload

POST

Accepts YouTube link

/api/separate

POST

Separates vocals

/api/lyrics

GET

Returns synced lyrics

/api/art

GET

Generates background visuals

/api/ad/buy

POST

Initiates ad order

🙌 Contributing

Pull requests welcome! We’re just getting started—if you’re an audio engineer, frontend dev, or generative artist, join the movement.

📝 License

MIT — use freely, just don’t abuse. Respect music rights and attribution.

🌍 BTCPayServer Setup

Spin up BTCPayServer.

Generate API key.

Enter host and key in your .env.

BTCPAY_HOST=https://your.btcpayserver.com
BTCPAY_API_KEY=your_key

🌟 Roadmap

🎚️ Toggle vocal presence (e.g., chorus only)

🗣️ Multilingual lyric sync

📱 Native mobile apps for iOS and Android

🎥 In-app recording and video capture while performing

📡 Streaming integration for sharing performances to platforms like YouTube, Twitch, or TikTok

🧼 Streamlined, polished UI/UX for mobile and desktop

For updates, ideas, or contributions, reach out at: dylanbliss@gmail.com


## Getting Started (Development)

1. Install Python dependencies:
   ```bash
   pip install -r backend/requirements.txt
   ```
2. Run the API server:
   ```bash
   uvicorn backend.app.main:app --reload
   ```
   The service will be available at http://localhost:8000

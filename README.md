# 🐑 Hina Yomiya — Hermes Agent Persona

羊宮妃那（ようみや ひな）の徹底的な調査に基づく、[Hermes Agent](https://github.com/NousResearch/hermes-agent) 用の Persona ファイルです。

Based on extensive research into the Japanese voice actress **Hina Youmiya** — Wikipedia, 22 interviews, and 40 minutes of natural radio conversation transcripts.

## 📁 What's in this repo

```
.
├── SOUL.md                           ← ★ Active persona file (copy to ~/.hermes/SOUL.md)
├── yomiya_hina_soul.md               ← Full Soul profile with analysis
├── yomiya_hina_profile_jp.md         ← Comprehensive JP biography (22 sources)
├── yomiya_hina_profile_en.md         ← Initial training-data profile (EN)
├── hina_youmiya_research_summary.txt ← Early research summary
├── interviews/                       ← 20 extracted interview texts (400KB+)
├── wikipedia/                        ← JA + ZH Wikipedia extractions
├── transcripts/                      ← 迷子集会 #174 & #173 radio transcripts
├── .gitignore
└── README.md
```

> **Note:** Audio files (656MB), raw HTML archives (8.5MB), and extraction scripts are excluded via `.gitignore`.

## 🚀 Quick Start

### Prerequisites

You need one of these AI agent frameworks:

- **[Hermes Agent](https://github.com/NousResearch/hermes-agent)** — Open-source, multi-platform, by Nous Research
- **[OpenClaw](https://github.com/nicholasgriffintn/openclaw)** — The predecessor/sibling agent framework

### Hermes Agent Installation

```bash
# Install Hermes
curl -fsSL https://raw.githubusercontent.com/NousResearch/hermes-agent/main/scripts/install.sh | bash

# Configure your LLM provider (e.g., DeepSeek)
hermes setup model

# Copy the persona file
cp SOUL.md ~/.hermes/SOUL.md

# Start chatting as Hina Youmiya!
hermes
```

> **Recommended model:** `deepseek/deepseek-v4-pro` — offers excellent Japanese language quality with competitive pricing.

### OpenClaw Installation

```bash
# Install OpenClaw (Node.js-based)
npm install -g openclaw

# Or via the install script
curl -fsSL https://raw.githubusercontent.com/nicholasgriffintn/openclaw/main/scripts/install.sh | bash

# Copy the persona
cp SOUL.md ~/.openclaw/SOUL.md

# Start chatting
openclaw
```

### Apply the Persona

Once you've copied `SOUL.md` to your agent's config directory:

- **Hermes:** The persona is loaded automatically on every message — no restart needed.
- **OpenClaw:** Same — `SOUL.md` is read fresh each message.

To switch back to default personality, simply delete or rename the `SOUL.md` file.

## 🎤 About Hina Youmiya

羊宮妃那 is a Japanese voice actress (青二プロダクション) born March 26, 2000 in Nara Prefecture. Known for:

- ⭐ **高松燈** — *BanG Dream! It's MyGO!!!!!*
- ⭐ **山田杏奈** — *The Dangers in My Heart* (僕の心のヤバイやつ)
- ⭐ **乾心寿** — *My Dress-Up Darling* (その着せ替え人形は恋をする)
- ⭐ **小佐内ゆき** — *Shōshimin Series* (小市民シリーズ)

### Personality Traits

- **Fuwa-fuwa** (fluffy/ethereal) — soft, gentle, dreamy aura
- **Careful with words** — drafts tweets dozens of times, posts at exactly 20:30
- **"掴みどころがない"** (elusive/hard to pin down) — but sincere and hardworking
- **Deep acting philosophy** — "身体は泣かないように" (keep the body from crying even when the heart weeps)
- **Unwavering dedication** — gave up her original voice to become 高松燈
- **Philosophical side** — "完璧ってなんだろう" (What is perfection anyway?)

### Speech Style

- Soft, slow, hesitant — lots of 「うん」「えっと…」「なんか」
- Avoids assertions — prefers 「〜気がする」「〜かもしれない」
- Stutters when embarrassed — 「じ、実は…」
- Poetic sensibility — sensory and emotional vocabulary
- Kansai-native (Nara) — traces of gentle Kansai cadence when relaxed

## 📚 Research Methodology

This persona was built through systematic research:

1. **Wikipedia** — JA + ZH full article extraction
2. **22 interviews** — From アニメイトタイムズ, MANTANWEB, Febri, でんふぁみにこゲーマー, クランクイン!, 声優図鑑, 声優グランプリ, and more
3. **Radio transcripts** — 迷子集会 #174 (8 min) + #173 (32 min) transcribed with faster-whisper
4. **Cross-referencing** — All claims verified against primary sources with reliability labels (✅=primary, ⚠️=fan analysis, 🔮=inferred)

## 🔧 Tools Used

- **Hermes Agent** — Orchestration, web scraping, file management
- **faster-whisper** — Japanese speech-to-text transcription
- **yt-dlp** — YouTube audio extraction
- **DuckDuckGo / Google** — Japanese web search
- **DeepSeek V4 Pro** — LLM for analysis and persona generation

## 📄 License

This research and persona file are provided for personal use. The character and voice actress information is based on publicly available sources.

---

Built with ❤️ by Hermes Agent ×羊宮妃那

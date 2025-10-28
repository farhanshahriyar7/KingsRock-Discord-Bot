
```markdown
# 🎵 KingsRock Discord Bot

An **AI-ready, full-featured bot** built with **Python**, **Lavalink**, and **Supabase** — designed for currently powerful music playback, user playlists, and real-time server logging.  
Built by **KingsRock Management** ❤️‍🔥

---

## 🚀 Overview

KingsRock Discord Bot is a next-gen bot that currently delivers **premium music control, playlist management, lyrics search, and Supabase-powered analytics** — all wrapped in a clean, modular Python architecture.

---

## ⚙️ Tech Stack

| Layer | Technology |
|--------|-------------|
| Language | Python 3.10+ |
| Bot Framework | discord.py (v2.x) |
| Music Backend | Lavalink |
| Database | Supabase (PostgreSQL + REST API) |
| Hosting | Railway / Render |
| Auth | Discord OAuth2 |
| Docs | Markdown + GitHub Wiki |

---

## ✨ Features

✅ **Slash Commands & Prefix Support**  
✅ **High-quality music playback via Lavalink**  
✅ **Queue system with embeds**  
✅ **Server & user playlists stored in Supabase**  
✅ **Lyrics search via Genius API**  
✅ **Activity logs and server analytics**  
✅ **DJ roles & server config system**  
✅ **Auto-reconnect and idle timeout**  
✅ **Modular cog-based design**

---

## 🧱 Project Structure

```

discord-advanced-music-bot/
├── bot.py                # Entry point
├── cogs/
│   ├── music.py          # Playback, queue, controls
│   ├── playlist.py       # Playlist management
│   ├── admin.py          # DJ role & settings
│   ├── lyrics.py         # Lyrics fetch command
│   └── **init**.py
├── utils/
│   ├── embeds.py         # Dynamic embed templates
│   ├── queue.py          # Song queue logic
│   ├── logger.py         # Activity logs
│   └── supabase_client.py # DB integration layer
├── config/
│   ├── config.yaml       # Lavalink, API keys
│   └── **init**.py
├── requirements.txt
├── README.md
└── .env.example

````

---

## 🔑 .env Configuration

```bash
DISCORD_TOKEN=your_discord_bot_token
LAVALINK_HOST=localhost
LAVALINK_PORT=2333
LAVALINK_PASSWORD=your_lavalink_password
SUPABASE_URL=https://xyzcompany.supabase.co
SUPABASE_KEY=your_service_role_key
GENIUS_API_KEY=your_genius_api_key
````

> ⚠️ **Never commit your `.env` file** — only keep `.env.example` for reference.

---

## 🛠️ Installation & Setup

### 1️⃣ Clone the repository

```bash
git clone https://github.com/yourname/discord-advanced-music-bot.git
cd discord-advanced-music-bot
```

### 2️⃣ Create virtual environment

```bash
python -m venv venv
source venv/bin/activate   # macOS/Linux
venv\Scripts\activate      # Windows
```

### 3️⃣ Install dependencies

```bash
pip install -r requirements.txt
```

### 4️⃣ Setup Lavalink

* Download Lavalink.jar from [Lavalink Releases](https://github.com/freyacodes/Lavalink/releases)
* Create `application.yml` with your config
* Run with:

```bash
java -jar Lavalink.jar
```

### 5️⃣ Setup Supabase

* Create a new Supabase project at [supabase.com](https://supabase.com)
* Run migrations from `/supabase/migrations`
* Add your `SUPABASE_URL` and `SUPABASE_KEY` to `.env`

### 6️⃣ Run the bot

```bash
python main.py
```

---

## 🧠 Command Examples

| Command                 | Description            |
| ----------------------- | ---------------------- |
| `/play [song/url]`      | Play or queue a song   |
| `/pause`                | Pause playback         |
| `/resume`               | Resume playback        |
| `/skip`                 | Skip to next track     |
| `/queue`                | View current queue     |
| `/playlist save [name]` | Save current queue     |
| `/playlist load [name]` | Load a playlist        |
| `/lyrics [song name]`   | Fetch song lyrics      |
| `/config djrole [role]` | Set DJ role for server |

---

## 📦 Database Schema (Supabase)

**Tables:**

* `users` → id, username, premium, joined_at
* `servers` → id, name, prefix, dj_role
* `playlists` → id, user_id, title, songs (JSONB)
* `logs` → id, server_id, action, timestamp

---

## 🧩 Contributing

We love contributions! 🫶

1. Fork this repo
2. Create your branch

   ```bash
   git checkout -b feature/your-feature
   ```
3. Commit your changes

   ```bash
   git commit -m "feat(music): add fade transition between songs"
   ```
4. Push & create Pull Request

   ```bash
   git push origin feature/your-feature
   ```

---

## 🧾 Commit Style Guide

Follow **Conventional Commits**:

```
feat(scope): add something new
fix(scope): fix something broken
chore: update dependency or config
docs: update documentation
```

---

## 🪩 Deployment (Recommended)

* **Option 1:** Railway.app (free Lavalink & Python runtime)
* **Option 2:** Docker Compose
* **Option 3:** VPS (example: Hetzner / Linode)

---

## 📈 Roadmap

* [ ] Supabase event logging dashboard
* [ ] Spotify playlist import
* [ ] Web dashboard (React + Supabase)
* [ ] AI-powered song recommendation

---

## 🧑‍💻 Authors

**Farhan Shahriyar** — [@farhanshahriyar7](https://github.com/farhanshahriyar)
**Mashrur Bin Morshed** — [@MashrurBinMorshed](https://github.com/MashrurBinMorshed)

---

## 🪪 License

MIT License © 2025 Farhan Shahriyar & Mashrur Bin Morshed
Feel free to fork, extend, or remix — just give credit 🎶

---

## 💬 Support

Need help?
Join our Discord or open an issue on GitHub!

```




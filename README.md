# 🤖 Universal Daily Video Automation

This is a fully automated video bot designed for **ANY** category (Affiliate, Gaming, Motivation, Crypto, etc.). It automatically picks a random video from your folder, assigns a unique title & caption from your list, and posts it to **Telegram** and a **Webhook** (for Make.com/n8n).

## ⚙️ How to Customize for YOUR Niche

Open `main.py` and simply **replace** the text inside these variables to match your category:

1.  **`TITLES_GRID`**: Add your own 50+ titles (e.g., "Best Gym Workout", "Funny Cat Moment", "Crypto Alert").
2.  **`CAPTIONS_GRID`**: Add your own captions (e.g., "Follow for more!", "Link in bio", "Tag a friend").
3.  **`FIXED_HASHTAGS`**: Paste your 30-40 generic hashtags here (sent with every post).
4.  **`INSTA_HASHTAGS`**: Paste your top 5 specific SEO hashtags here (sent to Webhook for Instagram).

## 📂 File Structure
* `videos/` → Upload your video files here (.mp4).
* `main.py` → The main script (Edit this to change text).
* `requirements.txt` → Create this file and write `requests` inside.
* `history.json` → Create this file and write `[]` inside.
* `.github/workflows/daily_bot.yml` → The automation timer file.

## 🔐 GitHub Secrets (Settings > Secrets)
Go to **Settings** > **Secrets and variables** > **Actions** and add these 3 secrets:

| Secret Name | Value |
| :--- | :--- |
| `TELEGRAM_TOKEN` | Your Bot API Token (from BotFather). |
| `TELEGRAM_CHAT_ID` | Your Channel ID (e.g., -100xxxxxxx). |
| `WEBHOOK_URL` | Your Make.com or n8n Webhook URL. |

---
*Just upload videos, update the text lists in `main.py`, and the bot handles the rest!*

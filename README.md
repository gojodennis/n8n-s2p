## INCOMPLETE!

# 🎓 Syllabus to YouTube Playlist (n8n Automation)

This n8n workflow converts a syllabus topic into a curated YouTube playlist. Ideal for self-learners, educators, and content curators who want to instantly generate focused learning playlists from any subject keyword.

---

## 🧠 What It Does

- Accepts a syllabus topic (via chatbot input)
- Searches YouTube for relevant, recent videos
- Creates a new YouTube playlist titled with the search topic
- Adds the top results to the playlist
- Logs both playlist and video IDs into Google Sheets for tracking and future reference

---

## ⚙️ Integrations Used

- **YouTube API** – Search videos, create playlists, add items
- **Google Sheets API** – Store playlist and video IDs
- **n8n Chat Trigger Node** – Receives input topic dynamically (can be connected to Telegram, Discord, etc.)

---

## 🚀 Flow Overview

[Chat Trigger]
→ [Search Videos by Topic]
→ [Create Playlist]
→ [Log Playlist ID to Sheet]
→ [Append Video IDs to Sheet]
→ [Add Videos to Playlist]


---

## 📁 Google Sheets Columns

Two sheets used:
- `videoID` — Logs each video added
- `playID` — Logs each playlist created

---

## 📌 Setup Instructions

1. Import the file: `Syllabus to Youtube playlist.json` into n8n.
2. Set up OAuth credentials for:
   - **YouTube OAuth2**
   - **Google Sheets OAuth2**
3. Connect a chatbot platform if using the `Chat Trigger` (or trigger manually via webhook).
4. Customize your Google Sheet document ID and Sheet names if needed.

---

## 💡 Use Cases

- Auto-generate learning playlists for students based on syllabus topics
- Build knowledge bases around any input domain
- Combine with AI summarization tools for deeper learning paths

---

## 🐚 License

MIT

---

## 🔗 Credits

Built with [n8n](https://n8n.io), YouTube Data API, and Google Sheets.

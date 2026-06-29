# 🌀 JoJo Daily Facts Database

A community-driven database of **JoJo's Bizarre Adventure** facts designed for Discord bots, webhooks, Scriptable, and other applications.

## Features

- 📖 Hundreds of curated JoJo facts
- 🎲 Random fact selection
- 🔄 No-repeat support
- 🌐 GitHub-hosted JSON database
- 📦 Easy to expand
- ⚡ Works with Scriptable, Discord bots, and web applications

---

# Repository Structure

```
jojo-facts/
│
├── README.md
├── database.json
├── progress.json
│
├── part1.json
├── part2.json
├── part3.json
├── part4.json
├── part5.json
├── part6.json
├── part7.json
├── part8.json
├── part9.json
│
├── stands.json
├── hamon.json
├── spin.json
├── protagonists.json
├── villains.json
├── allies.json
├── locations.json
├── anime.json
├── manga.json
├── trivia.json
└── eastereggs.json
```

---

# Database Format

Each JSON file contains an array of fact objects.

Example:

```json
[
  {
    "id": 1,
    "part": 3,
    "character": "Jotaro Kujo",
    "category": "Stand",
    "spoiler": false,
    "fact": "Star Platinum possesses incredible speed, precision, and strength."
  }
]
```

---

# Fact Fields

| Field | Description |
|--------|-------------|
| id | Unique ID within the file |
| part | JoJo Part number |
| character | Main character related to the fact |
| category | Type of fact |
| spoiler | Indicates if the fact contains spoilers |
| fact | The fact text |

---

# Categories

Examples include:

- Character
- Stand
- Hamon
- Spin
- Villain
- Ally
- Location
- Race
- Manga
- Anime
- Music Reference
- Trivia
- Behind the Scenes
- Araki
- Power System
- Ability
- Quote
- Easter Egg

---

# Parts Included

- Phantom Blood
- Battle Tendency
- Stardust Crusaders
- Diamond Is Unbreakable
- Golden Wind
- Stone Ocean
- Steel Ball Run
- JoJolion
- The JOJOLands

---

# Goals

Current Goal

- 500 curated facts

Future Goals

- 1,000 facts
- Character images
- Episode references
- Manga chapter references
- Anime episode references
- Source citations
- Multi-language support

---

# Contributing

Contributions are welcome.

Please ensure:

- Facts are accurate.
- Avoid duplicate facts.
- Keep grammar consistent.
- Mark spoilers appropriately.
- Use proper JSON formatting.

---

# Example Applications

This database can be used for:

- Discord bots
- Discord webhooks
- Scriptable automation
- Mobile widgets
- Websites
- Trivia games
- JoJo quizzes
- APIs

---

# License

This repository is intended for educational and fan projects.

JoJo's Bizarre Adventure and its characters are the property of Hirohiko Araki and their respective copyright holders.

This repository contains original fan-written trivia and metadata only and does not include copyrighted manga or anime content.

---

## ⭐ Star the repository if you find it useful! for webhook

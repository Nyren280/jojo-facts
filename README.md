# JoJo Facts Database

This repository is a modular, JSON-based collection of facts about JoJo's Bizarre Adventure. It is designed so new databases can be added without changing code: the master index (database.json) lists every data file the application should read.

Repository structure

- database.json — master index listing all database files and metadata
- progress.json — tracks which facts have been posted and when
- part1.json ... part9.json — part-specific fact databases
- stands.json, hamon.json, spin.json — technique and Stand databases
- protagonists.json, villains.json, allies.json — character group databases
- locations.json — in-universe locations
- anime.json, manga.json — production and publication facts
- trivia.json — behind-the-scenes facts
- eastereggs.json — hidden references and callbacks
- README.md — this file
- .gitignore — local ignores

JSON schema for fact objects

Every facts file is a JSON array of objects. Each object should follow this schema:

{
  "id": 1,
  "part": 1,
  "title": "Jonathan Joestar",
  "character": "Jonathan Joestar",
  "category": "Character",
  "spoiler": false,
  "difficulty": "Easy",
  "source": "Phantom Blood",
  "fact": "Jonathan Joestar is the first JoJo in the series."
}

Guidelines and conventions

- Use numeric, unique `id` values per file (start at 1 for each file).
- `part` should be the originating part number where applicable, or 0 if not applicable.
- `category` should be one of: Character, Stand, Technique, Location, Anime, Manga, Trivia, Easter Egg, etc.
- `spoiler` toggles whether the fact contains major spoilers (true/false).
- `difficulty` is a human-readable classification (Easy/Medium/Hard).
- Keep `fact` concise and self-contained.

How the application uses database.json

The application should read database.json first to discover which files to load. This allows adding new files without a code change — only database.json needs updating.

Contribution guidelines

1. Fork the repository and create a branch for your changes.
2. Add or update JSON files; keep the schema consistent.
3. Add meaningful commit messages and open a pull request describing the changes.
4. Avoid adding personally identifiable information.

Future goals and recommendations

- Expand the dataset to 1,000+ curated facts across databases.
- Add a validation script (Node.js/Python) to assert schema correctness and unique IDs.
- Add CI checks to run the validation script on PRs.
- Add scripts to export facts as CSV/Markdown for other tooling.
- Consider tagging facts with additional metadata (tags, language, contributors).

License

Specify a license in a future PR if needed.

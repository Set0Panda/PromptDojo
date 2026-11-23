# Prompt Dojo

A browser game that teaches everyday people how to use Claude — and that AI is not Google.

Seven belts, one habit each (talk don't search, give details, keep the conversation going, let it do the job, show it things, check what matters, freestyle test), across five themes: home & family, work, health & wellbeing, money & paperwork, free time & hobbies. Aimed at adults (40+) who know about AI but rarely use it.

Available in English and Spanish (Spain). The game opens in Spanish for Spanish-language browsers, and players can switch at any time with the language picker.

Everything is one self-contained file: `index.html`.

## Adding a language
All text lives in the `LANGS` object near the top of the script. Copy the `en` block, translate the values, give it a new key (e.g. `es`) and a `langName`. A language picker appears automatically once there is more than one.

## Note on scoring
The black-belt test uses Claude for scoring when the page runs as a Claude artifact. On GitHub Pages it falls back to a simple built-in checker.

## Retrying a belt

Each belt has a pool of questions (the base set plus `LANGS.<lang>.extra`). Every attempt draws a fresh set and avoids questions seen in the last attempt; once a pool is used up it starts recycling the oldest. When adding a language, add the same `extra` pool in the same order so progress carries across language switches.

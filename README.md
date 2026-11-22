# Prompt Dojo

A browser game that teaches everyday people how to use Claude — and that AI is not Google.

Seven belts, one habit each (talk don't search, give details, keep the conversation going, let it do the job, show it things, check what matters, freestyle test), across five themes: everyday life, work, health & fitness, money & paperwork, gaming & hobbies.

Available in English and Spanish (Spain). The game opens in Spanish for Spanish-language browsers, and players can switch at any time with the language picker.

Everything is one self-contained file: `index.html`.

## Adding a language
All text lives in the `LANGS` object near the top of the script. Copy the `en` block, translate the values, give it a new key (e.g. `es`) and a `langName`. A language picker appears automatically once there is more than one.

## Note on scoring
The black-belt test uses Claude for scoring when the page runs as a Claude artifact. On GitHub Pages it falls back to a simple built-in checker.

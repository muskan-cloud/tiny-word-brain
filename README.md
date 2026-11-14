# Tiny Word Brain 2.0 — Slang Translator

A lightweight, browser-only English ↔ slang translator with Gen Z, Gen Alpha, and mixed styles.

## Run it locally
Open `index.html` in a modern browser. No installation, build step, API key, or backend is needed.

## Features
- English → slang and slang → plain-English directions
- Gen Z, Gen Alpha, or mixed style
- Ten intensity levels, from subtle to full brainrot
- Phrase-aware substitution rules and examples
- Copy result and use a translation as the next input
- All processing happens locally in the browser; text is not uploaded

## Important limitation
This version is a rule-based translator, not a trained neural language model. It uses hand-written phrase and vocabulary rules. Slang is contextual, regional, and constantly changing, so results are playful approximations rather than authoritative translations.

## Free hosting with GitHub Pages
1. Open this repository's **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select branch **main** and folder **/(root)**, then click **Save**.
4. Wait for the published URL shown on the Pages settings screen.

The URL will be:
`https://muskan-cloud.github.io/tiny-word-brain/`

No server process is required: GitHub Pages serves the static website, and each visitor's browser runs the translator. GitHub Pages is free for public repositories on GitHub Free.

## Customize the slang
Open `index.html` and edit the `rules` array (English → slang) and `decode` array (slang → English) inside the script. Add longer phrases before shorter phrases so phrase matches get priority.

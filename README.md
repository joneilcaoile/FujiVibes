# Film Vibes

A film recipe generator for Fujifilm cameras. Describe the vibe you're going for, use any AI to generate recipes, then download ready-to-import .FP1 preset files for [Fuji X Raw Studio](https://fujifilm-x.com/en-us/support/download/software/x-raw-studio/).

**Live app:** [joneilcaoile.github.io/FujiVibes](https://joneilcaoile.github.io/FujiVibes/)

## How it works

1. **Describe your vibe.** Use guided questions (occasion, subjects, mood, lighting, grain preference) or write freeform. Pick how many presets you want (1, 3, 5, or 7).
2. **Copy the generated prompt** and paste it into any AI (ChatGPT, Claude, Gemini, etc.). The prompt tells the AI exactly what JSON format to return.
3. **Paste the AI's JSON response** back into the app. It validates the data and shows you each preset with its use case and best shooting conditions.
4. **Download your .FP1 files.** One file per preset, packaged as a zip. Drop them into `C:\Users\[you]\AppData\Local\com.fujifilm.denji\X_RAW_STUDIO\` and they're ready to load onto your camera via USB.

## Why the copy-paste workflow?

The AI processing happens on your own account, not through this app. No API keys stored, no data collected, no server. You choose which AI you trust, and the app just handles the Fujifilm-specific file format.

## Supported cameras

Any Fujifilm X-series or GFX body that works with X Raw Studio. Film simulation availability adapts to your camera's sensor generation (X-Trans III, IV, V).

## Tech

Single HTML file. No build step, no dependencies beyond [JSZip](https://stuk.github.io/jszip/) (CDN). Runs entirely in the browser.

## License

MIT

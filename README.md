# Flyer Studio

A single-file flyer and infographic generator that runs in the browser. Describe what you need in plain words. An LLM plans the layout and copy, and the page renders it with **real typography and real charts** instead of asking an image model to paint text and numbers (which is where garbled, "sloppy" AI graphics come from). Image models only supply background artwork.

**Live:** https://lowriskbtc.github.io/flyer-studio/

## How it avoids slop

- The planner returns structured JSON (hero, steps, bars, cta and other blocks), not a picture.
- Text, numbers and charts are set as live HTML/CSS/SVG, so they stay sharp and correct.
- Generated art is optional and sits behind the type, never carrying the words.
- Export to PNG with html2canvas.

## Use it

Open `index.html`, or the live page above. Pick an image provider:

- **Pollinations**: free, no key.
- **Gemini**: paste your own API key. It is kept only in your browser's local storage and is sent only to Google's API. Nothing is stored on a server, and no key is in this repository.

## Files

- `index.html`: the whole app (HTML, CSS and JS, no build step).

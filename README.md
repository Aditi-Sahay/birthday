# Happy birthday digital card

A single-page, four-screen birthday interaction built as a playful gift and a small front-end portfolio piece. Purple synthwave/CRT aesthetic, pixel-styled UI, zero dependencies to install


---

## What it does

A 4-screen quiz flow, gated by a "continue" button and tracked with a pixel progress indicator at the top:

| Screen | Content |
|---|---|
| **1. Landing** | Glitchy pixel title + subtitle, animated synthwave grid horizon, twinkling stars, CRT scanline overlay |
| **2. Question one** | *"question with 2 possible answers"* — Yes/No both lead somewhere sweet, reaction text fades in before the continue button appears |
| **3. Question two** | *"question with one possible answer"* — the **NO** button dodges the cursor (and finger, on touch) every time it's approached, with a rotating set of teasing captions, until **YES** is the only option left standing |
| **4. The letter** | A closing message in a terminal-style dashed box, with a heart-burst animation and a "play again" link |

## Tech Stack 

- Plain **HTML / CSS / vanilla JS**
- Fonts: [`Press Start 2P`](https://fonts.google.com/specimen/Press+Start+2P) (pixel display) + [`VT323`](https://fonts.google.com/specimen/VT323) (retro terminal body), loaded from Google Fonts
- All color/theme values are CSS custom properties for easy re-skinning
- Respects `prefers-reduced-motion`
- Fully responsive (tested down to small mobile widths)

## Customizing

Everything lives in one file, so editing is just find-and-replace:

- **The letter**: search for `<!-- EDIT THIS LETTER -->` — replace the lorem ipsum paragraphs and the `YOUR NAME HERE` sign-off with your own message
- **Names / copy**: the headline and questions are plain text in the `<section>` blocks — search for `SHIULI` to update the name
- **Colors**: all defined as CSS variables at the top of the `<style>` block (`--purple`, `--pink`, `--void`, etc.) — change these to re-theme the whole page
- **Fonts**: swap the Google Fonts `<link>` and the `font-family` values if you want a different pixel/retro pairing

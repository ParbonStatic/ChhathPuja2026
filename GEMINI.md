# GEMINI.md — Project context

**Project:** Chhath Mahaparv 2026 tribute site (ParbonStatic template).
**Architecture:** Zero-build. All HTML, CSS, inline SVG and vanilla JS live in `index.html`. Fonts: Google Fonts (Syne, Playfair Display italic, Caveat, Noto Serif Devanagari, Rozha One, Plus Jakarta Sans).

## Design rules
- Warm palette tokens in `:root` (haldi, saffron, sandur, ganga blue, ivory); no pure black — text is `--ink` brown.
- `body::before` holds the translucent fixed background artwork (inline SVG data URIs).
- Zine layout: pill navbar, split hero + polaroid collage (`.floating-tag` z-index 4 above `.polaroid` z-index 2), tilted marquee, alternating `.sec-head`/`.sec-head.flip`, staggered `.stagger-3`, 12-col `.bento`.

## Interactive module (`#arghya`)
Vibe chips → editable wish → "Offer Arghya" → sunrise glow, petals, confetti → card with Copy / Share / Save PNG (offscreen 1200×800 canvas) / Print.

## Open Graph
Absolute URLs point to `https://parbonstatic.github.io/ChhathPuja2026/og-image.png`. Keep `og-image.svg` as the source and re-export `og-image.png` (1200×630) after edits.

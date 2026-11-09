# Portfolio site notes

Static GitHub Pages site. Everything lives in `index.html`; images live in `assets/`. No build step.
Pushing to `main` publishes to https://wathanya11.github.io within a minute or two.

## Content rules
- English is the default. Every translatable element has `data-i="key"`; its Thai text sits in the `TH` object in the script at the bottom. Any new `data-i` key needs a `TH` entry.
- Only write facts the owner gave. Ask before adding dates, numbers or claims.
- Joined Next Gen Business Club in 2025 as Gen 6 (not 2024 / Gen 5).

## Design: whiteboard
- Off-white board, blue marker ink (`--blue`), hand-lettered headings (Patrick Hand SC), notes in Caveat, body in Mali.
- `.sk` = sketchy blue frame (add `.dbl` for a double line), `.fill` = solid blue box, `.board` = white card.
- Headline second lines use `<span class="it">` (outlined text).
- The red hand-drawn oval button (`.xp-link.pj-go`) opens a project page.

## Adding a project page
1. In an experience item, add `<button class="xp-link pj-go" data-go="ID" type="button">…</button>` (copy an existing one).
2. Add `<section id="ID" class="pj-page" hidden>` with a `.pj-bar` back button (`.pj-back` with `data-from="ID"`). Copy an existing project section as the template.
3. Put new images in `assets/` and reference them as `assets/name.jpg`.

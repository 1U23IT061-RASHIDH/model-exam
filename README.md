# Food Paradise

A responsive restaurant website for Food Paradise, built as an MCA model-exam project with a shared two-column page layout, local food photography, restaurant ambience audio, and a printable menu PDF.

## Technologies

- HTML5 for the semantic pages and native audio controls
- CSS3 for layout, typography, and responsive styling
- Vanilla JavaScript (Node.js) for generating the menu PDF; the website itself has no JavaScript framework dependencies

## Website pages

- [Home](index.html) — restaurant introduction, featured dishes, ambience player, and sidebar information
- [Menu](menu.html) — dish categories, prices, sidebar links, and PDF viewing/downloading
- [About](about.html) — story, mission, vision, food quality, and customer service

## Features

- Shared header, navigation, centered container, main content, sidebar, and footer on all three pages
- Responsive two-column desktop layout that stacks on smaller screens
- Local photographs in `images/`; no remote image dependencies
- `normalize.css` loaded before `main.css` on every page
- Native HTML5 audio player with play/pause, volume, and progress controls; playback never starts automatically
- A two-page A4 menu PDF with the website's categories, dishes, descriptions, prices, and local food photographs
- PDF view and download links on the menu page
- Float and clearfix demonstration on the homepage

## Audio

The player uses `audio/restaurant-ambience.mp3`, a genuine restaurant field recording by stephan. The recording is public domain; see the [Wikimedia Commons file page](https://commons.wikimedia.org/wiki/File:Restaurant_ambience.ogg) for the source and license information.

## Menu PDF

The generated PDF is at `documents/food-paradise-menu.pdf`. To regenerate it after changing the menu or its photographs, run this from the repository root:

```text
node scripts/generate-menu-pdf.js
```

The script uses only Node.js built-in modules and the existing JPEGs in `images/`.

## Folder structure

```text
model-exam/
├── index.html
├── menu.html
├── about.html
├── styles/
│   ├── normalize.css
│   └── main.css
├── images/
├── audio/
│   └── restaurant-ambience.mp3
├── documents/
│   └── food-paradise-menu.pdf
├── scripts/
│   └── generate-menu-pdf.js
└── README.md
```

## Links

- Live website: https://1u23it061-rashidh.github.io/model-exam/index.html
- GitHub repository: https://github.com/1U23IT061-RASHIDH/model-exam

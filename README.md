# Peterson Linen — website

Static HTML. No build step. Open `index.html` in a browser, or serve the folder.

## Pages
| File | Page |
| --- | --- |
| index.html | Home |
| about.html | About / Pamelyn Collins |
| services-personal-events.html | Services — Personal Events |
| services-corporate-events.html | Services — Corporate Events |
| our-linens.html | Our Linens + sizing guide |
| portfolio.html | Portfolio galleries |
| how-it-works.html | How It Works |
| faq.html | FAQ |
| trade.html | Trade & affiliates |
| contact.html | Contact + quote form |

## Structure
- `support.js` — the page runtime. Every page loads it; keep it alongside the HTML.
- `assets/` — photography and logo.
- `assets/fonts/Caramella_Regular.ttf` — the heading face, self-hosted via an `@font-face` rule in every page. Push this folder with the HTML or headings fall back to a serif.
- Body text (Libre Franklin) loads from Google Fonts; no other external dependency.

**Everything in this folder must be pushed together.** The pages reference `support.js` and `assets/` with relative paths — HTML files alone will render text with no images and no runtime.

## GitHub Pages
Push this folder's contents to the repository root (or `/docs`), then enable Pages for that branch and folder. No configuration needed.

## Outstanding content
- Portrait of Pam (about.html — placeholder image and caption in place).
- Portfolio captions: venue names and pieces used per event.
- Swatch-scale fabric photography for Collections and the linen catalog.
- Trade numbers: trade discount rate, payment terms, affiliate referral percentage (marked TBD).
- Quote form on contact.html has no backend — wire it to an email handler or form service.

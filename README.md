# Oku site concepts

The Oku marketing site: the home page and every feature and info page, with all the images they use.

## Open it

Unzip, then open `site/index.html` in Chrome, Safari or Firefox. Every page links to the others.

Some browsers limit pages opened straight from your disk. If anything looks off, serve the folder instead:

```
cd site
python3 -m http.server 8000
```

Then go to http://localhost:8000.

The pages load three things from the internet: the Inter typeface (Google Fonts), smooth scrolling (Lenis, from jsDelivr) and the company logos inside the app preview. Without a connection everything still works, in a fallback font.

## Pages

| File | Page |
| --- | --- |
| `index.html` | Home |
| `stocks.html` | Stocks and ETFs |
| `leverage.html` | Leverage |
| `earn.html` | Earn |
| `borrow.html` | Borrow, before launch. A switch at the bottom of the page opens the launch version |
| `borrow-launch.html` | Borrow, at launch |
| `social.html` | Social |
| `referrals.html` | Referrals |
| `availability.html` | Availability: the country checker, map and full list |
| `start.html` | Getting started |
| `support.html` | Support |
| `faq.html` | FAQ |
| `about.html` | About us |
| `app.html` | The Oku app preview that plays inside the phone on the home page |

`img/` holds every photo, app screen and graphic the pages use. Most section photos come in three widths (1600, 2560 and 3840 pixels), so high-resolution screens get the sharp one.

## The code

Each page is one self-contained HTML file: its markup, styles and scripts are all inline, so there is nothing to install or build. To share a link, upload the `site` folder as it is to any static host, such as Netlify, Vercel, Cloudflare Pages, GitHub Pages or an S3 bucket.

## Figures

Stock prices, returns and balances on the pages are illustrative, the same ones the app's own screens show. The bank loan rate on the Borrow pages cites the Federal Reserve's G.19 Consumer Credit release of October 7, 2026.

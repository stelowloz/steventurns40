# How this site works

This repository is the live site at https://steventurns40.com, served by GitHub Pages from the `main` branch. A push to `main` is a deploy and goes live in about a minute.

## Layout

- `index.html` is the whole site: styles, markup and script in one file. `404.html` is a copy of it, so keep the two identical.
- `img/` holds the photos, JPEG, 1280px wide (the Tokyo panorama is 2000px).
- `CNAME` and `.nojekyll` are required by GitHub Pages. Leave them alone.

## Where things live in index.html

- Trip content is data near the top of the script: `LEGS`, `SHOTS`, `HOPS`, `JOIN`, `EAT`, `CHAPTERS` (the day-by-day text), `STAYS`, `CLOCK` (booking deadlines), `LINKS`, `FAQ` and `CREDITS`.
- Each day's photo and caption is set in `PH`, the calendar labels in `CAL`.
- Colours are tokens on `:root`, with dark-theme values in the two dark blocks. Every destination has a two-tone pair such as `--jp` and `--jp2`.
- Pages are hash routes: `#trip`, `#days`, `#stays`, `#book`, `#faq`.

## House rules

- Never use em dashes in site copy.
- Keep the tone cheeky and warm. No "XL" jokes about turning 40.
- Mark dates as Confirmed or Estimated, and keep the wording honest about which is which.
- Every photo needs a line in `CREDITS` with its Wikimedia Commons file name, author and licence.
- Check both light and dark themes and a phone-width layout before pushing.

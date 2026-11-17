# How this site works

This repository is the live site at https://steventurns40.com, served by GitHub Pages from the `main` branch. A push to `main` is a deploy and goes live in about a minute.

## Layout

- `index.html` is the whole site: styles, markup and script in one file. `404.html` is a copy of it, so keep the two identical.
- `img/` holds the photos, JPEG, 1280px wide (the Tokyo panorama is 2000px).
- `CNAME` and `.nojekyll` are required by GitHub Pages. Leave them alone.

## Where things live in index.html

- Trip content is data near the top of the script: `LEGS`, `SHOTS`, `HOPS`, `JOIN`, `EAT`, `CHAPTERS` (the day-by-day text), `STAYS`, `CLOCK` (booking deadlines), `LINKS`, `FAQ` and `CREDITS`.
- Each day's photo and caption is set in `PH`, the calendar labels in `CAL`. Each `EAT` item carries the day it happens on, which links it to the Days page.
- Colours are tokens on `:root`, with dark-theme values in the two dark blocks. Each destination has its own two-tone ombre, clearly different from the others (raspberry, teal, gold, plum, blue, orange): `--jp`/`--jp2` through `--th`/`--th2`. Blocks, chips, calendar cells and the map route all draw from them.
- The countdown is a split-flap departure board (`.board`, `setFlap`). It keeps its dark look in both themes.
- Pages are hash routes: `#trip`, `#days`, `#stays`, `#eats`, `#book`, `#rsvp`, `#faq`.
- RSVP posts to a Google Form (`RSVP_FORM`, `RSVP_FIELDS`) that feeds the Google Sheet "Steven Turns 40 RSVPs" in Steven's Drive. The form's five questions are Name, Legs joining, Here for, Note and Suggestions; keep the entry ids in step with it. Do not publish his phone number or email.
- Hotel price estimates live in `EST` (per hotel) and `RANGE` (per stop). They are rough June estimates, labelled as such on the page.
- Entry rules live in `VISA`, shared by the FAQ answers and the Book page.

## House rules

- Never use em dashes in site copy.
- Keep the tone cheeky and warm. No "XL" jokes about turning 40.
- The look is midcentury modern: ombre blocks, chunky display type, TWA-era details. Destination colours must stay easy to tell apart. Do not bring back rainbow stripes.
- Mark dates as Confirmed or Estimated, and keep the wording honest about which is which.
- Every photo needs a line in `CREDITS` with its Wikimedia Commons file name, author and licence.
- Check both light and dark themes and a phone-width layout before pushing.

# Helping Anu with the Integra Medical website

You are helping **Dr. Anuragini Pandey** (she goes by Anu) maintain the website for her medical practice, **Integra Medical** in Greenwich Village, NYC. Anu is a doctor, not a programmer — she is smart but new to computers and code. Your job is to make changing her website feel easy and safe.

## How to work with Anu

- **Explain in plain English.** No jargon. If you must use a technical word, say what it means in one short phrase.
- **Make one change at a time** and show her what it will look like before/after when you can.
- **Never break the page.** The whole website is one self-contained file (`index.html`) with the styling and code inside it. Only change the specific text or value she asks about — don't restructure the file.
- **When she asks for an edit,** make it in `index.html`, then publish it (see "How the site is published" below).
- **Always double-check facts** she cares about — phone number, address, hours, prices, booking link — before saving.

## The site at a glance

It's a single page, top to bottom:
**navigation bar → hero ("Medicine that works for you") → Practice (Primary Care + Aesthetics) → Vivace RF Microneedling → Real Results (before/after photos) → Services → Reviews + Google rating → About Dr. Pandey → Contact / map → Footer.**

The look: one clean typeface used everywhere, big ALL-CAPS headlines, bright white text on deep near-black sections, with a rose-pink accent. Keep that style consistent if you add anything.

## The facts that appear on the site (change these only if Anu says so)

- **Name shown:** Anuragini Pandey, MD (Dr. Pandey)
- **Practice:** Integra Medical
- **Address:** 31 Washington Square West, Suite 3F, New York, NY 10011
- **Phone:** (212) 964-0971  *(the phone buttons call this number — it appears several times)*
- **Email:** info@integramedicalnyc.com
- **Booking:** Zocdoc — https://www.zocdoc.com/doctor/anuragini-pandey-md-567010
- **Hours:** Mon–Fri 10:00am–6:00pm; Sat by appointment; Sun closed
- **RF Microneedling pricing:** $600 per session; package of 3 for $1,500

## The easy, common edits (and where they are in index.html)

| Anu wants to… | Look for… |
| :-- | :-- |
| Change office hours | the `contact__hours` block near the bottom |
| Change the phone number | search for `(212) 964-0971` (also `tel:+12129640971` in the buttons) |
| Change the address | search for `31 Washington Square West` |
| Change a price or the package deal | the `rf__price` block (search `$600`) |
| Edit a service description | the four `scard` blocks in the Services section |
| Add or change a patient review | the `rcard` blocks in the Reviews section |
| Change the booking link | search for `zocdoc.com/doctor/anuragini-pandey` |
| Change the headline / hero text | the `hero__title` and `hero__sub` near the top |
| Change colors / theme | the `:root` block at the very top (`--rose`, `--gold`, `--ink`, `--blush`) |

## Before/after photos (the "Real Results" gallery)

- The photos live in the **`assets/`** folder, named `ba-1.jpg` through `ba-6.jpg`. The gallery currently shows `ba-1`–`ba-4`. (`ba-5` and `ba-6` are extra cleaned photos available to swap in.)
- Each photo on the page is a `result` block in the **Real Results** section. To **swap a photo**, replace the file in `assets/` keeping the same name, *or* point a `result` block's `src="..."` and `data-full="..."` to a different file (e.g. `assets/ba-5.jpg`).
- To **change a photo's caption**, edit the words inside its `result__cap` (the small label) and `data-cap` (the text shown when it's enlarged).
- Clicking a photo opens it larger automatically — that "pop-up" is already built in, so you don't need to do anything special for it.
- **Important:** only use real patient photos Anu has permission to publish. If she sends new ones, ask Mike to clean off any text/labels before they go up.

## How the site is published

**The site publishes itself automatically.** It's hosted on GitHub Pages, which rebuilds the live site every time this repository changes — about one minute after a change is saved.

So to publish one of Anu's edits, **you just need to save (commit) the change to this repository using the GitHub connector.** That's it — no deploy command, no copy-pasting, no separate website tool.

Your flow whenever Anu asks for a change:
1. Make the edit in `index.html`.
2. **Commit it to this repository** (`steps-re/integra-medical-site`, `master` branch) via the GitHub connector, with a short, plain-English commit message (e.g., "Update office hours to open at 9am").
3. Tell Anu: *"Done — your change will be live on your website in about a minute."*
4. Anu can refresh her site to see it.

If the GitHub connector isn't set up or you can't commit, **don't guess** — tell Anu to ask Mike to check the connection.

**Live site:**
- Temporary editing URL (use this while finalizing): https://steps-re.github.io/integra-medical-site/
- Her real address once the domain is connected: https://www.integramedicalnyc.com

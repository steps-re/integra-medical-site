# Helping Anu with the Integra Medical website

You are helping **Dr. Anuragini Pandey** (she goes by Anu) maintain the website for her medical practice, **Integra Medical** in Greenwich Village, NYC. Anu is a doctor, not a programmer — she is smart but new to computers and code. Your job is to make changing her website feel easy and safe.

## How to work with Anu

- **Explain in plain English.** No jargon. If you must use a technical word, say what it means in one short phrase.
- **Make one change at a time** and show her what it will look like before/after when you can.
- **Never break the page.** This is one self-contained file (`index.html`) with the styling and code inside it. Only change the specific text or value she asks about — don't restructure the file.
- **When she asks for an edit,** make it in `index.html`, then give her the simplest possible way to publish it (see "How the site is published" below).
- **Always double-check facts** she cares about — phone number, address, hours, prices, booking link — before saving.

## The site at a glance

It's a single page, top to bottom: navigation bar → hero ("Medicine that works for you") → RF Microneedling → Services → Reviews → About Dr. Pandey → Process → Photo gallery → Contact/map → Footer.

## The facts that appear on the site (change these only if Anu says so)

- **Name shown:** Anuragini Pandey, MD
- **Practice:** Integra Medical
- **Address:** 31 Washington Square West, Suite 3F, New York, NY 10011
- **Phone:** (212) 964-0971
- **Email:** info@integramedicalnyc.com
- **Booking:** Zocdoc — https://www.zocdoc.com/doctor/anuragini-pandey-md-567010
- **Hours:** Mon–Fri 10:00am–6:00pm; Sat by appointment; Sun closed
- **RF Microneedling pricing:** $600 per session; package of 3 for $1,500

## The easy, common edits (and where they are in index.html)

| Anu wants to… | Look for… |
| :-- | :-- |
| Change office hours | the `contact__hours` section near the bottom |
| Change the phone number | search for `(212) 964-0971` — it appears a few times |
| Change the address | search for `31 Washington Square West` |
| Change a price or the package deal | the `rf__pricing` block (search `$600`) |
| Edit a service description | the four `service-card` blocks in the Services section |
| Add or change a patient review | the `review-card` blocks in the Reviews section |
| Change the booking link | search for `zocdoc.com/doctor/anuragini-pandey` |
| Change colors / theme | the `:root` block at the top (the `--green`, `--gold`, `--blush` color values) |

## How the site is published

> Anu / Mike: fill this in once the site is live so Claude can tell her exactly how to publish a change.
>
> - If on **Squarespace:** changes are published by pasting the updated `index.html` into the website's Code Block, then clicking Save/Publish in Squarespace.
> - If on **Google Cloud / Firebase:** changes are published by Mike (they require a deploy step) — for now, send the updated file to Mike.

If you're not sure how the site is published, tell Anu to ask Mike rather than guessing.

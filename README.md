# Seating Plan

A wedding seating chart that runs entirely in the browser. Couples set up their room, paste in their guest list, and drag guests onto tables.

**Features**
- Floor plan with round, long or horizontal tables, a head table, and room labels (bar, DJ, dance floor) you can drag around
- Guest sheet with dietary needs and notes, sortable and printable
- "Keep apart" and "keep together" rules, flagged on the plan as soon as they're broken
- Paste guests from a spreadsheet, RSVP export or notes app
- Export a seating list or CSV for the caterer and venue
- Backup files to move a plan between devices or share it with a partner or planner

## Privacy

Plans are saved in the browser's `localStorage`. No guest data is uploaded anywhere. That makes hosting free and simple, but it has two consequences:
- A plan lives on one browser on one device. Moving it, or sharing it with a partner, works through **Export & backup → Download backup / Open a backup**.
- Clearing browser data deletes the plan, so encourage buyers to download a backup now and then.

## Hosting

It's a single static file (`index.html`), so any static host works.

**GitHub Pages:** Settings → Pages → Source: *Deploy from a branch* → pick the branch and `/ (root)` → Save. The site appears at `https://<user>.github.io/wedding-seat-chart/` within a minute or two. Pages is free for public repositories. Private repositories need a paid GitHub plan.

**Netlify Drop (no account setup):** drag the folder containing `index.html` onto <https://app.netlify.com/drop>.

To use your own domain, add it in the host's settings, for example `myseatingplan.com`.

## Running locally

Open `index.html` in a browser, or serve the folder:

```sh
python3 -m http.server 8000
```

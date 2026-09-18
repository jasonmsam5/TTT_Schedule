# TTT Schedule

Room Schedule Manager — a static, single-file HTML app (`index.html`) for managing room bookings. Data is stored in the browser's `localStorage`, so no backend is required.

## Visit frequency (fortnightly / non-weekly clinicians)

Not every clinician comes in each week. Open **Visit Frequency** in the sidebar
(or click the frequency pill on a clinician's badge) to set how often each person
attends: weekly, fortnightly, every 3 weeks, monthly, quarterly, or a custom
number of weeks up to 52.

Anyone who isn't weekly is marked with a pill (`2W`, `4W`, …) and a hatched
overlay on their bookings in the day grid, gym view and week view, and their
frequency is included in the CSV export.

### Per-shift frequency

Frequency can also be set on a single booking, for clinicians who are in weekly
most days but fortnightly or monthly for one shift (and vice versa). Double-click
the booking and change **How often is this shift?** — leave it on *Their usual* to
follow the clinician's frequency, or pick a cadence that applies to that shift
only. Shift-level pills carry a thin outline to distinguish them, and the
frequency editor shows how many shifts a clinician has set individually, with a
**reset** link to put them all back on their usual cadence.

Settings are saved to `localStorage` along with the rest of the schedule.

## Hosting on Netlify

1. Connect this repository to Netlify (New site from Git).
2. Build command: none required.
3. Publish directory: `.` (repo root).

Netlify picks these up automatically from `netlify.toml`. Once deployed, just open the site URL — no further configuration needed.

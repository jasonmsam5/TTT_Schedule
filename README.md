# TTT Schedule

Room Schedule Manager — a static, single-file HTML app (`index.html`) for managing room bookings. Data is stored in the browser's `localStorage`, so no backend is required.

## Visit frequency (fortnightly / non-weekly clinicians)

Not every clinician comes in each week. Open **Visit Frequency** in the sidebar
(or click the frequency pill on a clinician's badge) to set how often each person
attends: weekly, fortnightly, every 3 weeks, monthly, quarterly, or a custom
number of weeks up to 52.

Anyone who isn't weekly is marked with a pill (`2W`, `4W`, …) and a hatched
overlay on their bookings in the day grid, gym view and week view, and their
frequency is included in the CSV export. Settings are saved to `localStorage`
along with the rest of the schedule.

## Hosting on Netlify

1. Connect this repository to Netlify (New site from Git).
2. Build command: none required.
3. Publish directory: `.` (repo root).

Netlify picks these up automatically from `netlify.toml`. Once deployed, just open the site URL — no further configuration needed.

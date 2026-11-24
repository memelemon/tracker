# ARTIST IMPACT TRACKER

> <details>
> <summary>⚠️ ЛИЧНОЕ ИСПОЛЬЗОВАНИЕ</summary>
>
> Этот репозиторий и календарь предназначены исключительно для личного пользования meme_lemon. Это персональный архив творческой активности, а не публичный проект или открытая статистика.
> </details>

Private visual archive for monthly artistic work.

## Files
- `index.html` — responsive calendar dashboard.
- `data.json` — month, category, weekly and report data (source of truth for future updates).

## Current logic
- Calendar highlights report dates.
- A report with a coverage range paints the covered days as a gradual color trail leading to the report date.
- Monthly background and score use the arithmetic mean of four weekly scores. Weeks with no logged report currently count as 0 for the *logged-pace projection*, not as proof that no work happened.
- Category em dash means no data, not zero.
- Week 4 November is provisional because the Nov 24 entry summarizes Nov 1–24 and cannot be reliably split by week.

## Update workflow
Add each new report to `months[].reports`, set its actual date and coverage range, then update the relevant week score/status and category scores. Keep missing category values as `null`. Do not invent daily activity.

## Easter egg
Tap the small moon icon five times.

The repository is private. A private repository does not automatically make a GitHub Pages site privately viewable; hosting/access depends on the GitHub plan and Pages configuration.

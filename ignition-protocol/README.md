# Ignition Protocol Tracking System

Clinical-grade, mobile-friendly Markdown workspace to track the 12-week personal Ignition Protocol (Nov 25, 2024 – Feb 21, 2025). Use this to capture daily inputs in under 2 minutes, roll them into weekly reviews, and surface investor-ready proof points.

## Core assumptions
- Protocol window: **Nov 25, 2024 → Feb 21, 2025 (84 days)**.
- Chronological age: **43**; baseline biological age: **placeholder — update once baseline report available**.
- Role: Founder & Patient Zero; goal is a documentable transformation that validates a systematic peptide protocol.

## How to use this system (minimal friction)
1. **Daily (≤2 minutes):**
   - Open `tracking/daily_checkin_template.md`, duplicate it into `data/daily/YYYY-MM-DD.md`, fill in today’s values.
   - Log doses, sleep, weight, subjective scores, and one observation or win.
2. **Weekly (≈15 minutes):**
   - Open `tracking/weekly_review_template.md`, duplicate to `data/weekly_summaries/week-##.md` (Monday start recommended).
   - Summarize weight trend, averages, adherence, and insights; link photo set if applicable.
   - Update `tracking/current_week.md` with the new week number, dates, and quick metrics.
3. **Protocol reference & adjustments:**
   - Keep `protocol/dosing_schedule.md` and `protocol/titration_log.md` current when doses or frequencies change.
   - Refer to `protocol/stack_overview.md` and `reference/compound_mechanisms.md` to align observations with expected effects.
4. **Periodic labs & scans:**
   - Record labs in `data/bloodwork/bloodwork_log.md` (baseline, mid, final).
   - Capture DEXA details in `data/dexa/dexa_log.md` and summarize shifts in `analysis/baseline_snapshot.md` and `analysis/weekly_trends.md`.
5. **Synthesis for audiences:**
   - Build investor-facing highlights in `outputs/investor_proof_points.md`.
   - Draft the public story in `outputs/case_study_draft.md` and summarize visuals in `outputs/before_after_summary.md`.

## Calculated fields & helpful formulas
- **Protocol Day / Days Remaining:**
  - Day = (`Today` − 2024-11-25) + 1; Remaining = 84 − Day. Add inline in daily logs.
- **% Complete:** `Day / 84 * 100`.
- **Adherence rate:** `Doses taken / Doses scheduled * 100` (log weekly).
- **Weight trend:** Compare first vs last weight of the week; note delta in `weekly_review_template.md`.

## Folder map
- `protocol/` — stack overview, planned dosing, titration history.
- `data/` — raw daily entries, weekly summaries, labs, DEXA, photos (store links or filenames).
- `tracking/` — reusable templates + `current_week.md` for at-a-glance status.
- `analysis/` — baseline snapshot, rolling trends, protocol-level insights.
- `outputs/` — investor proof points, case study draft, before/after summary.
- `reference/` — target ranges, compound mechanism cards, expected timeline.

## Suggested naming conventions
- Daily: `YYYY-MM-DD.md` (e.g., `2024-11-25.md`).
- Weekly: `week-01.md` (Nov 25–Dec 1), `week-02.md`, etc. Note the date range inside the file.
- Photos: `photos/week-##-front.jpg`, `...-side.jpg`, `...-back.jpg` or cloud links.

## Data hygiene
- Keep raw captures in `data/` immutable; reflect corrections in the next day’s note.
- When adjusting doses, update both `protocol/dosing_schedule.md` and `protocol/titration_log.md` the same day.
- Use consistent units: weight (lbs), body fat (%), HRV (ms), sleep (hours + Eight Sleep score), labs (per standard units noted in `reference/target_ranges.md`).

## Rapid weekly workflow
- Pre-fill `tracking/current_week.md` each Monday with the week number and date range.
- During the week, drop quick notes or anomalies there for later synthesis.
- On review day, complete the weekly template, update `analysis/weekly_trends.md` and `analysis/protocol_insights.md`, then refresh `outputs/` files with standout proof points.

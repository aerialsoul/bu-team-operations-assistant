# Changelog

All notable changes to the club-wide files and system instructions.

Format: newest first. Entries marked **ACTION NEEDED** require you to do
something after updating.

---

## [1.1] — 2026-07-22

### Changed

- **Club-wide files now load automatically from GitHub** at session start.
  Managers no longer need a local copy of the `club-files/` folder.
  When club data changes, every manager gets the update on their next
  session — no download, no file replacement.

  **ACTION NEEDED:** Update your system instructions to v1.3 (this release).
  After that, you can delete the `bu-*.md` files from your working folder —
  they are no longer used. Your personal files (profile, config, coach files,
  tracker) are unaffected.

- **Version check now tracks system instructions**, not club files.
  The assistant tells you when a new version of the system instructions
  is available and what changed.

- **Setup simplified.** New managers only need six files in their working
  folder (the personal templates). The `club-files/` copy step is gone.

---

## [1.0] — 2026-07-08

First public release.

### Fixed

- **Age groups corrected to the NorCal 2026/27 Age Group Matrix.**
  NorCal has no U18. U19 is a two-year band spanning birth dates
  08/01/2007–07/31/2009. Age groups are defined by an **August 1 birth-date
  cutoff**, not by subtracting birth year from season year.

  `bu-game-durations.md` previously computed age groups as
  "season year minus birth year," which produced a table shifted a full
  year off — it listed U15 as birth year 2012 where the matrix says U15
  begins 08/01/2011. Every age group below U17 was wrong. The rule and the
  table have both been replaced with published cutoff dates.

  `bu-scheduling-constraints.md` carried a phantom `2008 | U18` row.
  2008-born players are U19.

  **ACTION NEEDED:** If you set up before v1.0, check your
  `manager-config.md` and `coach-*-profile.md` for a U18 label or any
  age group carried over from the old table. Ask the assistant:
  *"Check my team's age group against the current matrix."*

- Removed U23 from the durations table. U19 is the oldest BU age group.

### Changed

- Age group tables now express bands as birth-date ranges rather than
  single birth years, since a calendar birth year can straddle two age
  groups. A player born in 2009 is U17 if born Aug–Dec, U19 if born Jan–Jul.

- Guest player guidance now warns that the absent U18 makes the gap between
  U17 and U19 span two birth years, so a play-up may not be permitted.
  Confirm with your coach before relying on a source team.

### Added

- **Bundle version check.** The assistant now reads the published `VERSION`
  at session start and tells you when your club files are behind.

- **Tier headers.** Every file declares whether it is `CLUB-WIDE`
  (replaced on update), `PERSONAL` (never overwritten), or
  `COPY-ON-FIRST-USE`.

- Note in `bu-season-config.md` and `bu-game-durations.md` that NorCal has
  asked clubs to standardize GotSport team naming, and BU may move from
  birth-year names (`08B Rangers`) to age-group names (`U19 Rangers`).
  Unconfirmed as of 2026-07-08. If your schedule export uses unfamiliar
  team names, confirm the convention before diffing schedules — a rename
  will otherwise look like every team was deleted and replaced.

- `N1L (National 1 League)` added to the GotSport event ID list. New for
  Fall 2026; replaces NPL for some BU teams.

### Renamed

- `coach-[name]-profile.md` → `coach-NAME-profile.md`
- `coach-[name]-schedule.md` → `coach-NAME-schedule.md`

  Square brackets are legal in filenames but GitHub escapes them in URLs
  (`coach-%5Bname%5D-profile.md`), which looks broken when shared. All 28
  references across the bundle were updated to match.

  **ACTION NEEDED:** If you set up before v1.0, your coach files are
  already named after your actual coach (`coach-smith-profile.md`), so
  nothing changes for you. No action required.

### Removed

- Pilot-season narrative from `bu-season-config.md` naming specific
  managers, coaches, and teams. Club-wide files now contain no
  team-specific content.

- Team-specific examples from `bu-game-durations.md` and
  `bu-communication-guidance.md`, replaced with generic placeholders.

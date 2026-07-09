# BU Team Operations Assistant

A Claude project setup that helps Belmont United Soccer Club team managers
and coaches handle scheduling, game day logistics, field coordination, and
communications.

**This is an unofficial community project.** It is maintained by a parent
volunteer and is not an official Belmont United Soccer Club publication.
Nothing here replaces guidance from your club scheduler or club director.

Current bundle version: see [`VERSION`](VERSION). Changes: see
[`CHANGELOG.md`](CHANGELOG.md).

📦 **[Download the latest release](https://github.com/aerialsoul/bu-team-operations-assistant/releases/latest)**
— always download a release, not the main branch.

---

## What this does

Once set up, you can ask the assistant things like:

- "Walk me through Saturday."
- "Does the new schedule create any conflicts for our coach?"
- "Help me draft a reschedule request to the opposing manager."
- "Which BU teams are at Barrett Field on October 4, and who sets up?"
- "What changed in the schedule since last week?"

It knows NorCal game durations, the 2026/27 age group matrix, SAT/ACT
test-day restrictions, BU field access windows, and field setup procedures.

---

## Getting started

New here? Read [`SETUP.md`](SETUP.md). It takes about ten minutes and
assumes no technical background.

Short version: download this bundle, create a Claude project, paste in the
system instructions, upload the files, and say hello. The assistant walks
you through the rest.

---

## How the files are organized

Every file carries a `TIER:` line in its header telling you whether it's
yours to edit. This matters when a new version comes out.

### `club-files/` — CLUB-WIDE

Identical for every BU manager. **Do not edit these locally.** When a new
bundle version is released, you replace them wholesale. If you find an
error, report it (see below) so everyone gets the fix.

| File | What it holds |
|------|---------------|
| `bu-season-config.md` | Season dates, GotSport event IDs, export file types |
| `bu-game-durations.md` | NorCal age groups and game lengths |
| `bu-scheduling-constraints.md` | SAT/ACT dates, referee deadlines, holidays |
| `bu-field-access.md` | When BU has access to each field |
| `bu-field-procedures.md` | Setup, breakdown, and handoff by location |
| `bu-travel-times.md` | Drive times between venues |
| `bu-communication-guidance.md` | Escalation rules and message guidance |

### `templates/` — PERSONAL

Starting points. The assistant fills these in during Setup Mode, and they
become yours. **A bundle update never overwrites them.**

| File | What it holds |
|------|---------------|
| `user-profile.md` | Who you are, your role, your teams |
| `manager-config.md` | Your teams, guest player sources, your constraints |
| `coach-NAME-profile.md` | One per coach — contact info, warmup preference |
| `coach-NAME-schedule.md` | One per coach — their games this season |
| `scheduling-tracker.md` | Reschedule requests and their status |
| `manager-messaging-templates.md` | Your customized message templates |

`manager-messaging-templates.md` is a special case: it ships with BU's
official templates as a starting point, but most managers customize it.
Treat it as yours after first use.

### `system-instructions/`

The prompt that makes Claude behave as the assistant. Paste this into your
Claude project's custom instructions.

---

## Updating

The assistant checks the published version at session start and tells you
if your club files are behind. When that happens:

1. Download the latest release.
2. Replace everything in `club-files/` with the new versions.
3. Leave your personal files alone.
4. Check `CHANGELOG.md` for anything needing your attention.

Because club files are replaced rather than merged, there is nothing to
reconcile — which is exactly why you shouldn't edit them locally.

---

## Found a problem?

Club-wide errors affect every manager. If a travel time is wrong, a field
window has changed, or an age group looks off, please
[open an issue](https://github.com/aerialsoul/bu-team-operations-assistant/issues)
rather than fixing it locally. Your local fix helps one person; a reported
fix helps everyone.

---

## Security note

This repo deliberately contains **no field lock codes, no personal contact
information, and no player data.** Lock codes live on the BU Manager site.
If you find any of the above in this repo, please report it immediately.

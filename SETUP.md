# Setup Guide

For BU team managers and coaches. No technical background needed.
Budget about ten minutes.

---

## Before you start

**You need a paid Claude plan (Pro or Max).** The assistant needs to read
and write files in a project folder on your computer, which requires
Claude's Cowork mode. That comes with Pro and Max, not the free plan.

If you don't have a paid plan, you can still use a read-only version — see
[Option B](#option-b-read-only-no-file-writing) at the bottom. It's less
capable but costs nothing.

---

## Option A: Full setup (Pro or Max)

### 1. Download the bundle

Go to the [latest release](https://github.com/aerialsoul/bu-team-operations-assistant/releases/latest)
and download the **Source code (zip)** file. Don't download from the main
branch — releases are the stable, tested versions.

Unzip it somewhere you'll find again. Your Documents folder is fine.

### 2. Make your working folder

Create a new folder for your team. Something like:

```
BU Team Ops - [Your Team]
```

Copy into it:
- **everything** from `templates/`

That's it. The club-wide files (field info, scheduling constraints, season
config, etc.) load automatically from the web at the start of each session —
you don't need a local copy, and they're always current.

Leave `system-instructions/`, `club-files/`, `README.md`, and `CHANGELOG.md`
in the downloaded bundle. You don't need them in your working folder.

Your working folder should now have six `.md` files.

### 3. Create the Claude project

In the Claude desktop app, create a new project. Name it whatever you like.

When it asks for a folder, point it at the working folder you just made.

### 4. Paste the system instructions

Open `system-instructions/BU-Team-Operations-Assistant.md` from the
downloaded bundle in any text editor. Select all, copy.

In your Claude project, find the custom instructions field and paste it in.
Save.

### 5. Say hello

Open a conversation in the project and type:

> Hi, I'm setting up for the first time.

The assistant will read your files, notice they're blank templates, and walk
you through setup — your name and contact info, your teams, your coaches,
their warmup preferences, your guest player sources, and any constraints for
the season.

It'll ask before writing anything. Answer the questions, confirm at the end,
and you're running.

### 6. Load your schedule

Once setup is done, export your schedule from GotSport and upload the file.
Ask the assistant to load it. From there you can ask about conflicts, plan a
game day, or track a reschedule request.

---

## Keeping it current

**Club-wide data updates automatically.** Field info, scheduling constraints,
season dates — these are fetched from GitHub at the start of every session.
When something changes, you get it the next time you open the assistant.
No download, no file replacement.

**System instructions occasionally need a manual update.** The assistant
checks its own version at session start and tells you if a newer version
is available. When that happens:

1. Go to the [latest release](https://github.com/aerialsoul/bu-team-operations-assistant/releases/latest).
2. Open `system-instructions/BU-Team-Operations-Assistant.md` in any
   text editor. Select all, copy.
3. In your Claude project, paste it into the custom instructions field
   and save.
4. Read `CHANGELOG.md` — anything marked **ACTION NEEDED** needs a look.

Your personal files (profile, config, coach files, tracker) are never
touched by an update.

---

## Option B: Read-only (no file writing)

Without a paid plan you can still upload your personal files to a regular
Claude project as knowledge. Claude will read them and answer questions —
conflict checks, game day walkthroughs, message drafts. Club-wide data
still loads automatically from GitHub.

What you lose: Claude can't update your files. You'll maintain
`scheduling-tracker.md` and your config files by hand, and paste them back
in when they change. Workable for a single team, tedious past that.

---

## Getting help

If something in the club files looks wrong — a travel time, a field window,
an age group —
[open an issue](https://github.com/aerialsoul/bu-team-operations-assistant/issues).
Don't fix it locally.

If the assistant does something strange, that's usually the system
instructions, and also worth an issue.

If you're stuck on soccer rather than software — referee questions, rule
interpretations, disputes with other clubs — the assistant will tell you to
contact club leadership, and it's right. Ask your club scheduler or club
director.

# Belmont United Soccer Club - Game Durations
#
# TIER: CLUB-WIDE — Do not edit locally. Replaced wholesale on bundle update.
# BUNDLE VERSION: 1.0
#
# Source: NorCal League Standards
# Age Groups Source: NorCal 2026/27 Age Group Matrix
#   https://norcalpremier.com/club-development-2/age-group-change-resources/2026-27-age-group-matrix/
# Created By: Shane Rogers
# Last Updated: July 8, 2026
# Note: Game durations are stable NorCal standards and rarely change.
# Age group bands are defined by BIRTH DATE CUTOFF, not calendar birth year.

---

## HOW AGE GROUPS WORK IN NORCAL YOUTH SOCCER

Age groups are defined by **birth date cutoffs**, not by subtracting
birth year from season year. The cutoff is **August 1**.

Two things follow from this that cause most of the confusion:

1. **NorCal has no U18.** U19 is a two-year band spanning
   08/01/2007 – 07/31/2009. There is also no U20 or U23 at BU —
   **U19 is the oldest BU age group.**

2. **A calendar birth year can straddle two age groups.** A player
   born in 2009 is U17 if born Aug–Dec 2009, but U19 if born
   Jan–Jul 2009. Team names use calendar birth year; age groups
   do not. Always check the actual cutoff.

Players move up at the START of each Fall season.

---

## NORCAL AGE GROUPS & GAME DURATIONS - 2026/27

| Age Group | Born On or After | Through | Half Length | Halftime | Total Duration |
|-----------|------------------|---------|-------------|----------|----------------|
| U19 | 08/01/2007 | 07/31/2009 | 45 min | 10 min | 100 min (1hr 40min) |
| U17 | 08/01/2009 | 07/31/2010 | 45 min | 10 min | 100 min (1hr 40min) |
| U16 | 08/01/2010 | 07/31/2011 | 40 min | 10 min | 90 min (1hr 30min) |
| U15 | 08/01/2011 | 07/31/2012 | 40 min | 10 min | 90 min (1hr 30min) |
| U14 | 08/01/2012 | 07/31/2013 | 35 min | 10 min | 80 min (1hr 20min) |
| U13 | 08/01/2013 | 07/31/2014 | 35 min | 10 min | 80 min (1hr 20min) |
| U12 | 08/01/2014 | 07/31/2015 | 35 min | 10 min | 80 min (1hr 20min) |
| U11 | 08/01/2015 | 07/31/2016 | 30 min | 10 min | 70 min (1hr 10min) |
| U10 | 08/01/2016 | 07/31/2017 | 25 min | 10 min | 60 min (1hr) |
| U9 | 08/01/2017 | 07/31/2018 | 25 min | 10 min | 60 min (1hr) |
| U8 | 08/01/2018 | — | 25 min | 10 min | 60 min (1hr) |

Note the U19 band is twice as wide as the others (no U18 exists).

---

## DETERMINING AGE GROUP FROM TEAM NAME

BU team names have historically followed this pattern:
[Birth Year][B/G] [Team Name] — e.g. "08B [Club Name]" = born 2008, Boys team

⚠️ **This convention may be changing.** NorCal has asked clubs to
standardize team naming in GotSport, and BU may move to age-group
naming (e.g. "U19 [Club Name]"). If your GotSport export uses names
that don't match this pattern, stop and confirm the current convention
before relying on name-derived age groups.

Team names are a **starting point, not an authority.** Because the
cutoff is August 1, a team's calendar birth year may map to two
different age groups. Verify against the cutoff table above.

### Quick Reference for 2026/27:
- 08B teams → U19 → 100 min games
- 09B teams → U19 or U17 (straddles the 08/01/2009 cutoff) →
  100 min games either way
- 10B teams → U17 or U16 (straddles 08/01/2010) → 100/90 min
- 11B teams → U16 or U15 (straddles 08/01/2011) → 90 min either way
- 12B teams → U15 or U14 (straddles 08/01/2012) → 90/80 min
- 13B/14B teams → U14/U13 or U13/U12 → 80 min
- 15B/16B teams → U12/U11 or U11/U10 → 80/70/60 min
- 17B/18B teams → U10/U9 or U9/U8 → 60 min

**Combined-year teams** (e.g. a squad rostered as "09B/08B") play at
the age group of their oldest eligible players. A 09B/08B team plays
U19, because its 2008-born players are U19.

Note: Same logic applies to Girls (G) teams.

⚠️ Players born before 08/01/2007 are older than U19 and are not
eligible for any BU age group.

---

## GAME END TIME CALCULATOR

Formula:
**End Time = Start Time + (2 × Half Length) + Halftime**

### Examples Using 2026/27 Age Groups:
- **08B team (U19, 100 min)** starts at 12:00 PM:
  12:00 + 100 min = ends ~1:40 PM

- **15B team (U11, 70 min)** starts at 1:00 PM:
  1:00 + 70 min = ends ~2:10 PM

- **10B team (U16, 90 min)** starts at 12:00 PM:
  12:00 + 90 min = ends ~1:30 PM

- **17B team (U9, 60 min)** starts at 10:30 AM:
  10:30 + 60 min = ends ~11:30 AM

---

## WARMUP TIME

Each coach has a warmup time preference stored in their 
coach-NAME-profile.md. Default if not specified: **45 minutes.**

When calculating travel feasibility between games:
**Required arrival time = Game Start Time - Coach Warmup Preference**

### Example:
Coach prefers 45 min warmup. Next game starts at 2:00 PM.
→ Must arrive at field by 1:15 PM.
Previous game ends at 12:45 PM. Travel time is 20 min.
→ Arrives at ~1:05 PM. ✅ Comfortable (10 min buffer before warmup)

---

## NOTES ON GAME DURATION VARIATIONS

- **Tournament games** may use shorter halves - check tournament 
  schedule for specific format
- **State Cup games** follow standard NorCal durations
- **In-house / scrimmage games** have no standard duration
- **NPL games** follow standard NorCal durations by age group
- If a specific game's duration is unknown, use the standard 
  NorCal duration for that age group as the default assumption

---

## SEASON UPDATE REMINDER

At the start of each Fall season:
1. Pull the new NorCal Age Group Matrix for that seasonal year
2. Replace the cutoff dates in the table above with the published
   values — do NOT compute them by subtracting a year
3. Confirm NorCal still has no U18 (this has been stable, but check)
4. Update the "Last Updated" date at top of this file
5. Verify NorCal hasn't changed any duration standards

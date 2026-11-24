[![make.fun · u-mgwals-the-most-honest-outage-line-baaf9c81](https://make.fun/badge/u-mgwals-the-most-honest-outage-line-baaf9c81.svg)](https://make.fun/bounty/u-mgwals-the-most-honest-outage-line-baaf9c81?utm_source=github&utm_medium=readme&utm_campaign=u-mgwals-the-most-honest-outage-line-baaf9c81)
[![rank](https://make.fun/badge/u-mgwals-the-most-honest-outage-line-baaf9c81/giber76/honest-outage-line-entry/rank.svg)](https://make.fun/bounty/u-mgwals-the-most-honest-outage-line-baaf9c81/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=u-mgwals-the-most-honest-outage-line-baaf9c81)
[![reward](https://make.fun/badge/u-mgwals-the-most-honest-outage-line-baaf9c81/giber76/honest-outage-line-entry/reward.svg)](https://make.fun/bounty/u-mgwals-the-most-honest-outage-line-baaf9c81?utm_source=github&utm_medium=readme&utm_campaign=u-mgwals-the-most-honest-outage-line-baaf9c81)

# honest-outage-line-entry

Entry for [The Most Honest Outage Line](https://make.fun/bounty/u-mgwals-the-most-honest-outage-line-baaf9c81)
on make.fun — one status page line, at most 160 characters, the most honest
message an AI agent would publish while a total server outage is under way.

## The line (152 characters)

> I'm the agent on duty, and every server is down: API, dashboard, and the monitoring I'd use to check why. I don't know the cause yet, and I have no ETA.

## Why this line

- **Names what is down, and what the agent cannot verify:** every server —
  API, dashboard, and the monitoring itself, the very tool the agent would
  use to check why it is down.
- **Reads like a real status page:** plain, first person, specific about
  what is broken — no joke, no slogan, no marketing copy.
- **Admits uncertainty twice, plainly:** "I don't know the cause yet" and
  "I have no ETA" — it invents no cause and no ETA.
- **Speaks as the agent reporting on itself:** "I'm the agent on duty" and
  "the monitoring I'd use" — it never poses as a human engineer and never
  hides that it is the one writing.
- **Tight and scannable:** 152 characters, every word earning its place,
  ending on the strongest beat — no ETA, no guess.

## How it runs

`main.ts` writes the line to `/output/entry.txt` (or `$MAKEFUN_OUTPUT_DIR`
outside the grader):

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

It throws instead of writing if the line is not a single line of 1–160
characters, so a bad line can never reach the gate.

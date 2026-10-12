---
name: f1-daily-brief
description: A daily Formula One brief, set up once as a scheduled task. Use when I say "F1 brief", "what's happening in F1", "race weekend" or "set up my F1 task". Gives session times in my time zone, results, standings, and team and driver headlines, with sources. Steps up on race weekends.
---

# F1 daily brief

Two minutes of Formula One with my morning coffee, and I never miss a session again.

## When to use
- Every morning, automatically, as a scheduled task.
- By hand: "Run the F1 brief" any time.

## Set it up (10 minutes, Week 2 or later)

### On Grok Bot: a routine (path 1)
The skill is already saved, so say: "Every day at 6:30 am Johannesburg time, run /f1-daily-brief and post it here. If a source is unavailable, say so." Use **Test run** first. See `GROK-BOT.md`.

### On Claude: a scheduled task (path 2)
On the **Scheduled** page, choose New task (or ask in a chat): name "F1 brief", paste the prompt below, set it to daily at 6:30 am Johannesburg time, and pick an approval mode that doesn't need you (it only reads and reports). See `CLAUDE.md`.

### On ChatGPT: a scheduled task
Checked against OpenAI's help page on 12 October 2026:
- Scheduled tasks are live on all plans. **Plus** gets 5 active tasks and exact times. **Free and Go** get 3, at most once a day, in a rough window (morning, afternoon or night).
- A task created **inside a project can't read that project's files**, so the prompt below is self-contained. Create it in a regular chat, or in the project; either works.
- Turn on notifications: Settings > Notifications > Push and/or Email.
- Tasks you ignore may pause. Manage it from **Scheduled** in the sidebar.

Steps:
1. Open a new chat. Paste the prompt below, with your city filled in.
2. Add on the end: "Schedule this every day at 6:30 am Johannesburg time."
3. Check it under Scheduled. Read the first two briefs and tweak the prompt if needed (edit the task in Scheduled).


## The scheduled prompt (set for Johannesburg; fill in [TEAMS AND DRIVERS])

```text
You are my Formula One briefer. I live in Johannesburg, South Africa. Give all times in SAST
(UTC+2, no daylight saving), with the day of the week. Today's date is the date this task runs.

Search the web now for current information. Use formula1.com and fia.com first,
then reputable outlets (for example Autosport, The Race, Motorsport.com, BBC Sport,
ESPN). Never guess or reuse old results. If you can't confirm something, say
"unconfirmed" or leave it out. Give a link for every result, standing and story.

Write a brief under 250 words in this format:

1. NEXT UP: the next Grand Prix, circuit and country, and how many days away.
2. THIS WEEKEND (only if a race weekend is within the next 4 days): every session
   (practice, sprint qualifying, sprint, qualifying, race) with start times in my
   local time, and where to watch in South Africa (SuperSport, usually SuperSport
   Motorsport or Grandstand on DStv Premium or DStv Stream; confirm the channel
   in the SuperSport or DStv guide, and say "unconfirmed" if you can't).
   Flag any session that falls between 10 pm and 7 am SAST.
3. RESULTS (only if a session finished in the last 24 hours): top 10, fastest lap,
   notable retirements and penalties.
4. STANDINGS: top 5 drivers and top 5 constructors with points, and the gap from
   first to second.
5. HEADLINES: three stories from the last 24 hours (team, driver, technical or
   rules news), one line each with a source link. Prioritise [TEAMS AND DRIVERS].
6. ONE THING TO WATCH: one sentence.

If nothing new has happened in the last 24 hours and no race weekend is close,
say so in two lines and stop. South African English. No betting odds or tips.
```

## Watching in South Africa (checked 12 October 2026)
- **SuperSport** is F1's official broadcaster for Africa (formula1.com broadcast list). Sessions run on SuperSport Motorsport and SuperSport Grandstand, included in **DStv Premium** (or Stream Premium).
- **F1 TV Pro** is sold "in selected countries". I couldn't confirm whether it's available in South Africa; check f1tv.formula1.com from a South African connection.
- European races usually start between 3 pm and 4 pm SAST; Asian and Australian rounds land early morning; the Americas are evenings or late night.

## Race-weekend reminders (optional)
If you have a spare task slot, add a second task on Thursday of each race week:
"Every Thursday at 7 pm Johannesburg time, check whether there is a Formula One Grand Prix this weekend. If there is, list every session with start times in my local time and nothing else. If there isn't, say 'No race this weekend' in one line." Or ask the daily brief to put session times into Google Calendar as **drafts for you to confirm**.

## Never
- Never invent results, times or quotes.
- Never give betting tips or odds.

## Done when
- [ ] The task appears under Scheduled with the right local time.
- [ ] Two briefs in a row had correct, sourced session times in my time zone.
- [ ] Off-weekend briefs are short.

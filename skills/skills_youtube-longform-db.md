# YouTube Long-Form Content Database — Management Skill

> Load this skill when adding, replacing, or updating videos in the YouTube Long-Form Content database. It contains everything needed to generate on-brand video ideas, populate all fields correctly, and maintain the backlog.

---

## Database Reference

| Item | Value |
|------|-------|
| Database ID | `36e30e58-6a0d-81d4-98d3-e68d37478fc1` |
| Notion Page | https://www.notion.so/36e30e586a0d81d498d3e68d37478fc1 |
| Posting schedule | Tuesday, Thursday, Saturday |
| Target volume | 3 videos per week |

---

## Database Fields

| Field | Type | Notes |
|-------|------|-------|
| Title | Title | Pattern interrupt style — see hook framework below |
| Date | Date | Always Tuesday, Thursday or Saturday |
| Type of Post | Select | See content pillars below |
| Hook | Text | First 1-2 sentences spoken on camera — pattern interrupt only |
| Transcript | Text | Full video script — populated later |
| Thumbnail Idea | Text | Face + emotion + 3-4 word text overlay |
| Description | Text | Skool CTA at top, then keyword-rich human summary of video |
| Framework | Text | Timed outline 0:00–10:00 — see framework template below |
| Status | Select | Idea → Scripted → Recorded → Scheduled → Published |
| Rating | Select | Good / Don't Like — blank by default |

---

## Content Pillars (Type of Post)

| Pillar | Use For |
|--------|---------|
| Argument-Based | Hook into a symptom or frustration → name the cause (fight or flight) → introduce Heart Coherence as the solution |
| Educational | Explain the nervous system, fight or flight, frontal lobe, Heart Coherence — make complex concepts accessible |
| Mission-Based | Olly's personal story, why he does this work, what chronic illness took from him |
| Client Success | Real client stories and transformations — specific, not generic |
| Engagement-Based | Direct questions to the audience — drives comment-to-view ratio |
| Personal | What Olly is up to — builds relatability |

---

## Before Generating Any Video Idea

Always read these files first:
1. `C:\Users\Olly\AI OS\marketing\prospect_intel.md` — real prospect language, objections, and emotional states
2. `C:\Users\Olly\AI OS\marketing\argument_sheet.md` — the core argument that every video must connect to
3. `C:\Users\Olly\AI OS\marketing\CLAUDE.md` — brand voice, audience, banned words, content rules

Every video must connect to at least one of these argument stages:
- Hook into a Pain or Bleeding Neck Pain
- Challenge the Current Belief
- Introduce or reinforce the Actual Cause (fight or flight loop)
- Present the New Mechanism (Heart Coherence)
- Paint the Promised Land

---

## Hook Framework

**Pattern interrupt only — never a promise.**

- ❌ "In this video I am going to show you how to..."
- ✅ Lead with a symptom, frustration, or real prospect quote
- ✅ "Your tests come back normal but you still feel terrible..."
- ✅ "The reason nothing you have tried has lasted is not because those things don't work..."
- ✅ Use a direct client quote as the opener when available

**High-resonance words to use in hooks:**
- "Chronic symptoms" — use in the majority of hooks
- "Mysterious" — validates the experience of being failed by medicine
- "Doctors can't help" — broadest reach hook angle
- "Even when you're resting" — hits the exhaustion avatar specifically
- "The loop" — creates curiosity gap

---

## Video Framework Template (0:00–10:00)

Use this structure for every video. Populate each section with content specific to that video.

```
0:00-0:15 | HOOK
Pattern interrupt opening. Name the symptom, frustration or direct prospect quote.
Never start with "In this video..."

0:15-1:00 | VALIDATE
List specific symptoms by name. Make the right person feel directly spoken to.
Include duration: "you have been living like this for months, maybe years."

1:00-1:45 | REASSURE
"There is nothing insidious going on."
Remove fear before naming the cause. Normalise how they got here.

1:45-3:30 | NAME THE CAUSE
Body stuck in fight or flight as a permanent default.
Make the mechanism feel logical and solvable — not mysterious.

3:30-6:00 | DEEPEN THE LOOP
Show how symptoms create stress, stress creates more symptoms.
Add a real client story or scenario here — this is where retention drops without one.

6:00-7:30 | PERSONAL CREDIBILITY
"I have struggled with this for years."
Brief — not the main event. Bridges from their experience to yours.

7:30-9:00 | TEASE THE SOLUTION
"Something called Heart Coherence" — always this phrasing, every video.
Never assume they know what it is. Handle the objection: "I am not saying you have to meditate for 50 minutes a day."

9:00-10:00 | CTA
Comment HEART below. Link in description.
End with a tease to the next video for session watch time.
```

---

## Description Template

Every description follows this structure — no exceptions:

```
👉 Get your life back from chronic symptoms here: https://www.skool.com/the-healing-code-8609

In this video, [keyword-rich summary of what is covered, written in human conversational tone, 3-5 sentences].
```

---

## Proven Hook Angles (check these before generating new ideas)

| Hook Angle | Why It Works |
|-----------|-------------|
| "Doctors can't help you with these mysterious chronic symptoms" | Speaks to all avatars simultaneously — broadest reach |
| "Your tests come back normal but you still feel terrible" | Names the Avatar 3 bleeding neck pain in one sentence |
| "The loop that keeps your chronic symptoms going" | Creates curiosity gap, implies a solvable mechanism |
| "Nervous system reset for mysterious chronic symptoms" | Solution + problem in five words — complete promise |
| "I just want to enjoy life again — not endure it" | Direct prospect quote — extremely high resonance |
| "You've read the books, done the meditations, still stuck" | Speaks directly to The Researcher avatar |
| "Even when you're resting" | Validates the experience that confuses and shames |

---

## Adding New Videos to the Backlog

**Prompt to use:**
```
Load the dashboard management skill from C:\Users\Olly\AI OS\dashboard-management and the marketing skills from C:\Users\Olly\AI OS\marketing. Generate 10 new YouTube long-form video ideas for my backlog. Read prospect_intel.md and argument_sheet.md first. Each video needs a title, date (Tuesday/Thursday/Saturday continuing from the last date in the database), type of post, hook, description with the Skool CTA at the top, thumbnail idea, framework and status set to Idea. Add them directly to the Notion database ID 36e30e58-6a0d-81d4-98d3-e68d37478fc1.
```

---

## Replacing Videos Marked "Don't Like"

**Prompt to use:**
```
Load the dashboard management skill from C:\Users\Olly\AI OS\dashboard-management and the marketing skills from C:\Users\Olly\AI OS\marketing. Check the YouTube Long-Form Videos database (ID: 36e30e58-6a0d-81d4-98d3-e68d37478fc1) for any videos with Rating set to "Don't Like". For each one, read prospect_intel.md and argument_sheet.md and generate a replacement video keeping the same date. Use the pattern interrupt hook framework and populate title, hook, description with Skool CTA at the top, thumbnail idea, framework and set status back to Idea and rating back to blank. Update the existing Notion page — do not create a new one.
```

---

## Rules

1. Always read `prospect_intel.md` before generating any video idea — never generate from imagination alone
2. Always use "something called Heart Coherence" — never assume the audience knows what it is
3. Never start a hook with "In this video..."
4. Skool CTA always goes at the top of the description
5. Dates always fall on Tuesday, Thursday or Saturday
6. When replacing a video, update the existing page — never create a new one and leave the old one
7. Never use banned words from `CLAUDE.md` (game changer, deep dive, synergy, leverage, hustle, grind, unlock, skyrocket, supercharge)

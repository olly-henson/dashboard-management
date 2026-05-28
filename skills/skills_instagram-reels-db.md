# Instagram Reels Database — Management Skill

> Load this skill when adding, replacing, or updating reels in the Instagram Reels database. It contains everything needed to generate on-brand reel ideas, populate all fields correctly, and maintain the backlog.

---

## Database Reference

| Item | Value |
|------|-------|
| Database ID | `36e30e58-6a0d-81e7-8c2a-e6c4f729915a` |
| Notion Page | https://www.notion.so/36e30e586a0d81e78c2ae6c4f729915a |
| Posting schedule | Mon–Fri (3 reels per day). Saturday optional — move a reel from the Backlog by changing its date. |
| Target backlog volume | 30 reels (2 full weeks) |

---

## Database Fields

| Field | Type | Notes |
|-------|------|-------|
| Title | Title | Internal reference name — not published anywhere |
| Date | Date | Mon–Fri only by default. Saturday/Sunday by exception — change date manually in Backlog view |
| Type of Post | Select | See content pillars below |
| Hook | First 1-2 spoken sentences on camera — pattern interrupt only, never a promise |
| Caption | Text | Full Instagram caption: written text + CTA + hashtags. Ready to copy straight in. |
| Status | Select | Idea → Scripted → Filmed → Edited → Scheduled → Published |
| Rating | Select | Good / Don't Like — blank by default |

---

## Content Pillars (Type of Post)

| Pillar | Use For |
|--------|---------|
| Argument-Based | Hook into a symptom or frustration → name the cause (fight or flight) → tease Heart Coherence as the solution. Primary pillar — majority of reels. |
| Educational | Explain the nervous system, fight or flight, frontal lobe, Heart Coherence. Make complex concepts simple and specific. |
| Mission-Based | Olly's personal story, why he does this work, what chronic illness took from him and what changed. |
| Client Success | Real client stories and transformations — specific details, not generic wins. |
| Engagement-Based | Direct questions to the audience. Goal is high comment-to-view ratio. |
| Personal | What Olly is up to — builds relatability and humanises the account. |

---

## Before Generating Any Reel

Always read these files first:
1. `C:\Users\Olly\AI OS\marketing\prospect_intel.md` — real prospect language, objections, and emotional states
2. `C:\Users\Olly\AI OS\marketing\argument_sheet.md` — the core argument every reel must connect to
3. `C:\Users\Olly\AI OS\marketing\CLAUDE.md` — brand voice, audience, banned words, content rules

Every reel must connect to at least one of these argument stages:
- Hook into a Pain or Bleeding Neck Pain
- Challenge the Current Belief
- Introduce or reinforce the Actual Cause (fight or flight loop)
- Present the New Mechanism (Heart Coherence)
- Paint the Promised Land

---

## Hook Framework

Reels are 15–60 seconds. The first 1.7 seconds determine whether someone keeps watching.

**Pattern interrupt only — never a promise.**

- ❌ "In this video I am going to show you..."
- ✅ Lead with a symptom, frustration, or real prospect quote
- ✅ Name the exact experience — not "chronic illness" broadly but a specific feeling or moment
- ✅ Use prospect language wherever possible — their words outperform any paraphrase

**High-resonance words and phrases:**
- "Chronic symptoms" — use in the majority of hooks
- "Mysterious" — validates being failed by medicine
- "Even when you are resting" — hits the exhaustion avatar directly
- "The loop" — creates curiosity, implies a solvable mechanism
- "Tests come back normal" — names the Avatar 3 bleeding neck pain precisely
- "I just want to enjoy life again — not endure it" — direct prospect quote, extremely high resonance

---

## Reel Structure (15–60 seconds)

```
0–3s   | HOOK
       Pattern interrupt. Name the symptom, frustration or direct prospect quote.

3–10s  | VALIDATE
       Name the specific experience. Make the right person feel directly spoken to.

10–20s | REASSURE (where needed)
       "There is nothing insidious going on." Remove fear before naming the cause.

20–35s | NAME THE CAUSE
       Nervous system stuck in fight or flight. Make it feel logical, not mysterious.

35–45s | TEASE THE SOLUTION
       "Something called Heart Coherence" — always this phrasing, every reel.
       Never assume they know what it is.

45–60s | CTA
       "Comment HEART below." Simple, direct, no pressure.
```

---

## Caption Structure

Every caption follows this structure:

```
[Hook line or opening statement — mirrors the emotional angle of the reel]

[1–2 lines reframing the cause in plain language]

[One line of hope — "the body finally has the chance to heal" style]

➡️ Comment HEART below and I will send you access to my free community where I teach Heart Coherence — a simple daily practice to calm your nervous system and get your life back from chronic symptoms.

👉 Or grab it directly here: https://www.skool.com/the-healing-code-8609

#chronicillness #chronicfatigue #fibromyalgia #invisibleillness #chronicpain #brainfog #dysautonomia #nervoussystemhealing #nervoussystemregulation #heartcoherence #fightorflight #chronicillnessrecovery #healing #backtolife #regulateforrelief
```

---

## Caption Writing Rules

- **No em-dashes or hyphens as clause separators** — they read as AI. Use a full stop instead.
- **Limit hyphens overall** — if a sentence needs one to connect two thoughts, rewrite as two sentences.
- **One idea per paragraph** — short punchy lines read better on mobile.
- **CTA always last** — never mid-caption.
- **Hashtags always at the bottom** — same set on every reel unless specifically requested otherwise.
- **No banned words** — game changer, deep dive, synergy, leverage, hustle, grind, unlock, skyrocket, supercharge. Full list in `CLAUDE.md`.
- **British English** throughout.

---

## Standard Hashtag Set

Use on every reel unless Olly requests a different set:

```
#chronicillness #chronicfatigue #fibromyalgia #invisibleillness #chronicpain #brainfog #dysautonomia #nervoussystemhealing #nervoussystemregulation #heartcoherence #fightorflight #chronicillnessrecovery #healing #backtolife #regulateforrelief
```

---

## Adding New Reels to the Backlog

Run when the backlog is running low (fewer than 2 weeks of content remaining).

**Prompt:**
```
Load the dashboard management skill from C:\Users\Olly\AI OS\dashboard-management and the marketing skills from C:\Users\Olly\AI OS\marketing. Generate 30 new Instagram Reel ideas for the backlog. Read prospect_intel.md and argument_sheet.md first. Each reel needs: title, date (Mon–Fri only, 3 per day, continuing from the last date in the database), type of post, hook, caption (with CTA and hashtags at the bottom), status set to Idea. No hyphens as clause separators in captions — use full stops. Add them directly to Notion database ID 36e30e58-6a0d-81e7-8c2a-e6c4f729915a.
```

---

## Replacing Reels Marked "Don't Like"

Mark any reel as "Don't Like" in the Rating field, then run this prompt:

**Prompt:**
```
Load the dashboard management skill from C:\Users\Olly\AI OS\dashboard-management and the marketing skills from C:\Users\Olly\AI OS\marketing. Check the Instagram Reels database (ID: 36e30e58-6a0d-81e7-8c2a-e6c4f729915a) for any reels with Rating set to "Don't Like". For each one, read prospect_intel.md and argument_sheet.md and generate a replacement reel keeping the same date. Use the pattern interrupt hook framework. Populate title, hook, caption (with CTA and hashtags, no hyphens as clause separators). Set status back to Idea and rating back to blank. Update the existing Notion page — do not create a new one.
```

---

## Notion Views

| View | Filter | Sort |
|------|--------|------|
| This Week | Date is within this week | Date ascending |
| Backlog | None | Date ascending |

**How it works:** The This Week view automatically shows the 15 reels due that week (3 per day, Mon–Fri). On Monday morning, open it and the week's reels are already there. To post on Saturday or Sunday, go to Backlog, pick any reel you like, and change the date — it will appear in This Week automatically.

---

## Rules

1. Always read `prospect_intel.md` before generating any reel — never generate from imagination alone
2. Always use "something called Heart Coherence" — never assume the audience knows what it is
3. Never start a hook with "In this video..." or any promise-style opener
4. No hyphens as clause separators in captions — full stops only
5. Skool CTA always at the bottom of the caption, before hashtags
6. Hashtags always last — same standard set unless otherwise requested
7. Dates always Mon–Fri. Saturday only by exception (Olly moves it manually)
8. When replacing a reel, update the existing page — never create a new one and leave the old one
9. Never use banned words from `CLAUDE.md`
10. British English throughout

# YouTube Community Posts Database — Management Skill

> Load this skill when adding, replacing, or updating posts in the YouTube Community Posts database. It contains everything needed to generate on-brand posts, populate all fields correctly, and maintain the backlog.

---

## Database Reference

| Item | Value |
|------|-------|
| Database ID | `36e30e58-6a0d-81d1-8d13-e38b0136d61e` |
| Notion Page | https://www.notion.so/36e30e586a0d813798d7e134e068d2ca |
| Posting schedule | Every day — 1 post per day |
| Target backlog volume | 14 posts (2 full weeks) |

---

## Database Fields

| Field | Type | Notes |
|-------|------|-------|
| Title | Title | Internal reference name only — not published |
| Date | Date | One per day, every day |
| Type of Post | Select | See post types below |
| Post | Text | Full post copy, ready to paste into YouTube Community |
| Image Idea | Text | Suggested image type to accompany the post |
| Status | Select | Idea → Written → Scheduled → Published |
| Rating | Select | Good / Don't Like — blank by default |

---

## Post Types

| Type | Use For |
|------|---------|
| Personal Story | Olly's own healing journey — before/turning point/after arc. Most common and highest performing. |
| Personal Update | Photo of what Olly is up to — trip, activity, life moment. Short caption. Adds relatability. |
| Engagement | A question or poll for the audience. Drives comments. Short and direct — no preamble. |
| Personal Mission | Why Olly does this work. Connects to his experience and the gap he sees in mainstream medicine. |
| Case Study | A client result — screenshot, interview clip, or written story. Proof-based. Client-focused. |

---

## Before Generating Any Post

Always read these files first:
1. `C:\Users\Olly\AI OS\marketing\prospect_intel.md` — real prospect language, objections and emotional states
2. `C:\Users\Olly\AI OS\marketing\argument_sheet.md` — the core argument every post must connect to
3. `C:\Users\Olly\AI OS\marketing\CLAUDE.md` — brand voice, audience, banned words, tone rules

---

## Personal Story Structure

```
HOOK
One line that pulls the reader in. Bold statement, relatable question, or
"I didn't think it was possible..." style opener.

SETUP
Brief context — what was life like before? 2-4 lines max.

SYMPTOMS / WHAT IT LOOKED LIKE
List using ⏩ arrows. 4-8 items. Lead with the specific symptom the audience
will recognise — exhaustion, pain, brain fog, emotional reactivity.
Never lead with "chronic illness" as the hook — lead with the symptom.

TURNING POINT
What changed. "Things changed when..." / "The day things turned around..."

THE MECHANISM
Heart Coherence — introduce naturally, not as a sales pitch.
Always: "something called Heart Coherence" — never assume they know what it is.

THE RESULT
What life looks like now. Specific and grounded, not vague wellness promises.

CLOSE
CTA, soft sign-off, or engagement question.
```

---

## Format Rules

- **Line length:** One or two sentences per line maximum. Never long paragraphs.
- **White space:** Heavy. Line break every few lines. Scroll-friendly.
- **Ellipsis:** Use ... for pacing and dramatic rhythm in personal story posts. "Back in 2018..." / "But that didn't stop me..."
- **Emoji:** Use where they fit naturally — not as a rule. A single relevant emoji can work at the top of a post if it adds to the feel (e.g. 💚 for a healing story). ⏩ for lists. Never forced. Never mid-post unless it genuinely fits.
- **No hyphens as clause separators.** Use a full stop instead.
- **Sign-off:** "Olly" — no emoji as a rule. Occasionally "Olly 😎" if it fits naturally.
- **Spelling:** British English throughout. Casual and real — "I didn't half arse it either" is fine.
- **Arrow style:** ⏩ — consistent throughout.

---

## CTAs

**Standard CTA (use when no live event is running):**
```
If you'd like to learn how to regulate your nervous system with Heart Coherence so that you can get your life back, check out the link to my free community in the comments below.
```

**Engagement close (for Engagement posts):**
End with the question. No explicit CTA needed — the comments are the mechanism.

**Soft sign-off (for Personal Update or lighter posts):**
```
To your health, happiness and success.
Olly
```

---

## Image Ideas by Post Type

| Post Type | Image Suggestion |
|-----------|-----------------|
| Personal Story (low point) | Candid, raw, unposed personal photo from a difficult period |
| Personal Story (turning point) | Aspirational outdoor photo — walking, nature, activity |
| Personal Story (result) | Joyful moment — concert, social occasion, family, wedding |
| Personal Update | Whatever the update is — trip, activity, milestone |
| Engagement | Warm selfie, direct eye contact, looks like a genuine question |
| Personal Mission | Certification photo, professional moment, or calm selfie |
| Case Study | Client quote card, screenshot (with permission), or result graphic |

**General pool to draw from:** selfies, aspirational photos, beautiful scenery, life milestones, family photos, client results quotes or images.

---

## Real Post Example (use as tone and format reference)

```
How Heart Coherence Gave Me My Life Back 💚

Back in 2018...

My life got considerably worse.

After a series of pretty serious head injuries, I lost everything:

⏩ Business
⏩ Long-term relationship
⏩ Social life
⏩ Ability to drive

It was bad.

I spent a small fortune and a lot of my time trying to get help...

But nothing moved the needle.

[continues in this style — short lines, ellipsis pacing, honest tone]
```

**Why this works:**
- One emoji at the top that fits the content (💚 for healing)
- Short lines throughout — every sentence breathes
- Ellipsis creates rhythm and pace
- Honest and casual — "I didn't half arse it either"
- No hyphens as clause separators
- No corporate wellness language

---

## Adding New Posts to the Backlog

Run when the backlog is running low (fewer than 2 weeks of content remaining).

**Prompt:**
```
Load the dashboard management skill from C:\Users\Olly\AI OS\dashboard-management\skills\skills_youtube-community-db.md and the marketing skills from C:\Users\Olly\AI OS\marketing. Generate 14 new YouTube Community posts for the backlog. Read prospect_intel.md and argument_sheet.md first. Each post needs: title, date (one per day continuing from the last date in the database), type of post, full post copy (short lines, white space, ellipsis pacing, no hyphens as clause separators, British English, use emojis where they fit naturally), image idea, status set to Idea. Add them directly to Notion database ID 36e30e58-6a0d-81d1-8d13-e38b0136d61e.
```

---

## Replacing Posts Marked "Don't Like"

Mark any post as "Don't Like" in the Rating field, then run this prompt:

**Prompt:**
```
Load the dashboard management skill from C:\Users\Olly\AI OS\dashboard-management\skills\skills_youtube-community-db.md and the marketing skills from C:\Users\Olly\AI OS\marketing. Check the YouTube Community Posts database (ID: 36e30e58-6a0d-81d1-8d13-e38b0136d61e) for any posts with Rating set to "Don't Like". For each one, read prospect_intel.md and argument_sheet.md and generate a replacement post keeping the same date and post type. Use short lines, white space, ellipsis pacing, no hyphens as clause separators, British English, emojis where they fit naturally. Set status back to Idea and rating back to blank. Update the existing Notion page — do not create a new one.
```

---

## Notion Views

| View | Filter | Sort |
|------|--------|------|
| This Week | Date is within this week | Date ascending |
| Backlog | None | Date ascending |

Week starts Monday — update this in Notion settings if needed.

---

## Rules

1. Always read `prospect_intel.md` before generating any post
2. Always use "something called Heart Coherence" — never assume the audience knows what it is
3. No hyphens as clause separators — full stops only
4. Short lines and heavy white space throughout — this is not a paragraph-format platform
5. Use ellipsis (...) for pacing in personal story posts
6. Emojis where they fit naturally — not as a rule
7. No 😎 on every post — only when it genuinely fits
8. British English throughout — casual and real is fine
9. CTA always links to the free community in the comments — not bio
10. When replacing a post, update the existing page — never create a new one
11. Never use banned words from `CLAUDE.md`

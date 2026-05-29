# Email Campaigns Database — Management Skill

> Load this skill when adding, rewriting, or updating emails in the Email Campaigns database. It contains everything needed to write on-brand emails, populate all fields correctly, and maintain the sequence queue.

---

## Database Reference

| Item | Value |
|------|-------|
| Database ID | `36e30e58-6a0d-811c-b455-ce8fe3da15be` |
| Notion Page | https://www.notion.so/36e30e586a0d811cb455ce8fe3da15be |
| Platform | GoHighLevel |
| Active sequence | Back to Life |
| Contact tag | Back to Life Prospect |
| Frequency | Every other day |
| Target queue volume | 3+ emails ahead of the last Live email |

---

## Database Fields

| Field | Type | Notes |
|-------|------|-------|
| Subject | Title | The email subject line — published to prospects |
| Number | Number | Position in the sequence — 1, 2, 3 etc. |
| Send Day | Number | Which day in the sequence the email sends — Day 1, 3, 5, 7 etc. (every other day) |
| Type | Select | See email types below |
| Sequence | Select | Back to Life (expandable for future sequences) |
| Status | Select | Draft → Ready → Scheduled → Live |
| Copy | Text | Full email body — ready to paste into GoHighLevel |
| Notes | Text | Internal notes — context, avatar, what the email is trying to do |

---

## Status Definitions

| Status | Meaning |
|--------|---------|
| Draft | Being written or needs rewriting |
| Ready | Written, reviewed, ready to copy into GHL |
| Scheduled | Added to the GHL workflow |
| Live | Active and sending in the sequence |

---

## Email Types

| Type | Purpose | Frequency |
|------|---------|-----------|
| Welcome | First email — sets expectations, warm introduction | Email 1 only |
| Belief Shift | Challenge why they're stuck — introduce the actual cause | Most common |
| Personal Story | Olly's own experience — builds trust, makes the solution real | Every 4–5 emails |
| Empathy | Pure emotional validation — no solution, no CTA | Every 5–6 emails |
| Objection Handling | Address the most common reasons they haven't acted | As needed |
| Education | Explain the nervous system, fight or flight, Heart Coherence | Regular |
| Framework | Simple numbered structure — makes recovery feel achievable | Occasional |
| Client Proof | Mini-wins and results from clients — add as proof comes in | As available |
| Mission | Why Olly does this work — connection and authority without bragging | Every 8–10 emails |

---

## Before Writing Any Email

Always read these files first:
1. `C:\Users\Olly\AI OS\marketing\argument_sheet.md` — every email must connect to at least one stage of the argument
2. `C:\Users\Olly\AI OS\marketing\prospect_avatars.md` — write for one primary avatar
3. `C:\Users\Olly\AI OS\marketing\prospect_intel.md` — real prospect language and objections to weave in
4. `C:\Users\Olly\AI OS\marketing\CLAUDE.md` — brand voice, banned words, tone rules

---

## Voice and Structure Rules

- **Short lines.** Single sentences as their own paragraph. Creates pace and pulls the reader down.
- **150–300 words** — every line earns its place. Max 400 for personal story or framework emails.
- **Ellipsis (...)** used deliberately to create forward momentum. Not overused.
- **Plain language.** No clinical terms, no wellness jargon, no corporate language.
- **British English** throughout.
- **First person, conversational** — sounds like a message from someone who has been through it.
- **Never preachy.** Never "you deserve this."
- **Always use `{{contact.first_name}}`** for the first name merge tag — never "Hey there" or a placeholder.
- **Reframe blame before offering solution** — "it's not a willpower issue" removes self-blame and opens the prospect to the real cause.
- **Manage expectations honestly** — "it will take learning and consistent practice" builds credibility.
- **Specific losses outperform vague statements** — name the wedding, the birthday, the sport.
- **Never run the same email type twice in a row.**

### Subject Lines
- Mirror the first line or emotional hook of the email
- 5–9 words, plain language, no false urgency
- Examples: *"I know it's hard and lonely"* / *"It's not a willpower problem"* / *"I went all in — here's what happened"*

---

## CTA Options

| CTA Type | When to Use |
|----------|------------|
| Training/VSL link | Belief shift, education, story emails where prospect is ready to find out more |
| Open loop | When the concept needs to land and sit — no ask, let it breathe |
| Reply invite | Empathy and connection emails — "Drop me a reply if you'd like to know more" |
| No CTA | Pure empathy and personal story emails — end on a personal commitment |

CTA tone: always soft and conversational — never urgent, never "click here" or "sign up now."

---

## Proven Phrases — Use When They Fit

- "I just want to enjoy life again and not endure it"
- "I know the old happy me is still inside me somewhere"
- "This is robbing me of my life on a day to day basis"
- "A chicken and an egg relentless loop"
- "I cannot make it work for me"
- "Even when you're resting"
- "Constantly being knocked back"
- "Your heart and life gradually come back online"
- "A surviving and on-edge robot"
- "Something called Heart Coherence" — always use this framing when introducing it
- "I went all in" — personal conviction language
- "Just hanging on" — describes the daily reality of survival mode

---

## Adding New Emails to the Sequence

Run when the queue has fewer than 3 Ready emails ahead.

**Prompt:**
```
Load the dashboard management skill from C:\Users\Olly\AI OS\dashboard-management\skills\skills_email-campaigns-db.md and the marketing skills from C:\Users\Olly\AI OS\marketing. Generate 3 new emails for the Back to Life sequence. Read prospect_intel.md, argument_sheet.md and prospect_avatars.md first. Each email needs: subject line, number (next in sequence), send day (continuing every other day from the last), type, sequence set to Back to Life, full email copy (150–300 words, short lines, British English, {{contact.first_name}} for first name), status set to Ready. Add them directly to Notion database ID 36e30e58-6a0d-811c-b455-ce8fe3da15be.
```

---

## Replacing a "Don't Like" Email

Mark any email as "Don't Like" in the Rating field, then run this prompt:

**Prompt:**
```
Load the dashboard management skill from C:\Users\Olly\AI OS\dashboard-management\skills\skills_email-campaigns-db.md and the marketing skills from C:\Users\Olly\AI OS\marketing. Check the Email Campaigns database (ID: 36e30e58-6a0d-811c-b455-ce8fe3da15be) for any emails with Rating set to "Don't Like". For each one, read prospect_intel.md, argument_sheet.md and prospect_avatars.md and generate a replacement email keeping the exact same Number, Send Day and Type. Follow all voice and structure rules: 150–300 words, short lines, British English, {{contact.first_name}} for first name. Set Status back to Ready and Rating back to blank. Update the existing Notion page — do not create a new one.
```

---

## Rewriting a Draft Email

**Prompt:**
```
Load the dashboard management skill from C:\Users\Olly\AI OS\dashboard-management\skills\skills_email-campaigns-db.md and the marketing skills from C:\Users\Olly\AI OS\marketing. Check the Email Campaigns database (ID: 36e30e58-6a0d-811c-b455-ce8fe3da15be) for any emails with Status set to Draft that need rewriting. Read prospect_intel.md, argument_sheet.md and prospect_avatars.md. Rewrite the email following all voice and structure rules. Update the existing Notion page — do not create a new one. Set Status to Ready when done.
```

---

## Notion Views

| View | Filter | Sort |
|------|--------|------|
| Queue | Status is not Live | Number ascending |
| Live | Status is Live | Number ascending |
| All | None | Number ascending |

---

## Rules

1. Always read `argument_sheet.md`, `prospect_avatars.md` and `prospect_intel.md` before writing
2. Always use `{{contact.first_name}}` — never a placeholder or "Hey there"
3. 150–300 words per email — every line earns its place
4. Short lines throughout — single sentence paragraphs
5. British English throughout
6. Never run the same type twice in a row
7. No CTA on empathy emails — end on warmth and personal commitment
8. Always use "something called Heart Coherence" when introducing it — never assume they know what it is
9. When rewriting, update the existing page — never create a new one
10. Never fabricate client results — only use real proof as it comes in
11. Never use banned words from `CLAUDE.md`
12. Set Status to Ready only when the email is fully written and quality-checked

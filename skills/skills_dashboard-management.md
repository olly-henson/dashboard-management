# Dashboard Management — Weekly Business Review

> This skill gives Claude complete context to run, troubleshoot, and maintain Olly's Notion Business Dashboard every Monday at 9am. Load this file when Olly asks you to run the dashboard script or make any adjustments to the dashboard.

---

## What This Skill Covers

- Running the weekly metrics script
- Interpreting the output and flagging anything that needs attention
- Troubleshooting common script failures
- Making adjustments to the dashboard or databases

---

## The Weekly Script

**Command to run:**
```
node "C:\Users\Olly\AI OS\marketing\fetch_metrics.mjs"
```

**Location:** `C:\Users\Olly\AI OS\marketing\fetch_metrics.mjs`

**When:** Every Monday at 9am SAST — calendar event "🚨 Weekly Business Dashboard Review — Olly Henson Coaching" is set up in Google Calendar (recurring, every Monday).

---

## What the Script Does

### Auto-populated (no action needed from Olly)
| Metric | Source |
|--------|--------|
| Email Subscribers | GHL — contacts tagged "back to life prospect" |
| Customers | GHL — contacts tagged "back to life customers" |
| Skool Members | Calculated: Email Subscribers + Customers |
| YouTube Subscribers | YouTube Data API |
| YouTube New Subscribers | YouTube Analytics API |
| YouTube Views, Watch Time, Audience Retention | YouTube Analytics API |
| YouTube Videos Published This Month | YouTube Data API |
| YouTube Top Video | YouTube Analytics API |
| Website Visits (last 30 days) | Google Analytics 4 (GA4) |
| Avg % Improvement | Google Sheets — Summary Dashboard tab, column E (rows 4–12), averaged across all 9 metrics. Only populates once a client completes the full 6-week Regulate for Relief programme. |
| All growth % figures | Calculated from previous month's row in each sub-database |

### Manual entries (Olly does these after running the script)
| Metric | Where to find it |
|--------|-----------------|
| YouTube CTR (%) | YouTube Studio → Analytics → Content tab → Impressions CTR |
| Instagram — all metrics | Instagram app → Profile → Professional Dashboard → Account Insights → last 7 days. Record: Accounts Reached, Profile Visits, Link Clicks, Followers, New Followers. Top post: Content You Shared → sort by Reach. |
| Revenue & Expenses | End of month only — enter in Notion → Business Dashboard → Finances |
| Avg % Improvement | Auto from script once clients complete programme — otherwise enter manually from Google Sheets Summary Dashboard |

---

## Notion Business Dashboard

**URL:** https://www.notion.so/Business-Dashboard-36e30e586a0d81c88c70dfa1fc988004

### Summary Callout Blocks (top of dashboard)
These are auto-updated by the script on every run.

| Block | Notion Block ID | Notes |
|-------|----------------|-------|
| 📊 Marketing | `36e30e58-6a0d-81a5-be52-efb489ccc899` | Shows YouTube, Instagram, Email, Skool, Website growth |
| 🚀 Delivery | `36e30e58-6a0d-81f9-9823-c019527b2ac4` | Links to Customer Satisfaction DB |
| 💵 Sales | `36e30e58-6a0d-81af-b991-dc61d4f12e95` | Links to Sales Growth DB |
| 📋 Financial Management | `36e30e58-6a0d-817f-8b54-db801a31fb3e` | Links to Finances DB — shows only "Finances", NOT Expenses/Profit separately |

### Sub-databases (each is a child page of the dashboard)
| Page | Database ID | Key columns |
|------|-------------|-------------|
| YouTube | `36e30e58-6a0d-814f-939e-c49fab4e411f` | Subscribers, Views, Watch Time, CTR, Retention, Top Video, growth % |
| Instagram | `36e30e58-6a0d-81d9-a0d5-f5a2a944845d` | Followers, Reached, Views, Interactions, Best Reel, growth % |
| Email Subscribers | `36e30e58-6a0d-8106-a888-e0caa729eb12` | Total Subscribers, growth % |
| Skool Members | `36e30e58-6a0d-8116-817a-ee4a94d0f3ba` | Total Members, growth % |
| Customers (Sales Growth) | `36e30e58-6a0d-817e-ad03-fb879a1323d8` | New Customers, New Skool Members, Conversion Rate, growth % |
| Website | `36e30e58-6a0d-81d2-8d43-e1c4f2da396f` | Total Visits, growth % |
| Customer Satisfaction | `36e30e58-6a0d-81b2-9f0c-fb3ba412015d` | Avg % Improvement, Active Clients, Notes |
| Finances | `36e30e58-6a0d-81e2-817b-fceff7538eef` | Month, Revenue ($), MRR ($), Expenses ($), Profit (formula: MRR − Expenses) |

### Main Business Metrics Database
**ID:** `36e30e58-6a0d-8187-ac85-d3b16d11e297`
Stores the top-level monthly snapshot: all key numbers in one row per month.

---

## API Connections

| Service | Credential key in .env | Status |
|---------|----------------------|--------|
| Notion | `NOTION_API_TOKEN` | ✅ Connected |
| GoHighLevel | `GHL_PIT_TOKEN`, `GHL_LOCATION_ID` | ✅ Connected |
| YouTube Data API | `YOUTUBE_API_KEY`, `YOUTUBE_CHANNEL_ID` | ✅ Connected |
| YouTube Analytics API | `GA_CLIENT_ID`, `GA_CLIENT_SECRET`, `GA_REFRESH_TOKEN` | ✅ Connected (shared OAuth with GA) |
| Google Analytics 4 | `GA_CLIENT_ID`, `GA_CLIENT_SECRET`, `GA_REFRESH_TOKEN`, `GA_PROPERTY_ID` | ✅ Connected |
| Google Sheets (Regulate tracker) | `REGULATE_SHEET_ID` | ✅ Connected |
| Google Calendar | `GOOGLE_CLIENT_ID`, `GOOGLE_CLIENT_SECRET` | ✅ Connected |
| Instagram | `IG_ACCESS_TOKEN` | ⏳ Not yet connected — Instagram data is entered manually |

**Note:** All credentials are stored in `C:\Users\Olly\AI OS\marketing\.env` — never hardcode them in scripts.

---

## Interpreting the Output — What to Flag

After running the script, review each metric against the previous week/month and flag anything that needs attention:

### YouTube
| Signal | What it means | Suggested action |
|--------|--------------|-----------------|
| CTR (%) dropping | Thumbnails or titles not compelling enough | Review top-performing titles; test new thumbnail styles |
| Views dropping | Content not resonating or posting frequency dropped | Check posting schedule; review hook quality |
| Watch Time / Retention dropping | Viewers dropping off early | Review video structure; hook and first 30 seconds |
| Subscribers stalled | Growth plateauing | Analyse top video and replicate angle |

### Instagram
| Signal | What it means | Suggested action |
|--------|--------------|-----------------|
| Accounts Reached dropping | Reels not being pushed by algorithm | Review hooks; check if posting consistently |
| Followers not converting from Reach | Content not compelling enough to follow | Stronger CTA; check profile bio |
| Profile Visits not converting to followers | Bio/profile not doing its job | Review profile, bio and pinned posts |

### Email / Skool
| Signal | What it means | Suggested action |
|--------|--------------|-----------------|
| Email Subscribers not growing | Not enough leads entering the funnel | Review top-of-funnel content; check CTA is HEART |
| Skool Members stalled | Free community not growing | Check Skool CTA in content and email |

### Sales / Customers
| Signal | What it means | Suggested action |
|--------|--------------|-----------------|
| Customers not growing | Conversion from community to paid not working | Review DM follow-up process; check application flow |

### Website
| Signal | What it means | Suggested action |
|--------|--------------|-----------------|
| Visits very low | Little organic search traffic yet | Note: site is early stage; expected for now |

---

## Known Issues & Fixes

### Notion integration permissions
Each sub-database page must have the **Marketing OS** integration connected, otherwise the script gets a 404. If a database returns "not found":
- Go to that page in Notion → ⋯ → Connections → Connect to → Marketing OS

### Script writes to wrong database
If the main Business Metrics database is ever deleted and recreated, update `DB_ID` on line ~28 of `fetch_metrics.mjs` with the new database ID.

### YouTube Growth showing "—"
Caused by missing previous month row in the YouTube sub-database. Will resolve automatically once two months of data exist. Can also be caused by YouTube Analytics API errors (check Google Cloud Console — if error rate is high, may be a quota or OAuth scope issue).

### Financial Management callout reverting
The script updates the Financial Management callout on every run. It must show only **📈 Finances** (not Expenses/Profit separately). If it reverts, check the `snapshotUpdates` array in `fetch_metrics.mjs` around line ~725.

### Customer Satisfaction link pointing to wrong page
Must link to the Customer Satisfaction database block ID `36e30e586a0d81b29f0cfb3ba412015d` — NOT to `NOTION_CUSTOMERS_DB_ID` which points to the Sales Growth database.

---

## Making Adjustments

When Olly asks to change the dashboard:
1. Always check current block/database state via Notion API before editing
2. Use the block IDs above to target the right elements
3. Remember the Notion API cannot change a block's type — delete and recreate if needed
4. After any script changes, run it once to confirm output is clean
5. Never hardcode API keys — always read from `.env`

---

## Files Reference

| File | Purpose |
|------|---------|
| `fetch_metrics.mjs` | Main weekly script — pulls all data and updates Notion |
| `create_dashboard_db.mjs` | One-time script — creates Business Metrics database |
| `setup_dashboard.mjs` | One-time script — builds dashboard page layout |
| `add_calendar_reminder.mjs` | One-time script — created the Google Calendar recurring event |
| `.env` | All credentials — never commit to GitHub |

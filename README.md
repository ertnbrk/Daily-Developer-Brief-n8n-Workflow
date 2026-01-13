# Daily Developer Brief

Daily Developer Brief is a production-grade automation pipeline built with **n8n** that aggregates, filters, ranks, and delivers **high-signal developer news** from multiple sources into a concise daily briefing.

The system is designed to eliminate noise (finance, crypto, irrelevant trends) and surface only content that matters to developers, DevOps engineers, and platform teams.

---

<img width="1162" height="494" alt="workflow" src="https://github.com/user-attachments/assets/d583e94e-b27e-4bd1-b192-4e12f866c505" />


---

## ✨ What This Project Does

- Aggregates developer-relevant content from:
  - Google News
  - Reddit (curated subreddits)
- Applies **keyword-based ingestion**
- Filters out low-signal and irrelevant topics (finance, crypto, jobs, ads)
- Deduplicates content using hashing
- Scores and ranks content by relevance
- Categorizes content into:
  - Breaking / Security
  - Developer Discussions
  - Releases & Updates
- Archives selected items into **Notion**
- Generates a **HTML-safe email digest** optimized for email clients
- Runs automatically on a scheduled basis (daily)

---

## 🧠 Why This Exists

Following tech news is noisy and time-consuming.  
Daily Developer Brief solves this by:

- Reducing dozens of articles to **8–10 minutes of curated reading**
- Focusing strictly on **engineering-relevant signals**
- Automating the entire pipeline end-to-end
- Delivering results in a format suitable for daily consumption

This project also serves as a **DevOps / Automation portfolio showcase**, demonstrating real-world workflow design, data filtering, and delivery automation.

---

## ⚙️ Workflow Highlights

### Content Filtering
- Excludes:
  - Crypto & finance news
  - Job listings and career posts
  - Marketing content
- Includes:
  - Software engineering
  - DevOps / Cloud
  - Open source releases
  - Security advisories
  - Developer community discussions

### Scoring Logic (Simplified)
- Reddit posts weighted by engagement (upvotes)
- News articles weighted by relevance
- Final output limited to top ranked items

---

## 📨 Email Digest

- Email-client safe HTML
- Card-based layout
- Magazine-style grid (no infinite scroll)
- Optimized for Gmail, Outlook, Apple Mail
- Designed for **quick daily reading**

---

## 🗂️ Notion Archive

- Stores selected daily content
- Enables long-term tracking
- Can be extended with:
  - Read/unread status
  - Personal notes
  - Tags and priorities

---

## 🚀 How to Use

1. Import the workflow JSON into n8n
2. Configure environment variables:
   - Apify API token
   - Notion API token
   - Email credentials
3. Adjust keyword and subreddit lists in the global config
4. Enable the schedule trigger
5. Receive your daily developer brief automatically

---

## 🎯 Use Cases

- Daily developer news monitoring
- DevOps / Platform engineering awareness
- Security & release tracking
- Personal knowledge curation
- Automation & workflow portfolio project

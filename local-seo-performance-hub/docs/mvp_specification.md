# MVP Specification – Local SEO Performance Hub

## 1. Objective
Deliver a working SaaS MVP that provides **local businesses** with a single **Visibility Score (0–100)** derived from rankings, reviews, and citations.  
Goal: Validate willingness to pay and collect feedback from early adopters (dentists, lawyers, plumbers, etc.).

---

## 2. Core Features (MVP Only)

### 2.1 Business Input Form
- Fields: Business name, zip code, website URL.
- Trigger: Generates a Visibility Score.

### 2.2 Local Rank Tracking
- Use SERP API (SERPWow / DataForSEO).
- Track up to **10 keywords** for one location.
- Show results in list + simple heatmap grid.

### 2.3 Review Monitoring (Google only at MVP stage)
- Connect Google Business Profile API.
- Pull star rating, review count, latest 5 reviews.
- Display in dashboard.

### 2.4 Citation Check (Top 5 Directories)
- Scrape or API check for:
  - **Germany**: Gelbe Seiten, Das Örtliche, Jameda, Yelp, Facebook.
  - **International**: Yelp, YellowPages, Angi, Facebook, TripAdvisor.
- Show % completion of listings.

### 2.5 Visibility Score Calculation
- Formula (simple weighting at MVP stage):
  - Rankings = 40%
  - Reviews = 40%
  - Citations = 20%
- Output: Single number + “Competitor Benchmark” (use public competitors in same zip).

### 2.6 Dashboard + Weekly Email Report
- Dashboard view: score + 3 modules (Rankings, Reviews, Citations).
- Weekly automated PDF/email report (basic template, no white-label yet).

---

## 3. Technical Setup

### 3.1 Frontend
- Option A: Low-code (Bubble / Retool).
- Option B: React + Tailwind (scalable).

### 3.2 Backend
- Node.js + Express API layer.
- PostgreSQL for business + keyword + review storage.

### 3.3 Integrations
- SERPWow / DataForSEO (keyword ranking).
- Google My Business API (reviews).
- Simple scraper/API for citations.

### 3.4 Hosting
- Vercel (frontend).
- Heroku / AWS RDS (backend + DB).
- EU data center (Frankfurt) → GDPR compliance.

### 3.5 Reporting
- jsPDF or Puppeteer to auto-generate PDF from dashboard.
- SendGrid for email delivery.

---

## 4. User Journey (Happy Path)

1. User signs up → Enters business name, zip code, keywords.
2. System pulls data (rankings, reviews, citations).
3. Dashboard shows:
   - Visibility Score = 64/100
   - Rank overview: 3 keywords top-10, 7 keywords >20
   - Reviews: 4.3 stars (82 total), last 3 reviews listed
   - Citations: 3/5 found, 60% complete
4. Weekly → Email report with updated score.

---

## 5. Success Criteria
- MVP live within 6–8 weeks.
- At least **10 paying beta users** (€49–97/month).
- Average onboarding time <10 minutes per business.
- Feedback loop: Users confirm Visibility Score is clear & valuable.

---

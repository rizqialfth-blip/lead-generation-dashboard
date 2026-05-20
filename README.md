# 📊 Lead Generation Dashboard: Internal Tool Case Study

An internal AI-powered lead generation and scoring dashboard built in 8 hours using Lovable + Firebase, designed to automate prospect qualification for sales teams.

## 🔧 Project Overview
- **Role:** AI Internal Tool Builder / Data Pipeline Engineer
- **Stack:** Lovable (UI Generation) + Firebase (Real-time Database)
- **Build Time:** 8 Hours (Vibe Coding Sprint)
- **Objective:** Replace manual spreadsheet tracking with an automated, real-time lead scoring dashboard.

---

## ⚙️ Core Features Built

### 1. Automated Lead Scoring Engine
Each incoming lead is automatically scored 0–100 based on:
- **Industry match** (weighted: 40%)
- **Company size** (weighted: 30%)
- **Engagement signals** (weighted: 30%)

```json
{
  "lead_id": "LEAD-2026-001",
  "company": "TechCorp Indonesia",
  "score": 87,
  "tier": "Hot",
  "signals": {
    "industry_match": true,
    "company_size": "51-200",
    "engagement": "Visited pricing page 3x"
  }
}
```

### 2. Real-Time Firebase Pipeline
- Leads flow from form submissions → Firebase Firestore → Dashboard in **< 500ms**
- Firestore security rules enforced for role-based access (Admin / Sales Rep)

### 3. Data Annotation Layer
All leads are tagged with structured metadata to train future ML scoring models:
- `[Source: Organic / Paid / Referral]`
- `[Intent: High / Medium / Low]`
- `[Verified: true/false]`

---

## 📈 Impact Metrics
- **85% reduction** in manual lead qualification time
- **Real-time visibility** across 3 sales pipeline stages
- Built and deployed in a single 8-hour sprint

---

## 🛠️ Tech Stack
| Layer | Tool |
|-------|------|
| UI Generation | Lovable |
| Database | Firebase Firestore |
| Auth | Firebase Auth |
| Hosting | Firebase Hosting |

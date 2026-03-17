# 🛡️ RideCover — AI-Powered Parametric Insurance for Q-Commerce Delivery Workers

> **Guidewire DEVTrails 2026 | University Hackathon**
> Protecting the weekly income of Zepto & Blinkit delivery partners against uncontrollable external disruptions.

---

## 📌 Problem Statement

India has over **5 million Q-Commerce delivery workers** (Zepto, Blinkit) who are the backbone of the instant delivery economy. These workers operate in dense urban zones, delivering groceries in under 10–20 minutes, earning ₹600–₹1,200/day.

But when external disruptions hit:

- 🌧️ **Heavy Rain / Floods** — Roads are flooded, deliveries halted
- 🌫️ **Severe Air Pollution** — AQI spikes make outdoor work unsafe
- 🚫 **Curfews / Local Strikes** — Zones are locked, pickup impossible
- 🌡️ **Extreme Heat** — Dangerous outdoor conditions

**They cannot work. They earn ₹0. Nobody compensates them.**

These workers lose **20–30% of their monthly income** due to such uncontrollable events. No insurance product in India addresses this specific problem. When disruptions occur, they bear the full financial loss with absolutely no safety net.

> ❌ Zepto doesn't pay them for lost days
> ❌ No government scheme covers this
> ❌ No existing insurance product solves this

---

## 💡 Our Solution — RideCover

RideCover is an **AI-enabled parametric insurance web platform** built exclusively for Q-Commerce delivery workers (Zepto & Blinkit partners).

### What it does:
- Workers pay a **small weekly premium (₹35–₹80/week)**
- Our system **monitors weather and disruptions 24/7** automatically
- When a disruption threshold is breached → **claim is auto-triggered**
- **Lost income is credited to their UPI instantly** — no forms, no calls, no waiting

> ✅ Coverage Scope: **INCOME LOSS ONLY**
> ❌ No health, life, accident, or vehicle repair coverage

### Why Parametric?
Traditional insurance requires the worker to **prove their loss** — file documents, wait weeks, maybe get rejected. Parametric insurance works on **pre-defined triggers** — if rainfall exceeds 50mm/hr, payout happens. No questions asked. No paperwork. Instant.

---

## 👤 Persona & Scenario

### Who Are We Protecting?

| Detail | Info |
|---|---|
| **Name** | Ramesh Kumar |
| **Platform** | Zepto Delivery Partner |
| **City** | Hyderabad |
| **Daily Earnings** | ₹800/day |
| **Working Hours** | 8–12 hours/day |
| **Weekly Earnings** | ~₹5,600/week |
| **Zone** | Kondapur (flood-prone area) |

---

### 📖 Scenario — Without RideCover

> It's a Tuesday afternoon in Hyderabad. The IMD issues a Red Alert for heavy rainfall.
> Zepto suspends all deliveries in Kondapur zone.
> Ramesh sits at home for 6 hours.
> He loses ₹400 in income that day.
> This happens 3–4 times a month during monsoon.
> Monthly loss: ₹1,200–₹1,600. Nobody pays him back.

---

### 📖 Scenario — With RideCover ✅

> Ramesh pays ₹55/week on RideCover — his income insurance.
>
> Tuesday afternoon — IMD Red Alert issued.
> **RideCover's system detects** rainfall > 50mm/hr in Kondapur zone.
> Claim is **automatically triggered** — Ramesh does nothing.
> AI verifies his GPS location and activity.
> **₹400 is credited to his UPI within minutes.**
>
> Ramesh didn't fill any form. He didn't call anyone.
> The money just came. ✅

---

## ⚙️ Application Workflow

```
┌─────────────────────────────────────────┐
│           WORKER ONBOARDING             │
│  Name | Phone | Zone | Platform |       │
│  Average Daily Earnings                 │
└──────────────────┬──────────────────────┘
                   ↓
┌─────────────────────────────────────────┐
│         AI RISK PROFILING               │
│  Analyse zone: flood history, AQI,      │
│  rainfall patterns, disruption freq     │
│  → Generate Zone Risk Score             │
└──────────────────┬──────────────────────┘
                   ↓
┌─────────────────────────────────────────┐
│      POLICY CREATION (WEEKLY)           │
│  Base Premium: ₹35–₹80/week            │
│  Adjusted by Risk Score                 │
│  Worker activates & pays weekly         │
└──────────────────┬──────────────────────┘
                   ↓
┌─────────────────────────────────────────┐
│     REAL-TIME DISRUPTION MONITORING     │
│  Weather API → Rainfall, Temp, AQI      │
│  Social Triggers → Curfew, Strike       │
│  Checks every hour automatically        │
└──────────────────┬──────────────────────┘
                   ↓
┌─────────────────────────────────────────┐
│       PARAMETRIC TRIGGER FIRED          │
│  Threshold breached in worker's zone    │
│  Claim auto-initiated — no action       │
│  needed from the worker                 │
└──────────────────┬──────────────────────┘
                   ↓
┌─────────────────────────────────────────┐
│         FRAUD DETECTION LAYER           │
│  GPS location vs disruption zone        │
│  Activity logs during disruption        │
│  Duplicate claim check                  │
│  Anomaly score via ML model             │
└──────────────────┬──────────────────────┘
                   ↓
┌─────────────────────────────────────────┐
│           INSTANT PAYOUT                │
│  Lost hours × Daily earnings rate       │
│  Credited via UPI / Razorpay            │
│  Worker notified instantly              │
└──────────────────┬──────────────────────┘
                   ↓
┌─────────────────────────────────────────┐
│             DASHBOARD                   │
│  Worker: Income protected, claim history│
│  Admin: Loss ratios, fraud flags,       │
│  zone analytics, predictive insights    │
└─────────────────────────────────────────┘
```

---

## 💰 Weekly Premium Model

| Risk Level | Zone Type | Weekly Premium | Max Weekly Payout |
|---|---|---|---|
| 🟢 Low Risk | Historically safe, low AQI | ₹35/week | ₹800 |
| 🟡 Medium Risk | Moderate disruption history | ₹55/week | ₹1,200 |
| 🔴 High Risk | Flood-prone, high AQI zones | ₹80/week | ₹1,800 |

**Premium is dynamically recalculated every week based on:**
- Historical disruption data for the worker's zone
- Predicted weather forecast for the upcoming week
- Worker's average active hours and earnings baseline

---

## 📡 Parametric Triggers

| # | Trigger | Threshold | Payout Type |
|---|---|---|---|
| 1 | 🌧️ Heavy Rainfall | > 50mm/hr — IMD Red Alert | Per disrupted hour |
| 2 | 🌡️ Extreme Heat | > 45°C sustained for 3+ hrs | Per disrupted hour |
| 3 | 🌫️ Severe AQI | AQI > 300 (Severe Category) | Per disrupted hour |
| 4 | 🌊 Flash Flood Alert | IMD / Government flood warning | Full disrupted shift |
| 5 | 🚫 Unplanned Curfew | Official zone-level curfew | Full disrupted shift |
| 6 | ✊ Local Strike / Bandh | Verified strike in delivery zone | Full disrupted shift |

---

## 🧾 Sample Claim Calculation

```
Worker: Ramesh | Zone: Kondapur | Platform: Zepto
Daily Earnings: ₹800 | Hourly Rate: ₹100/hr

Disruption: Heavy Rainfall — Red Alert
Duration: 6 hours (2 PM – 8 PM)

Claim Amount = Hourly Rate × Disrupted Hours
             = ₹100 × 6
             = ₹600 ✅

Weekly Premium Paid: ₹55
Payout Received: ₹600
Net Benefit: +₹545 for Ramesh
```

---

## 🤖 AI/ML Integration Plan

### 1. Dynamic Premium Calculation
- **Model:** XGBoost / Gradient Boosting
- **Inputs:** Zone flood history, avg AQI, rainfall frequency, seasonal trends
- **Output:** Weekly premium price (₹35–₹80)
- **When:** Recalculated every Monday for the upcoming week

### 2. Predictive Risk Modeling
- **Model:** Time-Series Forecasting (Facebook Prophet)
- **Purpose:** Predict disruption likelihood for next 7 days per zone
- **Use:** Adjust coverage terms and alert workers in advance

### 3. Fraud Detection
- **Model:** Isolation Forest (Anomaly Detection)
- **Checks:**
  - Is worker's GPS in the claimed disruption zone?
  - Were any deliveries made during the claimed disruption window?
  - Is this a duplicate claim for the same event?
  - Is the claim frequency unusually high?
- **Output:** Fraud Risk Score (0–100) → Auto-approve or flag for review

---

## 🛠️ Tech Stack

| Layer | Technology | Purpose |
|---|---|---|
| **Frontend** | React.js + Vite + Tailwind CSS | Web UI — all 5 screens |
| **Backend** | Node.js + Express.js | API, business logic, triggers |
| **Database** | MongoDB | Worker profiles, policies, claims |
| **AI/ML** | Python + scikit-learn + XGBoost | Premium calc + fraud detection |
| **Weather API** | OpenWeatherMap (free tier) | Real-time disruption detection |
| **Payment** | Razorpay Test Mode | Mock UPI payout simulation |
| **Hosting** | Vercel (Frontend) + Render (Backend) | Deployment |
| **Auth** | JWT Tokens | Secure login |

---

## 📁 Repository Structure

```
RideCover/
├── client/                        # React + Vite Frontend
│   ├── src/
│   │   ├── pages/
│   │   │   ├── Register.jsx       # Worker onboarding
│   │   │   ├── Policy.jsx         # Weekly policy & premium
│   │   │   ├── Monitor.jsx        # Live disruption monitor
│   │   │   ├── Claims.jsx         # Auto claim & payout status
│   │   │   └── Dashboard.jsx      # Worker & Admin dashboard
│   │   ├── components/            # Reusable UI components
│   │   └── services/              # API call functions
├── server/                        # Node.js + Express Backend
│   ├── routes/                    # API routes
│   ├── controllers/               # Business logic
│   ├── models/                    # MongoDB schemas
│   └── services/
│       ├── weatherService.js      # OpenWeatherMap integration
│       ├── triggerService.js      # Parametric trigger logic
│       └── payoutService.js       # Razorpay mock integration
├── ml/                            # Python ML Models
│   ├── premium_model.py           # Dynamic pricing model
│   ├── fraud_detection.py         # Anomaly detection
│   └── risk_predictor.py          # Zone risk forecasting
├── README.md
└── .env.example
```

---

## 🗺️ Implementation Plan

### Phase 1 — Ideation & Foundation (March 4–20)
- [x] Finalize persona (Zepto/Blinkit Q-Commerce)
- [x] Define 6 parametric triggers with thresholds
- [x] Design weekly premium model (₹35–₹80)
- [x] Set up GitHub repository
- [x] Write README documentation
- [ ] Create wireframes for all 5 screens
- [ ] Set up React + Vite base project
- [ ] Record 2-minute strategy video

### Phase 2 — Automation & Protection (March 21–April 4)
- [ ] Worker registration and onboarding flow
- [ ] AI-based weekly premium calculation
- [ ] Insurance policy creation and activation
- [ ] OpenWeatherMap API integration
- [ ] Build 5 automated parametric triggers
- [ ] Claims management system
- [ ] Basic fraud detection (rule-based)
- [ ] Mock payout flow (Razorpay test)

### Phase 3 — Scale & Optimise (April 5–17)
- [ ] Advanced ML fraud detection (Isolation Forest)
- [ ] Worker dashboard (income protected, claim history)
- [ ] Admin dashboard (loss ratios, zone analytics)
- [ ] Predictive risk modeling per zone
- [ ] Final 5-minute demo video
- [ ] Pitch deck (PDF)

---

## 🏆 Why Choose RideCover?

### 1. 🎯 Solves a Real Gap
No existing product in India protects gig workers from income loss due to environmental disruptions. This is a completely underserved market of 5 million+ workers.

### 2. ⚡ Zero-Touch Claims
Worker never needs to file anything. The system detects, validates, and pays — fully automated. This is the biggest UX advantage over traditional insurance.

### 3. 📍 Hyper-Local Pricing
Premium is based on the **worker's actual zone risk** — not a national average. A worker in a flood-safe zone pays less. Fair, transparent, data-driven.

### 4. 📅 Weekly Model = Gig Worker Friendly
Gig workers think and earn week-to-week. A weekly premium of ₹55 is psychologically easier than ₹220/month. Matches their exact earning cycle.

### 5. 🤖 AI-Powered, Not Manual
Every part of RideCover is automated — premium calculation, disruption detection, fraud check, payout. No human bottleneck in the claim process.

### 6. 🔒 Fraud-Proof
Multi-layer AI validation before every payout — GPS check, activity logs, duplicate detection. Protects the insurer while being seamless for genuine workers.

### 7. 📱 Inclusive Design
Simple web UI that works on any browser, including basic Android phones. No app download required. Designed for workers with limited tech literacy.

---

## 👥 Team

| Name | Role |
|---|---|
| [Mahesh Bollineni] | Lead |
| [BHUDETI D V V SIVARAMPRASAD] | Member |
| [NALLAMOTHU GIRISH CHOWDARY] | Member |

---

## 📎 Links

- 🎥 Phase 1 Video: [Link coming soon]
- 💻 GitHub Repo: [Link coming soon]


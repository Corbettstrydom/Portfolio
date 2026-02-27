# QA Portfolio – Corbett Strydom
> Aspiring QA Engineer | Business Systems Student | Fintech & Payments Focus | Cape Town, South Africa

[![AWS Certified](https://img.shields.io/badge/AWS-Cloud%20Practitioner-FF9900?style=flat&logo=amazon-aws)](https://aws.amazon.com/certification/)
[![Cybersecurity](https://img.shields.io/badge/Cybersecurity-Certificate%20CPUT-blue?style=flat)](https://www.cput.ac.za/)
[![Status](https://img.shields.io/badge/Status-Open%20to%20Work-brightgreen?style=flat)]()
[![Portfolio](https://img.shields.io/badge/Projects-7-4472C4?style=flat)]()

---

## 👋 About Me

I'm a Business Systems student at Rosebank College (graduating 2027) based in Cape Town, South Africa. I'm building a career in **QA engineering with a focus on fintech and payments infrastructure**.

This portfolio documents hands-on testing work across real and industry-standard environments, as well as academic work in financial and transactional data analysis — built to demonstrate practical QA and data skills before entering the industry as a junior QA engineer.

I'm interested in roles involving **integration testing, payment system validation, defect management, and financial data quality** in fintech or digital banking environments.

---

## 📁 Portfolio Projects

### 💳 01 – Stripe Payment Flow Testing
**Type:** Functional | Risk-Based | Payment Testing  
**Environment:** Stripe Payments Demo (test mode) · Chrome · Windows 11  
**Folder:** `/stripe-payment-testing`

End-to-end structured testing of the Stripe checkout flow covering happy path, card declines, input validation, edge cases, 3D Secure authentication, and post-payment confirmation.

| Metric | Result |
|---|---|
| Test Cases Executed | 12 |
| Tests Passed | 12 |
| Risks Identified | 8 |
| Test Areas Covered | Happy Path, Error Handling, Validation, Edge Cases, Authentication, Post-Payment |

**Deliverables:**
- ✅ User journey map (6-step happy path)
- ✅ 12 test cases with expected and actual results
- ✅ Risk register with likelihood, severity, and safeguard recommendations
- ✅ Screenshot evidence for each test case
- ✅ Key findings report

**🔍 Key Finding:**  
Idempotency handling confirmed — rapid double-click on Pay produces only one payment intent. No duplicate charge created. Button is correctly disabled on first click with loading state shown.

---

### 🛒 02 – SauceDemo E-Commerce Exploratory Testing
**Type:** Exploratory | Functional | Multi-Persona Testing  
**Environment:** saucedemo.com · Chrome · Windows 11  
**Folder:** `/saucedemo-testing`

Exploratory and functional testing across three user personas (`standard_user`, `problem_user`, `performance_glitch_user`), uncovering functional defects, UI failures, and a session-level security finding.

| Metric | Result |
|---|---|
| Bugs Logged | 15 |
| Critical / High Severity | 9 |
| User Personas Tested | 3 |
| Duplicate Bugs Identified | 6 (correctly linked to root cause SD-BUG-004) |

**Deliverables:**
- ✅ 15 bug reports with severity, priority, steps to reproduce, and screenshot evidence
- ✅ Key findings report with risk impact assessment
- ✅ Correct deduplication of product navigation defects to a single root cause

**🔍 Key Finding:**  
Cart contents persisted between different user sessions after a logout/login switch. In a real system, this is a **session isolation defect** with data privacy implications — relevant to any fintech or e-commerce platform handling user data.

---

### 🇿🇦 03 – Takealot Cart & Checkout Testing
**Type:** Functional | Exploratory | Real-World Platform  
**Environment:** takealot.com · Chrome · Windows 11  
**Folder:** `/takealot-testing`

Functional and exploratory testing of South Africa's largest e-commerce platform, focusing on cart management, checkout flow, session handling, input validation, and UI responsiveness.

| Metric | Result |
|---|---|
| Test Cases Executed | 10 |
| Passed | 9 |
| Not Run | 1 (session timeout – flagged honestly, not forced) |
| Bugs Logged | 10 |

**Deliverables:**
- ✅ 10 structured test cases with pass/fail status
- ✅ 10 bug reports covering UI, validation, state management, and concurrency
- ✅ Tested on a live production environment

**🔍 Key Finding:**  
Rapid quantity changes cause delayed and inconsistent cart UI updates — a timing/concurrency defect with direct relevance to high-traffic payment and checkout systems.

---

### 📄 04 – Stripe Initial Test Report
**Type:** Structured Functional Testing  
**Environment:** Stripe Payments Demo · Chrome · Windows 11  
**Folder:** `/stripe-initial-report`

An earlier focused test report covering 4 core payment scenarios with formal pass/fail reporting, scope definition, environment documentation, and a key findings summary. Included to show portfolio progression and testing discipline from the start.

| Metric | Result |
|---|---|
| Test Cases | 4 |
| Passed | 4 |
| Scenarios Covered | Happy path, generic decline, invalid card, duplicate submission |

---

### 📊 05 – Financial News & Market Events Analysis
**Type:** Financial Data Analysis | Business Intelligence | Data Visualisation  
**Tools:** Google Looker Studio · Microsoft Excel · CSV Data Analysis  
**Folder:** `/university-work/financial-news-analysis`  
**Grade:** 80%+

Analysis of two financial news event datasets covering global market movements, trading volumes, sentiment, profit/loss outcomes, and sector impact across 18 major indices. The primary dataset contains **3,033 real market event records** spanning February–August 2025, sourced from major financial publications.

| Metric | Detail |
|---|---|
| Total Records | 3,033 market event entries |
| Date Range | February 2025 – August 2025 |
| Market Indices | 18 (Nasdaq, FTSE 100, S&P 500, Hang Seng, DAX, Nikkei 225, ASX 200, and more) |
| Companies Tracked | Apple, Microsoft, Tesla, JP Morgan Chase, Goldman Sachs, Boeing, Samsung, and more |
| Market Event Types | 20 (IPO launches, interest rate changes, geopolitical events, earnings reports, and more) |
| Sectors Covered | 18 (Finance, Technology, Healthcare, Energy, Automotive, and more) |
| News Sources | Bloomberg, Reuters, Financial Times, Wall Street Journal, CNBC, and more |
| Outcome Analysis | Profit/Loss classification using IF logic across all records |

**Deliverables:**
- ✅ Raw datasets (CSV) with financial news events and market data
- ✅ Interactive Looker Studio dashboard with market event analysis
- ✅ Sentiment analysis across market events and sectors
- ✅ Profit/Loss outcome classification using Excel IF functions
- ✅ Trading volume and index change analysis across global markets
- ✅ Pivot summary table filtered by company (Apple Inc.)

**📊 Live Dashboard:** [View Financial News Events Dashboard on Looker Studio](https://lookerstudio.google.com/reporting/16d1bbea-ba9d-4011-9d30-334b0c7fc81c)

**🔍 Why This Matters for Fintech QA:**  
Understanding the financial data that flows through payment and banking systems is as important as knowing how to test it. This project demonstrates hands-on experience with real financial data structures, market event classification, sentiment analysis, and global market indices — all directly relevant to testing data integrity and validation in fintech environments.

---

### 🚗 06 – Ride Bookings Transactional Data Analysis
**Type:** Transactional Data Analysis | Operational Data Quality | Business Intelligence  
**Tools:** Microsoft Excel · CSV Data Analysis  
**Folder:** `/university-work/ride-bookings-analysis`  
**Grade:** 80%+

Analysis of a production-scale ride-booking dataset containing **150,000 booking records** across a full year. The dataset covers booking status, cancellation flows, payment methods, vehicle types, driver and customer ratings, ride distances, and booking values — mirroring the kind of transactional data that sits behind any payments or mobility fintech platform.

| Metric | Detail |
|---|---|
| Total Records | 150,000 ride booking entries |
| Date Range | Full year (365 days) |
| Booking Statuses | Completed, Cancelled by Customer, Cancelled by Driver, Incomplete, No Driver Found |
| Vehicle Types | 7 (Auto, Bike, eBike, Go Mini, Go Sedan, Premier Sedan, Uber XL) |
| Payment Methods | 6 (Cash, Credit Card, Debit Card, UPI, Uber Wallet) |
| Locations | 176 unique pickup and drop locations |
| Cancellation Reasons | Customer-side (5 reasons) and Driver-side (4 reasons) tracked separately |
| Ratings | Driver and Customer ratings (3.0–5.0 scale) |

**Deliverables:**
- ✅ Raw dataset (CSV) with 150,000 booking records
- ✅ Booking status distribution analysis (completed vs cancelled vs incomplete)
- ✅ Cancellation pattern analysis by customer and driver reason
- ✅ Payment method breakdown across booking types
- ✅ Null value analysis — understanding conditional data population by booking status
- ✅ Driver and customer rating trend analysis

**🔍 Why This Matters for Fintech QA:**  
This dataset mirrors the transactional data structure of any ride-hailing or payments platform. Key QA-relevant observations include: booking values and ratings are null for cancelled/incomplete rides (conditional data population based on status), payment method coverage across 6 types, including UPI and digital wallets, and cancellation reason tracking on both sides of a transaction — all patterns directly applicable to testing payment and booking systems in fintech.

---

### 🎓 07 – University Academic Projects
**Type:** Academic | Business Systems | Data Analysis  
**Folder:** `/university-work`  
**Grade:** 80%+ across projects

A collection of academic projects completed as part of my Bachelor of Information Technology in Business Systems at Rosebank College. Included to demonstrate consistent academic performance and technical breadth alongside independent portfolio work.

---

## 🛠️ Skills Demonstrated

| Skill | Evidence |
|---|---|
| Test case design & execution | Projects 01, 02, 03, 04 |
| Bug reporting & defect lifecycle | SauceDemo (15 bugs), Takealot (10 bugs) |
| Risk-based testing | Stripe risk register |
| Exploratory testing | SauceDemo, Takealot |
| Multi-persona testing | SauceDemo (3 user types) |
| Session & security-aware testing | SauceDemo cross-user cart finding |
| Evidence & screenshot documentation | All QA projects |
| Duplicate/root cause identification | SauceDemo SD-BUG-004 |
| Payment flow testing | Stripe (both projects) |
| Financial data analysis | 3,033-record market events dataset |
| Transactional data analysis | 150,000-record ride bookings dataset |
| Null value & data quality analysis | Ride bookings conditional data population |
| Data visualisation | Looker Studio dashboard |
| Excel IF functions & data classification | Profit/Loss outcome analysis |
| Business intelligence reporting | Financial News Events dashboard |

---

## 🧰 Tools & Technologies

![Chrome](https://img.shields.io/badge/Chrome-DevTools-4285F4?style=flat&logo=google-chrome)
![Jira](https://img.shields.io/badge/Jira-Defect%20Tracking-0052CC?style=flat&logo=jira)
![Excel](https://img.shields.io/badge/Excel-Advanced-217346?style=flat&logo=microsoft-excel)
![GitHub](https://img.shields.io/badge/GitHub-Portfolio-181717?style=flat&logo=github)
![AWS](https://img.shields.io/badge/AWS-Cloud%20Practitioner-FF9900?style=flat&logo=amazon-aws)
![Python](https://img.shields.io/badge/Python-Scripting%20Basics-3776AB?style=flat&logo=python)
![SQL](https://img.shields.io/badge/SQL-Query%20Writing-4479A1?style=flat&logo=mysql)
![Looker Studio](https://img.shields.io/badge/Looker%20Studio-Data%20Visualisation-4285F4?style=flat&logo=google)
![Wireshark](https://img.shields.io/badge/Wireshark-Network%20Analysis-1679A7?style=flat)

---

## 📜 Certifications

- 🏅 **AWS Certified Cloud Practitioner** — Amazon Web Services
- 🏅 **Cybersecurity Certificate** — CPUT

---

## 🎓 Education

**Bachelor of Information Technology in Business Systems**  
Rosebank College · In Progress · Expected 2027  
*Relevant coursework: Business systems analysis, process optimisation, data analysis, cybersecurity foundations, cloud computing*

---

## 📬 Contact

📧 Corbettstrydom6@gmail.com  
🔗 [linkedin.com/in/corbett-strydom](https://www.linkedin.com/in/corbett-strydom)  
📍 Cape Town, South Africa  

---

*Open to junior QA, integration testing, and business systems roles in fintech and digital banking.*

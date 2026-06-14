# QA & Automation Portfolio – Corbett Strydom

> Co-Founder at BlkQuarry | AI & Business Operations Consulting | Business Systems Student | Cape Town, South Africa

[![AWS Certified](https://img.shields.io/badge/AWS-Cloud%20Practitioner-FF9900?style=flat&logo=amazon-aws)](https://aws.amazon.com/certification/)
[![Cybersecurity](https://img.shields.io/badge/Cybersecurity-Certificate%20CPUT-blue?style=flat)](https://www.cput.ac.za/)
[![Status](https://img.shields.io/badge/Status-Open%20to%20Work-brightgreen?style=flat)](https://github.com/Corbettstrydom/Portfolio)
[![BlkQuarry](https://img.shields.io/badge/BlkQuarry-blkquarry.com-0A0F4F?style=flat)](https://blkquarry.com)
[![Portfolio](https://img.shields.io/badge/Projects-9-4472C4?style=flat)](https://github.com/Corbettstrydom/Portfolio)

-----

## 👋 About Me

I co-founded BlkQuarry, an AI and business operations consulting firm that helps mid-size businesses fix broken processes, eliminate wasted AI spend, and build automation systems that actually work. My work sits at the intersection of business analysis and technical delivery — I work with operations leads, CEOs, and CFOs to turn underperforming processes into measurable results, then build the systems that make it happen.

I started building and testing the business infrastructure earlier this year, going public in May 2026 with a paid client engagement already delivered. The projects in this portfolio are a mix of that client work, automation tools I built for the business, and the QA and data work that underpins the consulting practice.

I am a final-year Business IT student at Rosebank College (graduating 2027), AWS Cloud Practitioner certified, and in 2026 was selected for the South African national men’s water polo squad.

-----

## 📁 Portfolio Projects

### 🔧 01 – Business Process Automation (Client Delivery)

**Type:** n8n · Workflow Automation · Client Consulting
**Status:** Delivered — Professional Services Client, Cape Town *(NDA)*

Built and deployed an n8n automation pipeline for a professional services client, replacing a manual multi-step workflow with a fully automated system. Handled data routing between multiple business tools, eliminating repetitive manual tasks and reducing operational overhead entirely.

**Scope:**

- Requirements gathering and AS-IS process mapping
- n8n pipeline architecture and build
- End-to-end testing and error handling
- Handover documentation and client walkthrough

**Outcome:** Manual data routing process eliminated. Client team no longer handles the workflow by hand.

-----

### 🖥️ 02 – Role-Based Job Tracking Web App (Client Delivery)

**Type:** Web Application · Business Systems · Client Consulting
**Status:** Delivered — Print & Logistics Client, Cape Town *(NDA)*

Built and delivered a role-based job tracking web application for a client in the print and logistics space. The system manages the full job lifecycle across multiple user roles with real-time status visibility for operations and management.

|Metric    |Detail                                                    |
|----------|----------------------------------------------------------|
|Users     |6 role-based accounts                                     |
|Job Stages|5                                                         |
|Features  |Dropdown intake, admin KAM view, real-time status tracking|
|Process   |Requirements gathering → build → UAT → handover           |

**Outcome:** Manual job tracking replaced with a structured digital system. Management has real-time visibility across all active jobs.

-----

### 🏠 03 – Booking Automation System (Client Delivery)

**Type:** Python · API Integration · Workflow Automation
**Status:** Delivered — Hospitality Client, Cape Town *(NDA — private repo)*

Built a multi-platform booking automation system for a short-term rental property. The system prevents double bookings, syncs availability across platforms in real time, and automates the full post-checkout workflow including owner and cleaner notifications.

**Key features:**

- Booking lock system — soft locks availability the moment a guest starts a reservation, preventing double bookings during the payment window across all platforms simultaneously
- Automated calendar sync via channel manager integration
- Owner WhatsApp notification on every confirmed booking with guest name, arrival time, platform, and booking value
- Automated arrival reminder to owner the day before each check-in
- Cleaner WhatsApp notification on checkout day with one-tap mobile clean confirmation portal
- Availability re-opens automatically across all platforms once cleaner confirms room is ready

**Outcome:** Double booking risk eliminated. Owner and cleaner workflows fully automated with zero manual intervention required.

-----

### 🤖 04 – Lead Generation and Outbound Automation System

**Type:** Python · Playwright · SMTP · Claude API
**Folder:** `/tools`

A two-part outbound system built for BlkQuarry’s prospecting pipeline. Removes dependency on paid SaaS tools for lead sourcing and outreach at scale.

|Feature         |Detail                                                          |
|----------------|----------------------------------------------------------------|
|Scraper input   |Business type + location (e.g. “logistics company in Cape Town”)|
|Output          |CSV with name, address, phone, website, email                   |
|Email extraction|Visits each business website and /contact page                  |
|Max results     |Configurable, up to ~120 per search                             |
|Email providers |Zoho, Gmail, Outlook, any SMTP                                  |
|Personalisation |Claude API for dynamic copy at scale                            |
|Follow-up logic |Adapts based on open and reply behaviour                        |
|Volume          |~1,600 contacts per month                                       |

**Use case:** BlkQuarry outbound prospecting — identify businesses by industry and location, extract decision-maker contact info, send personalised first-touch emails and follow-ups without a paid SaaS tool.

-----

### 📰 05 – AI News Summariser

**Type:** Python · LLM Integration · Scheduled Automation
**Folder:** `/tools`

Pulls articles from multiple sources, filters by topic, and generates clean summaries automatically using an LLM. Runs on a schedule with no manual input. Outputs formatted for newsletters or internal briefings.

-----

### 💳 06 – Stripe Payment Flow Testing

**Type:** Functional | Risk-Based | Payment Testing
**Environment:** Stripe Payments Demo (test mode) · Chrome · Windows 11
**Folder:** `/stripe-payment-testing`

End-to-end structured testing of the Stripe checkout flow covering happy path, card declines, input validation, edge cases, 3D Secure authentication, and post-payment confirmation.

|Metric             |Result                                                                          |
|-------------------|--------------------------------------------------------------------------------|
|Test Cases Executed|12                                                                              |
|Tests Passed       |12                                                                              |
|Risks Identified   |8                                                                               |
|Test Areas Covered |Happy Path, Error Handling, Validation, Edge Cases, Authentication, Post-Payment|

**🔍 Key Finding:**
Idempotency handling confirmed — rapid double-click on Pay produces only one payment intent. No duplicate charge created. Button is correctly disabled on first click with loading state shown.

-----

### 🛒 07 – SauceDemo E-Commerce Exploratory Testing

**Type:** Exploratory | Functional | Multi-Persona Testing
**Environment:** saucedemo.com · Chrome · Windows 11
**Folder:** `/saucedemo-testing`

Exploratory and functional testing across three user personas (`standard_user`, `problem_user`, `performance_glitch_user`), uncovering functional defects, UI failures, and a session-level security finding.

|Metric                   |Result                                       |
|-------------------------|---------------------------------------------|
|Bugs Logged              |15                                           |
|Critical / High Severity |9                                            |
|User Personas Tested     |3                                            |
|Duplicate Bugs Identified|6 (correctly linked to root cause SD-BUG-004)|

**🔍 Key Finding:**
Cart contents persisted between different user sessions after a logout/login switch — a **session isolation defect** with data privacy implications relevant to any platform handling user data.

-----

### 📊 08 – Financial News & Market Events Analysis

**Type:** Financial Data Analysis | Business Intelligence | Data Visualisation
**Tools:** Python · Google Looker Studio · Microsoft Excel
**Folder:** `/university-work/financial-news-analysis`
**Grade:** 80%+

Analysis of 3,033 real market event records spanning 18 major global indices. Built an interactive Looker Studio dashboard surfacing event-driven price movement patterns for decision-maker review.

|Metric            |Detail                                                              |
|------------------|--------------------------------------------------------------------|
|Total Records     |3,033 market event entries                                          |
|Market Indices    |18 (Nasdaq, FTSE 100, S&P 500, Hang Seng, DAX, Nikkei 225, and more)|
|Market Event Types|20                                                                  |
|Sectors Covered   |18                                                                  |

**📊 Live Dashboard:** [View Financial News Events Dashboard on Looker Studio](https://lookerstudio.google.com/reporting/16d1bbea-ba9d-4011-9d30-334b0c7fc81c)

-----

### 🚗 09 – Ride Bookings Transactional Data Analysis

**Type:** Transactional Data Analysis | Operational Data Quality | Business Intelligence
**Tools:** Python · Microsoft Excel
**Folder:** `/university-work/ride-bookings-analysis`
**Grade:** 80%+

Analysis of a production-scale ride-booking dataset containing 150,000 booking records across a full year, identifying booking behaviour, peak demand windows, cancellation patterns, and operational inefficiencies across 176 locations.

|Metric          |Detail                              |
|----------------|------------------------------------|
|Total Records   |150,000 ride booking entries        |
|Booking Statuses|5                                   |
|Vehicle Types   |7                                   |
|Payment Methods |6                                   |
|Locations       |176 unique pickup and drop locations|

-----

## 🛠️ Skills Demonstrated

|Skill                           |Evidence                                       |
|--------------------------------|-----------------------------------------------|
|Client delivery end-to-end      |Projects 01, 02, 03                            |
|Workflow automation             |n8n, Python, Playwright, SMTP, API integration |
|Business process mapping        |AS-IS/TO-BE analysis across all client projects|
|Requirements gathering          |Client discovery and solution scoping          |
|Test case design & execution    |Projects 06, 07                                |
|Bug reporting & defect lifecycle|SauceDemo (15 bugs)                            |
|Risk-based testing              |Stripe risk register                           |
|Exploratory testing             |SauceDemo, Takealot                            |
|Financial data analysis         |3,033-record market events dataset             |
|Transactional data analysis     |150,000-record ride bookings dataset           |
|Data visualisation              |Looker Studio dashboard                        |
|LLM integration                 |Claude API, prompt engineering                 |

-----

## 🧰 Tools & Technologies

[![Python](https://img.shields.io/badge/Python-Automation-3776AB?style=flat&logo=python)](https://python.org)
[![n8n](https://img.shields.io/badge/n8n-Workflow%20Automation-EA4B71?style=flat)](https://n8n.io)
[![Claude API](https://img.shields.io/badge/Claude-API%20Integration-0A0F4F?style=flat)](https://anthropic.com)
[![AWS](https://img.shields.io/badge/AWS-Cloud%20Practitioner-FF9900?style=flat&logo=amazon-aws)](https://aws.amazon.com/certification/)
[![SQL](https://img.shields.io/badge/SQL-Query%20Writing-4479A1?style=flat&logo=mysql)](https://mysql.com)
[![Looker Studio](https://img.shields.io/badge/Looker%20Studio-Data%20Visualisation-4285F4?style=flat&logo=google)](https://lookerstudio.google.com)
[![Excel](https://img.shields.io/badge/Excel-Advanced-217346?style=flat&logo=microsoft-excel)](https://microsoft.com)
[![GitHub](https://img.shields.io/badge/GitHub-Portfolio-181717?style=flat&logo=github)](https://github.com/Corbettstrydom)
[![Jira](https://img.shields.io/badge/Jira-Defect%20Tracking-0052CC?style=flat&logo=jira)](https://atlassian.com/jira)

-----

## 📜 Certifications

- 🏅 **AWS Certified Cloud Practitioner** — Amazon Web Services
- 🏅 **Cybersecurity Certificate** — CPUT

-----

## 🎓 Education

**Bachelor of Information Technology in Business Systems**
Rosebank College · In Progress · Expected 2027
*Relevant coursework: Business systems analysis, process optimisation, data analysis, cybersecurity foundations, cloud computing*

-----

## 🏆 Awards

**South African National Men’s Water Polo Squad — 2026**
Selected to represent South Africa at national level, one of a small number of players chosen from across the country.

-----

## 📬 Contact

📧 [corbett@blkquarry.com](mailto:corbett@blkquarry.com)
🌐 [blkquarry.com](https://blkquarry.com)
🔗 [linkedin.com/in/corbett-strydom](https://www.linkedin.com/in/corbett-strydom)
📍 Cape Town, South Africa

-----

*Open to consulting engagements, junior analyst roles, and operations and automation projects in Cape Town and remotely.*
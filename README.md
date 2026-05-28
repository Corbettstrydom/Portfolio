# Corbett Strydom – AI & Automation Portfolio

> Co-Founder at BlkQuarry · AI Consulting · Automation Engineering · Cape Town, South Africa

[![BlkQuarry](https://img.shields.io/badge/BlkQuarry-AI%20Consulting-2F3FD3?style=flat)](https://blkquarry.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-corbettstrydom-0A66C2?style=flat&logo=linkedin)](https://www.linkedin.com/in/corbettstrydom)
[![Status](https://img.shields.io/badge/Status-Open%20to%20Work-brightgreen?style=flat)](https://blkquarry.com)
[![Location](https://img.shields.io/badge/Location-Cape%20Town%2C%20SA-0A0F4F?style=flat)]()

---

## About

I co-founded [BlkQuarry](https://blkquarry.com), an AI consulting firm that helps mid-size businesses fix broken AI implementations, build custom automation systems, and identify where AI spend is being wasted.

My work sits at the intersection of business operations and technical delivery. I work with CEOs, Operations Directors, and CFOs to turn underperforming AI investments into measurable results — and I build the tools to make that happen.

This portfolio documents the automation systems, lead generation tools, and client-facing projects I build as part of that work.

---

## Projects

### 01 – Google Maps Lead Scraper

**Type:** Python · Web Scraping · Lead Generation  
**Folder:** [`/tools/maps_scraper.py`](./tools/maps_scraper.py)

A Playwright-based scraper that searches Google Maps by business type and location, extracts business details (name, address, phone, website), and then visits each website to extract contact email addresses. Exports everything to a timestamped CSV ready for outreach.

| Feature | Detail |
|---|---|
| Input | Business type + location (e.g. "marketing agency in Cape Town") |
| Output | CSV with name, address, phone, website, email |
| Email extraction | Scrapes business website and /contact page |
| Max results | Configurable, up to ~120 per search |

**Use case:** BlkQuarry outbound prospecting — identify SMEs by industry and location, extract decision-maker contact info at scale.

---

### 02 – Cold Email Sender

**Type:** Python · SMTP · Outbound Automation  
**Folder:** [`/tools/cold_email_sender.py`](./tools/cold_email_sender.py)

Reads a leads CSV (from the scraper or any source), sends personalised cold emails via SMTP with configurable delay between sends to avoid spam filters. Works with Zoho, Gmail, Outlook, or any SMTP provider. Logs every send attempt to a timestamped CSV.

| Feature | Detail |
|---|---|
| Input | Leads CSV + SMTP credentials |
| Personalisation | Business name injected into subject and body |
| Providers | Zoho, Gmail, Outlook, custom SMTP |
| Safety | Configurable delay between sends (default 45s) |
| Logging | Sent/failed log with timestamps |

**Use case:** BlkQuarry outbound sequence — follow up on scraped leads with a personalised first-touch email at scale, without paying for a SaaS tool.

---

### 03 – n8n Business Process Automation (Client Project)

**Type:** n8n · Workflow Automation · Client Delivery  
**Status:** Delivered — Professional Services Client, Cape Town

Built and deployed an n8n automation pipeline for a professional services client, replacing a manual multi-step workflow with a fully automated system. The solution handled data routing between multiple business tools, eliminating repetitive manual tasks and reducing operational overhead.

**Scope:**
- Requirements gathering and process mapping
- n8n pipeline architecture and build
- End-to-end testing and error handling
- Handover documentation and client walkthrough

**Outcome:** Manual process eliminated. Client's team no longer handles data routing between tools manually.

> *This is a paid client engagement delivered under BlkQuarry. Full workflow documentation available on request.*

---

### 04 – QA & Data Analysis Projects (Previous Work)

**Type:** Quality Assurance · Fintech · Data Analysis  
**Folder:** [`/Portfolio`](./Portfolio)

A collection of structured QA testing projects and financial data analysis work completed prior to founding BlkQuarry. Included to demonstrate testing discipline, attention to detail, and data skills that underpin the consulting work.

Highlights:
- Stripe payment flow testing (12 test cases, 8 risks identified)
- SauceDemo exploratory testing (15 bugs, session isolation defect found)
- Financial market events analysis (3,033 records, Looker Studio dashboard)
- Ride bookings transactional data analysis (150,000 records)

---

## Tools & Technologies

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![n8n](https://img.shields.io/badge/n8n-Automation-EA4B71?style=flat)
![Playwright](https://img.shields.io/badge/Playwright-Web%20Scraping-45ba4b?style=flat)
![Zapier](https://img.shields.io/badge/Zapier-FF4A00?style=flat&logo=zapier&logoColor=white)
![Make](https://img.shields.io/badge/Make.com-Automation-6D00CC?style=flat)
![SQL](https://img.shields.io/badge/SQL-Query%20Writing-4479A1?style=flat&logo=mysql&logoColor=white)
![SMTP](https://img.shields.io/badge/SMTP-Email%20Automation-grey?style=flat)
![Looker Studio](https://img.shields.io/badge/Looker%20Studio-Data%20Visualisation-4285F4?style=flat&logo=google)

---

## Services (BlkQuarry)

| Service | Description | From |
|---|---|---|
| AI Business Audit | Identify where AI spend is wasted | $830 |
| AI Rescue Consulting | Fix broken AI implementations (90-day guarantee) | $4,100 |
| Custom AI Bot Build | Build AI systems that work (3–6 weeks) | $1,950 |
| Monthly Retainer | Ongoing AI operations support | $440/mo |
| Fractional AI Officer | Part-time AI leadership for your business | $1,100/mo |

→ [blkquarry.com](https://blkquarry.com)

---

## Certifications

- Cybersecurity Certificate — CPUT
- Bachelor of IT in Business Systems — IIE Rosebank College (in progress, 2027)

---

## Contact

📧 corbett.strydom000@gmail.com  
🔗 [linkedin.com/in/corbettstrydom](https://www.linkedin.com/in/corbettstrydom)  
🌐 [blkquarry.com](https://blkquarry.com)  
📍 Cape Town, South Africa

---

*Available for Upwork contracts · Automation builds · AI implementation projects*

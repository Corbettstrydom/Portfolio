# QA Portfolio – Corbett Strydom
> Aspiring QA Engineer | Business Systems Student | Fintech & Payments Focus | Cape Town, South Africa

[![AWS Certified](https://img.shields.io/badge/AWS-Cloud%20Practitioner-FF9900?style=flat&logo=amazon-aws)](https://aws.amazon.com/certification/)
[![Cybersecurity](https://img.shields.io/badge/Cybersecurity-Certificate%20CPUT-blue?style=flat)](https://www.cput.ac.za/)
[![Status](https://img.shields.io/badge/Status-Open%20to%20Work-brightgreen?style=flat)]()

---

## 👋 About Me

I'm a Business Systems student at Rosebank College (graduating 2027) based in Cape Town, South Africa. I'm building a career in **QA engineering with a focus on fintech and payments infrastructure**.

This portfolio documents hands-on testing work across real and industry-standard environments — built independently to demonstrate practical QA skills before entering the industry as a junior QA engineer.

I'm interested in roles involving **integration testing, payment system validation, and defect management** in fintech or digital banking environments.

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
Idempotency handling confirmed — rapid double-click on Pay produces only one payment intent. No duplicate charge created. Button correctly disabled on first click with loading state shown.

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
- ✅ Correct deduplication of product navigation defects to single root cause

**🔍 Key Finding:**  
Cart contents persisted between different user sessions after logout/login switch. In a real system this is a **session isolation defect** with data privacy implications — relevant to any fintech or e-commerce platform handling user data.

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

## 🛠️ Skills Demonstrated

| Skill | Evidence |
|---|---|
| Test case design & execution | All 4 projects |
| Bug reporting & defect lifecycle | SauceDemo (15 bugs), Takealot (10 bugs) |
| Risk-based testing | Stripe risk register |
| Exploratory testing | SauceDemo, Takealot |
| Multi-persona testing | SauceDemo (3 user types) |
| Session & security-aware testing | SauceDemo cross-user cart finding |
| Evidence & screenshot documentation | All 4 projects |
| Duplicate/root cause identification | SauceDemo SD-BUG-004 |
| Payment flow testing | Stripe (both projects) |

---

## 🧰 Tools & Technologies

![Chrome](https://img.shields.io/badge/Chrome-DevTools-4285F4?style=flat&logo=google-chrome)
![Jira](https://img.shields.io/badge/Jira-Defect%20Tracking-0052CC?style=flat&logo=jira)
![Excel](https://img.shields.io/badge/Excel-Test%20Management-217346?style=flat&logo=microsoft-excel)
![GitHub](https://img.shields.io/badge/GitHub-Portfolio-181717?style=flat&logo=github)
![AWS](https://img.shields.io/badge/AWS-Cloud%20Practitioner-FF9900?style=flat&logo=amazon-aws)
![Python](https://img.shields.io/badge/Python-Scripting%20Basics-3776AB?style=flat&logo=python)
![SQL](https://img.shields.io/badge/SQL-Query%20Writing-4479A1?style=flat&logo=mysql)

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

# 🚨 Cross-Session Account Misuse Investigation (Shared Lab Environment)

## 📂 Repository Name

`chatgpt-session-misuse-investigation`

---

## 📄 README.md

## 📌 Executive Summary

This case study documents an incident involving unauthorized account usage caused by session persistence on a shared college laboratory system. A student unknowingly accessed another user's ChatGPT account due to an active session left open on a shared machine.

The investigation focused on identifying the source system and attributing the activity to a specific user using behavioral analysis and indirect indicators.

---

## 🧠 Incident Overview

* **Incident Type:** Session Persistence / Unauthorized Account Usage
* **Environment:** Shared College Computer Lab
* **Affected Asset:** ChatGPT Account
* **Severity:** Medium

---

## ⏱️ Timeline of Events

| Timeframe | Event                                                        |
| --------- | ------------------------------------------------------------ |
| Day 1     | Unrecognized chat activity observed in account               |
| Day 2–3   | Continued monitoring confirms ongoing unauthorized usage     |
| Day 4     | Live observation conducted in lab environment                |
| Day 4     | Initial attribution attempt (user name prompt) failed        |
| Day 4     | Behavioral artifact identified ("program 12" naming pattern) |
| Day 4     | User successfully identified through correlation             |

---

## 🔍 Indicators of Compromise (IoCs)

* Unknown chat messages appearing in account
* Repeated usage patterns not matching account owner
* Presence of consistent naming convention (e.g., "program 12")

---

## 🧪 Investigation Methodology

### 1. Monitoring & Validation

* Observed repeated unauthorized activity over multiple days
* Confirmed activity was real-time, not historical

### 2. Live Environment Analysis

* Physically accessed lab during active session usage
* Correlated real-time activity with account behavior

### 3. Attribution Attempts

#### Attempt 1: Direct User Identification

* Asked user to input their name in chat
* Failed due to message not being submitted

#### Attempt 2: Behavioral Correlation (Successful)

* Identified unique naming artifact: "program 12"
* Queried lab users regarding naming pattern
* User confirmed ownership, establishing attribution

---

## 🧬 Root Cause Analysis

* User failed to log out from ChatGPT on shared system
* Browser session remained active (persistent cookies/session token)
* Subsequent user accessed the same system
* ChatGPT reused existing authenticated session

---

## ⚠️ Impact Assessment

* Exposure of private conversations
* Unauthorized usage of account
* Potential academic or personal data leakage

---

## 🛠️ Remediation Actions

* Logged out from all active sessions
* Cleared browser cookies and cache
* Educated users on session management practices

---

## 🔐 Preventive Measures

* Always log out from shared systems
* Use private/incognito browsing in public environments
* Enable multi-factor authentication (MFA)
* Avoid saving sessions on shared devices

---

## 📘 Lessons Learned

* Session persistence can lead to unauthorized access without credential compromise
* Behavioral indicators are valuable for attribution when logs are unavailable
* Physical verification can be critical in endpoint investigations
* Multi-day observation improves accuracy of incident validation

---

## 🧑‍💻 Skills Demonstrated

* Incident Detection & Analysis
* Behavioral Correlation
* Endpoint Investigation
* Root Cause Analysis
* Real-time Monitoring

---

## 📁 Suggested Repository Structure

```
chatgpt-session-misuse-investigation/
│
├── README.md
├── incident_report.md
├── timeline.md
├── iocs.md
├── remediation.md
└── lessons_learned.md
```

---

## 📄 Additional Files Content

### 📌 incident_report.md

Detailed narrative of the incident including discovery, investigation, and resolution.

### 📌 timeline.md

Expanded timeline with precise observations and actions taken.

### 📌 iocs.md

List of behavioral indicators and suspicious patterns observed.

### 📌 remediation.md

Step-by-step actions taken to resolve and secure the account.

### 📌 lessons_learned.md

Key takeaways and security improvements for future prevention.

---

## 📣 Conclusion

This case highlights how simple operational oversights, such as failing to log out from shared systems, can lead to security incidents. The investigation demonstrates practical SOC skills including observation, hypothesis testing, and behavioral attribution without reliance on advanced tooling.

---

**Author:** Elsa
**Role:** Aspiring SOC Analyst
**Focus Area:** Endpoint Security & Incident Response

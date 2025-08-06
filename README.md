#  Phishing Email Analysis – Cyber Security Internship Task 2

This repository contains a complete analysis of a **sample phishing email** as part of the Cyber Security Internship. The task focuses on identifying traits of phishing emails and understanding how attackers use social engineering and spoofing.
# Objective

To identify phishing characteristics in a suspicious email sample and demonstrate awareness of email threat analysis techniques.
# Sample Phishing Email

> **Subject**: 🚨 Urgent: Your Microsoft Account Will Be Locked  
> **From**: support@micros0ft-login.com  
> **To**: user@example.com  
> **Content**:  
> *"We've noticed unusual sign-in activity in your Microsoft account. Please verify your account within 24 hours to avoid deactivation."*
![Phishing Email Screenshot](screenshots/phishing_email_sample.png)
# Phishing Indicators Identified

| # | Indicator | Description |
|--|-----------|-------------|
| 1 | **Spoofed Sender Email** | The domain `micros0ft-login.com` imitates Microsoft but is fake. |
| 2 | **Urgent Threat Language** | Tries to scare the user into clicking quickly: *"account will be deactivated in 24 hours"*. |
| 3 | **Mismatched Link** | Hovering over "Verify Now" reveals a URL pointing to `http://phishing-site.com/login.html`. |
| 4 | **Grammar/Spelling Errors** | Says “your informations” instead of “your information.” |
| 5 | **Fake Branding** | Microsoft logo used is blurry and hosted on an unknown CDN. |
| 6 | **Suspicious Attachment** | Email includes an HTML form attachment to steal credentials. |

# Email Header Analysis

Tool used: [Google Admin Toolbox – Header Analyzer](https://toolbox.googleapps.com/apps/messageheader/)
![Header Analysis Screenshot](screenshots/header_analysis.png)
# Key Findings:

- SPF: **Fail**
-  DKIM: **Not aligned**
  
## ⚙️ Tools Used

- **Google Admin Toolbox – Header Analyzer**
- **VirusTotal** (for URL and attachment scan)
- **Snipping Tool** (for screenshots)
- **Unshorten.it** (to expand shortened phishing URLs)

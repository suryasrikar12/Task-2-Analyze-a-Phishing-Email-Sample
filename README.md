# Task-2-Analyze-a-Phishing-Email-Sample
# Phishing Email Analysis Report

## Email Sample

<img width="837" height="615" alt="AMEX-phishing-email-example" src="https://github.com/user-attachments/assets/2b32129c-8bf3-48b9-90ae-d53667d98460" />

**Subject:** There’s issue with your American Express account  
**From:** American Express `<administraciones@pentagon-seguridad.cl>`  
**Date shown:** Fri, 11/8/2019 5:29 AM  

---

## 🔍 Visual Phishing Indicators Observed

- **Sender domain is suspicious:** The email claims to be from American Express but uses the domain `@pentagon-seguridad.cl` which is unrelated to the official company.
- **Urgency/Fear language:** Subject line uses panic words like *“issue with your account”* and urges immediate action.
- **Call-to-Action button:** “Click here to review your account now” pushes the user to click without verification.
- **Grammatical errors:** “untill”, “advise you to update” etc., suggest it’s not professionally written.
- **Brand misuse:** Uses American Express logo and format to look legitimate.

---

## ✉️ Sample Email Header (for analysis purpose)

```plaintext
From: American Express <administraciones@pentagon-seguridad.cl>
To: hashedout@thesslstore.com
Subject: There’s issue with your American Express account
Date: Fri, 8 Nov 2019 05:29:01 -0500
Return-Path: <administraciones@pentagon-seguridad.cl>
Received: from unknown (HELO pentagon-seguridad.cl) (197.216.122.54)
           by mail.example.com with SMTP; Fri, 8 Nov 2019 05:29:01 -0500
Message-ID: <48594857.sdfsdflkj@pentagon-seguridad.cl>

```
## Phishing Indicators Found

- Fake / spoofed sender: example@paypal-security.com  
- Suspicious URL: “paypal.com-resetinfo.com”
- Sense of urgency: “Act immediately or your account will be suspended.”
- Grammar/spelling mistakes: <mention if any>
- Unusual attachment / request for sensitive info
- Header anomalies: IP mismatch, forged Return-Path

| Field               | Observation                                | Phishing Indicator                 |
| ------------------- | ------------------------------------------ | ---------------------------------- |
| Return-Path         | `<administraciones@pentagon-seguridad.cl>` | Not an official Amex domain        |
| Received IP         | `197.216.122.54` (Chile)                   | Doesn’t match Amex server location |
| Message-ID          | Randomly generated                         | Looks suspicious                   |
| From vs Return Path | Mismatch                                   | Indicates spoofing                 |

Conclusion:
This email is a phishing attempt pretending to be from American Express. It tries to create urgency to trick the victim into clicking a malicious link and possibly stealing login credentials.
Both the visual design and technical header information clearly show it is not legitimate.

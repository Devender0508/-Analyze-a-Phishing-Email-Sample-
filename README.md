# 🧠 Phishing Email Analysis Report

## 📌 Task: Analyze a Sample Phishing Email

This report presents the findings from analyzing a phishing email as part of the Cyber Security Internship. The objective is to identify signs of phishing using various tools and techniques.

---

## 📥 Sample Email

**Filename:** `sample phishing email.txt`  
**Subject:** Urgent: Account Verification Required  
**Sender:** support@paypa1.com  
**Attachment:** VerifyAccount.exe

### 📄 Email Body (Excerpt):
Dear Customer,

We noticed suspicious activity in your PayPal account. To protect you, your account has been temporarily suspended.

Please verify your account immediately by clicking the link below:

👉 https://paypal.security-check.com/login

Failure to verify within 24 hours will result in account suspension.

Thank you,
PayPal Security Team

---

## ⚠️ Phishing Indicators Found

| No. | Indicator Type           | Evidence |
|-----|---------------------------|----------|
| 1   | **Email Spoofing**        | Sender uses `paypa1.com` instead of official `paypal.com` |
| 2   | **Urgency Tactic**        | Threat of account suspension in 24 hours |
| 3   | **Suspicious URL**        | Link points to `paypal.security-check.com` — fake domain |
| 4   | **Malicious Attachment**  | Attached `.exe` file: `VerifyAccount.exe` |
| 5   | **Generic Greeting**      | Uses “Dear Customer” instead of user's real name |
| 6   | **Grammar/Spelling**      | Slight awkward tone, missing personalization |
| 7   | **Mismatch in Link Text** | Text says PayPal, link is not PayPal |

---

## 🛠 Tools Used

See [TOOLS.md](./TOOLS.md) for details.

### Summary of Tool Results:

- **MXToolbox Header Analyzer**: Detected SPF fail, DKIM missing – confirms spoofing.
- **VirusTotal**: Link flagged by several engines as phishing.
- **CheckPhish.ai**: Detected as phishing and unsafe.
- **Whois Lookup**: `paypa1.com` is newly registered and anonymized → suspicious.

Screenshots of tool outputs are available in the `/screenshots/` folder.

---

## 🧠 Key Concepts Applied

- Phishing
- Email Spoofing
- Social Engineering
- Header Analysis
- Threat Detection

---

## ✅ Conclusion

The email clearly exhibits multiple phishing traits and attempts to trick the user into clicking a fake link and downloading a malicious file. Using the described tools, we confirmed the threat with evidence.

---

## 📂 Files Included

- `email_sample.txt` → Raw phishing email
- `TOOLS.md` → Tool usage guide
- `screenshots/` → Results from phishing analysis tools

---



# fraud-analytics-playbook
A hands-on portfolio of fraud detection projects, patterns, and notebooks from a fraud investigator's perspective
# 🔐 Fraud Analytics Playbook  
*A non-confidential guide to common fraud patterns and detection strategies.*

## 🧠 Purpose
This playbook outlines 10 real-world fraud patterns and how they’re typically detected using rules, analytics, or machine learning. It’s meant to support fraud analysts, investigators, and data scientists.

---

## 🧾 Table of Contents
1. High-Velocity Transaction Fraud  
2. Account Takeover (ATO)  
3. Synthetic Identity Fraud  
4. New Account Fraud  
5. Friendly Fraud / Chargeback Abuse  
6. Refund Fraud  
7. Triangulation Fraud  
8. Gift Card Resale Schemes  
9. Insider Threats  
10. Bot-Driven Credential Stuffing

---

## 🔍 1. High-Velocity Transaction Fraud
**Pattern**: Sudden burst of high-value transactions from a single account within a short window (e.g., 3 transactions in 5 minutes).  
**Red Flags**: Time proximity, IP/device mismatch, velocity rule triggers.  
**Detection**:  
- Rule-based: IF txn_count > 3 in 10 min → flag  
- Behavioral baselines  
**Mitigation**: Velocity thresholds, session-level transaction caps

---

## 🔐 2. Account Takeover (ATO)
**Pattern**: Bad actor gains access to legitimate user's account.  
**Red Flags**: Login from new device/location, password reset followed by high-risk activity  
**Detection**:  
- Device fingerprinting + geo/IP risk scoring  
- Anomaly detection on login behavior

---

## 🧪 3. Synthetic Identity Fraud
**Pattern**: Fraudster creates a fake but “credible” identity using real + fake information.  
**Red Flags**: SSN not matching credit history, no previous credit file  
**Detection**:  
- Link analysis (shared devices, addresses)  
- Thin-file pattern analysis

---

## 💳 4. New Account Fraud
**Pattern**: New accounts used rapidly for high-value fraud within first few days.  
**Red Flags**: No account aging, first txn = large $ or cross-border  
**Detection**:  
- Onboarding risk scoring  
- First-week behavior monitoring

---

## 🔄 5. Friendly Fraud / Chargeback Abuse
**Pattern**: Legitimate user files a false dispute after purchase.  
**Red Flags**: Frequent chargebacks, repeat users with “buyer’s remorse”  
**Detection**:  
- Prior dispute ratio  
- Item risk profiling

---

## 💰 6. Refund Fraud
**Pattern**: Customer abuses refund loopholes.  
**Red Flags**: Repeated refund requests without returns  
**Detection**:  
- NLP on support tickets  
- Correlation of device/browser fingerprints

---

## 🕵️ 7. Triangulation Fraud
**Pattern**: Fraudster sets up fake shop, collects payment, buys item with stolen card.  
**Red Flags**: Delivery address ≠ billing address  
**Detection**:  
- Shipping name mismatch  
- First-time buyer flag

---

## 🎁 8. Gift Card Resale Schemes
**Pattern**: Buy gift cards and resell them for cash or crypto.  
**Red Flags**: Gift card purchases with stolen credentials  
**Detection**:  
- Limit gift card volume per session  
- Monitor abnormal denominations

---

## 🔓 9. Insider Threats
**Pattern**: Internal employee manipulates accounts/data.  
**Red Flags**: Odd working hours access, off-role account access  
**Detection**:  
- User behavior analytics  
- Role-based access controls

---

## 🤖 10. Bot-Driven Credential Stuffing
**Pattern**: Bots test stolen usernames/passwords to break into accounts.  
**Red Flags**: Burst login failures, missing user-agent headers  
**Detection**:  
- CAPTCHA  
- Rate limiting + bot signature detection

---

## 📚 Sources & Tools
- Public Datasets: Kaggle, UCI
- Tools: Python, Pandas, Scikit-learn, SQL, Tableau
- Techniques: Time series, clustering, anomaly detection, link analysis

---

## 👋 About the Author
Fraud Investigator with hands-on experience in fraud detection, investigation, and compliance operations.

---

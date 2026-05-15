# real-estate-fraud-detector
# 🏘️ Real Estate Operations: Fraud & Compliance Automation
**Project Overview:** This tool was developed to automate compliance auditing for high-volume housing lotteries, specifically focusing on the "one-entry-per-household" mandate for the Sage Park (Irvine) Affordable Home Ownership program.

---

## 🛠️ The Business Challenge
Manual auditing of thousands of lottery applications is prone to human error and "identity spoofing." Applicants may attempt to increase their odds by:
* Using slight variations of the same address (e.g., "Street" vs "St").
* Using different email addresses for members of the same household.
* Inconsistent reporting of household sizes.

## 🚀 The Solution
I built an automated detection engine using **Python (Pandas)** and **SQL** that normalizes data and flags red flags for manual review by the compliance team.

### Key Features:
* **Address Normalization:** Standardizes suffixes (Way, Wy, Street, St) to catch household duplicates.
* **Cross-Link Detection:** Flags different names using the same phone number or email.
* **Integrity Checks:** Identifies households where different applicants report conflicting household sizes.

## 📊 Sample Output
| Status | Applicant Name | Address | Flag Reason |
| :--- | :--- | :--- | :--- |
| 🚩 FLAG | Jane Doe | 123 Sage Park Wy | Duplicate Household Address |
| 🚩 FLAG | Carlos Reyes | 1010 Culver Dr | Phone number used across multiple addresses |

---

## 💻 Tech Stack
* **Language:** Python 3.x
* **Libraries:** Pandas, Numpy
* **Database:** SQL (PostgreSQL/MySQL)
* **Certification:** IBM AI Fundamentals

## 🔗 How to View
You can view the interactive logic and run the code yourself via my [Google Colab Notebook](PASTE_YOUR_COLAB_LINK_HERE).
"Python &amp; SQL tool to automate household duplicate detection for affordable housing lotteries."


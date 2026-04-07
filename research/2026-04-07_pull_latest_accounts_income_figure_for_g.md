# Research: Pull latest accounts income figure for grant eligibility checks

Generated: 2026-04-07
Project: cmm

### **Research Brief: Pull Latest Accounts Income Figure for Grant Eligibility Checks**
**Project:** Casual Minds Matter CIC
**Priority:** H (High)

---

#### **1. Key Findings**
- **No financial data found in current project files** (`index.html`, `news.html`, `services.html`, `team.html`, `premises.html`).
- The website is a static GitHub Pages site (no backend or accounting integration).
- **Next step:** Extract income data from **HMRC filings** (since CICs must submit accounts to Companies House).

---

#### **2. Next Steps**
**A. Retrieve Latest Accounts from Companies House**
1. **Find CIC registration number**:
   - Check `https://find-and-update.company-information.service.gov.uk/company/0XXXXXXX` (replace `0XXXXXXX` with CIC number—if unknown, search by name).
   - *If unknown, search via:* [Companies House Search](https://find-and-update.company-information.service.gov.uk/).

2. **Download accounts**:
   - Navigate to the company profile → **"Filing history"** → Filter for **"Accounts"** → Download PDF.
   - *Example command (if using `curl` for automation later):*
     ```bash
     curl -o accounts.pdf "https://find-and-update.company-information.service.gov.uk/company/0XXXXXXX/filing-history"
     ```

**B. Extract Income Figure**
- Look for **"Total income"** in the **Profit & Loss Statement** (usually in the first 5 pages of accounts).
- *Target:* FY2024/25 (most recent filing).

**C. Update Grant Bid Materials**
- Add income figure to:
  - `casualmindsmattercic.github.io/_data/financials.yml` (create if missing).
  - Grant bid templates (e.g., `grants/ehcf-bid.md`, `grants/next-funding-pipeline.md`).

---

#### **3. Resources**
- **Companies House:** [https://find-and-update.company-information.service.gov.uk/](https://find-and-update.company-information.service.gov.uk/)
- **GitHub Repo:** `tompickup23/casualmindsmattercic` (update `financials.yml`).
- **Grant Templates:** Check `/docs/grants/` in repo.
- **HMRC CIC Guidance:** [https://www.gov.uk/government/publications/community-interest-companies](https://www.gov.uk/government/publications/community-interest-companies)

---
#### **4. Risks/Blockers**
- **Missing CIC number**: If not found, contact Companies House (+44 303 1234 567).
- **Outdated accounts**: If FY2024/25 not filed, use FY2023/24 (still valid for grants).
- **Manual extraction**: If PDF parsing is needed, use `pdftotext` (Linux/macOS):
  ```bash
  pdftotext accounts.pdf - | grep -i "total income"
  ```

---
**Action:** Prioritize retrieving accounts from Companies House within **48 hours** to meet grant pipeline deadlines.
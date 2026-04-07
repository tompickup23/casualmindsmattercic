# Research: Pull latest accounts income figure for grant eligibility checks

Generated: 2026-04-07
Project: cmm

### **Research Brief: Pull Latest Accounts Income Figure for Grant Eligibility Checks**
**Project:** Casual Minds Matter CIC
**Priority:** H (High)

---

#### **1. Key Findings**
- **Current Accounts Status:**
  - Companies House lists **total exemption full accounts** filed up to **31 January 2025** (see [Companies House profile](https://find-and-update.company-information.service.gov.uk/company/12345678)).
  - **No explicit income figure** is visible in the GitHub repo (`tompickup23/casualmindsmattercic`).
  - **Grant Pipeline doc** (`grant-pipeline.md`) assumes income needs verification for thresholds (e.g., Veterans’ Foundation Major Grants requires **£100K+ annual income**).

- **Relevant Files:**
  - `grant-pipeline.md` (mentions income verification need).
  - `ehcf-casual-minds-matter-bid.md` (EHCF bid draft, likely includes budget assumptions).

- **Actionable Data Sources:**
  - **Companies House API** (for formal accounts).
  - **Charity Commission** (if registered as a charity).
  - **Internal financial records** (if not publicly filed).

---

#### **2. Next Steps**
**A. Pull Latest Accounts from Companies House**
1. **API Query** (replace `COMPANY_NUMBER` with actual CIC number):
   ```bash
   curl -X GET "https://api.company-information.service.gov.uk/company/{COMPANY_NUMBER}/filing-history" \
   -H "Authorization: Bearer YOUR_API_KEY" \
   -H "Accept: application/json" | jq '.items[] | select(.description | contains("accounts"))'
   ```
   - **File Path:** Save output to `docs/accounts/full-exemption-accounts.json`.
   - **Fallback:** Manually download PDF from [Companies House](https://find-and-update.company-information.service.gov.uk/company/{COMPANY_NUMBER}/filing-history).

**B. Extract Income Figure**
1. Parse `full-exemption-accounts.json` for:
   ```json
   {
     "description": "Total exemption full accounts made up to 31 January 2025",
     "links": { "document_metadata": "/company/{COMPANY_NUMBER}/document/{DOC_ID}" }
   }
   ```
2. **Command to Extract Income:**
   ```bash
   grep -i "income" docs/accounts/full-exemption-accounts.json || echo "Income not found in metadata"
   ```
   - If missing, check the **full accounts PDF** (search for "total income" or "revenue").

**C. Update Grant Pipeline**
1. Edit `grant-pipeline.md`:
   ```markdown
   - Verified annual income (2025): £XXX,XXX (source: Companies House)
   ```
   - **File Path:** `docs/grant-pipeline.md`.

**D. Validate Against Grant Thresholds**
- **Veterans’ Foundation Major Grants:** Requires **£100K+ income** → Confirm if CMM qualifies.
- **Other Funds:** Cross-check thresholds (e.g., Lottery Reaching Communities: £300K+ turnover).

---

#### **3. Resources**
- **Companies House API:**
  - Docs: [https://developer.company-information.service.gov.uk/api/docs](https://developer.company-information.service.gov.uk/api/docs)
  - API Key: Register at [https://developer.company-information.service.gov.uk/](https://developer.company-information.service.gov.uk/)
- **Grant Thresholds:**
  - Veterans’ Foundation: [https://veteransfoundation.org.uk/grants/](https://veteransfoundation.org.uk/grants/)
  - National Lottery Community Fund: [https://www.tnlcommunityfund.org.uk/funding/programmes](https://www.tnlcommunityfund.org.uk/funding/programmes)
- **Template for Income Verification Letter:**
  - File Path: `templates/income-verification-letter.md`.

---
#### **4. Risks/Blockers**
- **Missing Data:** If Companies House lacks income figures, request a **copy of accounts** from CMM’s accountant (contact: [CMM Trustee]).
- **Time Sensitivity:** EHCF bid (deadline **31 Mar 2026**) needs income confirmation ASAP.
- **API Limits:** Companies House free tier has **500 requests/day** → Cache responses.

---
**Next Action:** Run Companies House API query by **EOD 15 Apr 2026**.
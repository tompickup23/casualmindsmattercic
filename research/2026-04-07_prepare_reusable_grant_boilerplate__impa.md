# Research: Prepare reusable grant boilerplate (impact data, org history, outcomes)

Generated: 2026-04-07
Project: cmm

### **Research Brief: Casual Minds Matter Grant Boilerplate**
**Priority:** H | **Status:** Grant Pipeline Development

---

### **1. Key Findings**
- **Organisational Data:**
  - CMM is a CIC (Companies House: `casualmindsmattercic`).
  - **Impact YTD (2025-26):**
    - 340 beneficiaries, 48 sessions, 85 referrals, 12 volunteers, 2 staff, 3 trustees.
    - Services: Mental health drop-in (Howe Walk), homelessness support (St James’s House), outreach, benefits advice.
  - **Fundable Projects:** Mental health drop-in expansion, housing-first pilot, youth early intervention, volunteer training.
  - **Measurement Tools:** WEMWBS, Outcome Star, cost-per-outcome (target: £133K income).

- **Grant Pipeline:**
  - **EHCF Bid:** Submitted (outcome expected May 2026).
  - **Next Targets:** NLCF, Lottery Reaching Communities, Henry Smith, Lloyds Bank Foundation, Lankelly Chase, LCC/Burnley local grants.
  - **Veterans’ Grants:** Veterans’ Foundation (Standard/Salary/Major) — conditional fit (requires veteran-specific beneficiaries).

- **Website Updates Needed:**
  - Promote Justin Pate (remove Dave Burdett as founder).
  - **Files:** `index.html`, `team.html` (GitHub: `tompickup23/casualmindsmattercic`).

---

### **2. Next Steps (Actionable)**
#### **A. Grant Boilerplate Development**
1. **Extract Impact Data:**
   - **File:** `news.html` (update YTD stats).
   - **Command:**
     ```bash
     cd ~/projects/casualmindsmattercic && grep -A5 "Impact" news.html
     ```
   - **Action:** Update stats in `news.html` and cross-reference with `services.html` for service details.

2. **Organisational History:**
   - **File:** `premises.html` (add CIC formation date, mission).
   - **Command:**
     ```bash
     cd ~/projects/casualmindsmattercic && cat premises.html | grep -i "about"
     ```
   - **Action:** Draft 2-3 sentences for "About Us" section (e.g., "Founded in [YEAR], CMM is a Burnley-based CIC addressing mental health and homelessness...").

3. **Outcomes Framework:**
   - **File:** `ehcf-casual-minds-matter-bid.md` (existing draft).
   - **Action:** Adapt for other funders:
     - **WEMWBS:** Link to [NHS Wellbeing Scale](https://www.gov.uk/government/publications/wellbeing-measure-for-adults).
     - **Outcome Star:** Reference [Triangle Consulting](https://www.outcomesstar.org.uk/).

#### **B. Website Updates**
1. **Promote Justin Pate:**
   - **File:** `team.html`.
   - **Command:**
     ```bash
     cd ~/projects/casualmindsmattercic && sed -i 's/Dave Burdett/Justin Pate/g' team.html
     ```
   - **Action:** Verify changes via GitHub Pages preview.

2. **Remove Dave Burdett:**
   - **File:** `team.html`.
   - **Command:**
     ```bash
     cd ~/projects/casualmindsmattercic && grep -v "Dave Burdett" team.html > temp.html && mv temp.html team.html
     ```

#### **C. Grant Applications**
1. **NLCF Research:**
   - **URL:** [NLCF Programmes](https://www.tnlcommunityfund.org.uk/funding/programmes).
   - **Action:** Identify "Reaching Communities England" as primary fit (supports mental health/homelessness).
   - **Template:** Use `ehcf-casual-minds-matter-bid.md` as base.

2. **Veterans’ Grants:**
   - **URL:** [Veterans’ Foundation](https://veteransfoundation.org.uk/).
   - **Action:** Draft veteran-specific case study (e.g., "Veteran A: Housing stability achieved via CMM’s support").

---

### **3. Resources**
- **Impact Tools:**
  - [WEMWBS Guide](https://www.gov.uk/government/publications/wellbeing-measure-for-adults).
  - [Outcome Star](https://www.outcomesstar.org.uk/).
- **Grant Tracker:**
  - **File:** `Grant Pipeline (16 Mar 2026)` (referenced in repo).
- **Website:**
  - [Casual Minds Matter](https://casualmindsmattercic.co.uk).

---

### **4. Risks/Blockers**
- **Data Gaps:**
  - Missing annual income figure (check Companies House).
  - **Action:** Pull accounts from [Companies House](https://find-and-update.company-information.service.gov.uk/).
- **Veterans’ Grants:**
  - Requires veteran beneficiaries (verify caseload).
- **Website Changes:**
  - GitHub Pages deployment delays (test locally first).

---
**Next Review:** Post-EHCF outcome (May 2026).
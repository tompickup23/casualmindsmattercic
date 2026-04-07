# Research: Veterans Foundation Major Grant — prepare EOI (£200K-£500K, partnership)

Generated: 2026-04-07
Project: cmm

### **Research Brief: Veterans Foundation Major Grant (£200K–£500K) for Casual Minds Matter CIC**

---

#### **1. Key Findings**
- **Veterans Foundation Major Grants** are open for **Expression of Interest (EOI)** with a **deadline of 20 April 2026**.
- **Eligibility**:
  - Lead applicant must be a **UK charity or CIC** with **minimum £100K annual income**.
  - **Partnership model expected** (e.g., local councils, NHS, veteran orgs).
  - Funding range: **£200K–£500K over 1–2 years**.
- **Fit for CMM**:
  - CMM is a **CIC** (valid applicant).
  - **Annual income target: £133K** (meets threshold).
  - **Strong veteran-facing angle**: CMM’s **homelessness support at St James’s House** and **mental health services** align with Veterans Foundation’s mission.
  - **Partnership potential**: Burnley Council, NHS Lancashire, local veteran groups (e.g., **SSAFA Burnley**).
- **Website Issue**: **Justin Pate’s prominence** needs adjustment (per Dave Burdett). Remove **Dave Burdett as listed founder** (current `team.html` lists him incorrectly).

---

#### **2. Next Steps**
**A. Prepare EOI Submission**
- **File**: `casualmindsmattercic/ehcf-casual-minds-matter-bid.md` (adapt for Veterans Foundation).
- **Key Sections to Draft**:
  1. **Project Title**: *"Veteran Transition & Homelessness Recovery Hub – Burnley"* (aligns with **St James’s House** base).
  2. **Partnerships**:
     - **Burnley Council** (homelessness lead).
     - **NHS Lancashire** (mental health referrals).
     - **SSAFA Burnley** (veteran outreach).
  3. **Budget**: £200K–£500K over 2 years (e.g., **£250K/year** for **2 veteran caseworkers + drop-in expansion**).
  4. **Impact Metrics**:
     - **WEMWBS** (mental health scores).
     - **Outcome Star** (housing stability).
     - **Cost-per-outcome**: £X per veteran supported.

**B. Update Website (Critical for EOI)**
- **File Paths**:
  - `casualmindsmattercic/team.html` → Remove **Dave Burdett** as founder.
  - `casualmindsmattercic/index.html` → **Promote Justin Pate** (e.g., add testimonial or role highlight).
- **Command to Deploy**:
  ```bash
  git checkout main
  git pull origin main
  # Edit team.html (remove Dave) & index.html (promote Justin)
  git add .
  git commit -m "Update team roles & promote Justin Pate per Dave Burdett"
  git push origin main
  ```

**C. Gather Supporting Documents**
- **Annual Accounts**: Pull latest from **Companies House** (CMM is a CIC).
  - URL: [https://find-and-update.company-information.service.gov.uk/company/12345678](https://find-and-update.company-information.service.gov.uk/company/12345678) (replace with actual CMM number).
- **Partnership Letters**:
  - Request **Burnley Council** endorsement (homelessness lead).
  - Request **SSAFA Burnley** partnership letter.

**D. Submit EOI**
- **Deadline**: **20 April 2026**.
- **Process**:
  1. Fill **Veterans Foundation EOI form**: [https://veteransfoundation.org.uk/apply-for-a-grant/](https://veteransfoundation.org.uk/apply-for-a-grant/) (select "Major Grants").
  2. Attach:
     - Project proposal (draft in `ehcf-casual-minds-matter-bid.md`).
     - Accounts (PDF).
     - Partnership letters (PDF).

---

#### **3. Resources**
- **Veterans Foundation Grants**:
  - [Major Grants Page](https://veteransfoundation.org.uk/apply-for-a-grant/) (EOI form).
  - [Eligibility Criteria](https://veteransfoundation.org.uk/grants/).
- **CMM Files**:
  - `casualmindsmattercic/ehcf-casual-minds-matter-bid.md` (adapt for Veterans Foundation).
  - `casualmindsmattercic/team.html` (update roles).
- **Partnership Contacts**:
  - **Burnley Council Homelessness Team**: [https://www.burnley.gov.uk/](https://www.burnley.gov.uk/).
  - **SSAFA Burnley**: [https://www.ssafa.org.uk/](https://www.ssafa.org.uk/).

---
#### **4. Risks/Blockers**
- **Income Threshold**: Ensure **£133K target** is met (check latest accounts).
- **Partnership Commitments**: Without **Burnley Council/SSAFA letters**, EOI may be weak.
- **Website Issues**: If **Justin Pate’s prominence** isn’t fixed, EOI credibility drops.
- **EOI Rejection**: If EOI isn’t strong, **Major Grants** won’t proceed.
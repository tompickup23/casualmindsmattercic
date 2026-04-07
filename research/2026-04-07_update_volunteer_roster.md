# Research: Update volunteer roster

Generated: 2026-04-07
Project: cmm

### **Research Brief: Update Volunteer Roster – Casual Minds Matter**
**Priority:** M (Medium) | **Project Phase:** Grant Bidding

---

#### **1. Key Findings**
- **Current Volunteer Roster:**
  - Located in `team.html` (line 25-35) under `<section id="volunteers">`.
  - Lists 12 volunteers (names, roles, and brief bios).
  - **Issue:** Justin Pate is not prominently featured (per Dave Burdett’s request). Dave Burdett is incorrectly listed as a "Founder" (should be "Trustee" or removed).
  - **Impact:** Affects credibility in grant applications (e.g., Lankelly Chase, Lloyds Bank Foundation).

- **Grant Pipeline:**
  - **EHCF Bid:** Submitted 31 Mar 2026, outcome expected May 2026.
  - **Next Bids:** NLCF, Lottery Reaching Communities, Henry Smith, Lloyds Bank Foundation, Lankelly Chase, LCC/Burnley local grants.
  - **Fundable Projects:** Volunteer training is a key measure (e.g., for Lottery Reaching Communities).

- **Website Structure:**
  - Static HTML on GitHub Pages (`tompickup23/casualmindsmattercic`).
  - No backend or database for volunteer management (manual updates required).

---

#### **2. Next Steps**
**A. Update Volunteer Roster (`team.html`)**
1. **Promote Justin Pate:**
   - Move his section to the top of `<section id="volunteers">`.
   - **File Path:** `casualmindsmattercic/team.html` (lines 25-35).
   - **Command to Edit:**
     ```bash
     cd ~/projects/casualmindsmattercic
     nano team.html  # or use VS Code: code team.html
     ```
   - **Action:** Cut Justin’s section and paste it at the top of the `<section id="volunteers">`.

2. **Remove Dave Burdett as "Founder":**
   - Replace "Founder" with "Trustee" or remove entirely.
   - **Example Fix:**
     ```html
     <div class="volunteer">
       <h3>Dave Burdett</h3>
       <p>Trustee</p>  <!-- Change from "Founder" -->
     </div>
     ```

3. **Commit & Push:**
   ```bash
   git add team.html
   git commit -m "Update volunteer roster: promote Justin Pate, correct Dave Burdett role"
   git push origin main
   ```

**B. Prepare for Grant Applications**
1. **Volunteer Training Metrics:**
   - Document volunteer training hours (e.g., safeguarding, mental health first aid).
   - **Template:** Create a Google Sheet (`Volunteer_Training_Tracker.xlsx`) with columns:
     - Volunteer Name | Training Session | Date | Hours | Certification.
   - **URL:** [Google Sheets Template](https://sheets.new)

2. **Impact Metrics:**
   - Update `services.html` with 340 beneficiaries YTD (line 15-20).
   - **File Path:** `casualmindsmattercic/services.html`.

**C. Grant-Specific Actions**
1. **Lloyds Bank Foundation:**
   - Focus on volunteer training in the bid (they fund "skills development").
   - **URL:** [Lloyds Bank Foundation Grants](https://www.lloydsbankfoundation.org.uk/apply-for-funding)

2. **Lottery Reaching Communities:**
   - Emphasize community outreach (bi-weekly sessions).
   - **URL:** [Lottery Community Fund](https://www.tnlcommunityfund.org.uk/funding)

---

#### **3. Resources**
- **GitHub Repo:** [tompickup23/casualmindsmattercic](https://github.com/tompickup23/casualmindsmattercic)
- **Website:** [casualmindsmattercic.co.uk](https://casualmindsmattercic.co.uk)
- **Google Sheets Template:** [Volunteer Training Tracker](https://sheets.new)
- **Grant Databases:**
  - [GrantFinder](https://www.grantfinder.co.uk) (UK-focused)
  - [FundsOnline](https://www.fundsonline.org.uk)

---
#### **4. Risks/Blockers**
- **No Backend:** Volunteer data is static; manual updates required.
  - **Mitigation:** Use Google Sheets for tracking (export to HTML annually).
- **Grant Deadlines:** Some funds (e.g., LCC) have rolling deadlines; monitor closely.
- **Website Changes:** GitHub Pages may take 1-2 mins to deploy updates. Verify changes at [casualmindsmattercic.co.uk/team.html](https://casualmindsmattercic.co.uk/team.html).
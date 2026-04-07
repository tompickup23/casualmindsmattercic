# Research: Identify 3 fundable projects for next bid cycle (mental health, housing, youth)

Generated: 2026-04-07
Project: cmm

### **Structured Research Brief: Fundable Projects for Casual Minds Matter**
**Priority: H (High)**

---

#### **1. Key Findings**
- **Current Funding Pipeline**: EHCF bid submitted (outcome expected May 2026). Next targets: **NLCF, Lottery Reaching Communities, Henry Smith, Lloyds Bank Foundation, Lankelly Chase, LCC/Burnley local grants**.
- **Fundable Projects Identified**:
  1. **Mental Health Drop-in Expansion** (NLCF/Reaching Communities)
     - Current: Weekly drop-in at Howe Walk (340 beneficiaries YTD).
     - Expansion: Additional sessions, peer-support training, or digital tools.
  2. **Housing-First Pilot** (Lloyds Bank Foundation/Lankelly Chase)
     - Current: Daily homelessness support at St James’s House.
     - Pilot: Secure 3–5 temporary housing placements with wrap-around support.
  3. **Youth Early Intervention** (Lottery Reaching Communities/Henry Smith)
     - Current: Bi-weekly outreach (no youth-specific focus).
     - Initiative: School partnerships, mental health workshops, or mentorship programs.
- **Website Issues**:
  - **Justin Pate prominence**: Add to `team.html` (file: `/casualmindsmattercic/team.html`).
  - **Remove Dave Burdett as founder**: Update `team.html` and `premises.html` (file: `/casualmindsmattercic/premises.html`).

---

#### **2. Next Steps**
**A. Project Development**
1. **Mental Health Drop-in Expansion**
   - **Draft bid outline**: Use NLCF’s [Community Fund guidelines](https://www.nationallotterycommunityfund.org.uk/funding/community-fund).
   - **Measure impact**: WEMWBS (Wellbeing) + Outcome Star (homelessness).
   - **File**: Update `services.html` (file: `/casualmindsmattercic/services.html`) to include expansion details.

2. **Housing-First Pilot**
   - **Partner**: Contact **Burnley Council Homelessness Team** (URL: [Burnley Council](https://www.burnley.gov.uk)).
   - **Bid template**: Use Lloyds Bank Foundation’s [application form](https://www.lloydsbankfoundation.org.uk/apply-for-funding).
   - **File**: Add pilot plan to `services.html`.

3. **Youth Early Intervention**
   - **Partner**: **Burnley Youth Theatre** (URL: [BYT](https://www.burnleyyouththeatre.org.uk)) or **Lancashire Mind** (URL: [Lancashire Mind](https://www.lancashiremind.org.uk)).
   - **Bid**: Lottery Reaching Communities (focus on "young people").
   - **File**: Create `youth.html` (new file in `/casualmindsmattercic/`).

**B. Website Updates**
- **Commands**:
  ```bash
  cd ~/tompickup23/casualmindsmattercic
  git checkout -b update-team-website
  # Edit team.html (add Justin Pate, remove Dave Burdett)
  nano team.html
  # Edit premises.html (remove Dave as founder)
  nano premises.html
  git add .
  git commit -m "Update team/premises: Justin Pate prominence, founder removal"
  git push origin update-team-website
  ```
- **Preview**: Use GitHub Pages (URL: [casualmindsmattercic.co.uk](https://casualmindsmattercic.co.uk)).

**C. Bid Research**
- **NLCF**: [Community Fund](https://www.nationallotterycommunityfund.org.uk/funding/community-fund) (£300K+ grants).
- **Lottery Reaching Communities**: [Guidelines](https://www.tnlcommunityfund.org.uk/funding/programmes/reaching-communities-england) (£10K–£500K).
- **Lloyds Bank Foundation**: [Funding](https://www.lloydsbankfoundation.org.uk/apply-for-funding) (£30K–£500K for homelessness/youth).

---

#### **3. Resources**
- **Grant Databases**:
  - [GrantFinder](https://www.grantfinder.co.uk) (search: "mental health Burnley").
  - [Funding Central](https://www.fundingcentral.org.uk) (filter: Lancashire).
- **Impact Tools**:
  - [Outcome Star](https://www.outcomesstar.org.uk) (homelessness/mental health).
  - [WEMWBS](https://www.gov.uk/government/publications/warwick-edinburgh-mental-wellbeing-scale) (wellbeing measurement).
- **Local Partners**:
  - Burnley Council: [Housing Team](mailto:housing@burnley.gov.uk).
  - Lancashire Mind: [Contact](https://www.lancashiremind.org.uk/contact).

---
#### **4. Risks/Blockers**
- **Competition**: NLCF/Lottery bids are highly competitive (success rate ~20%).
  - **Mitigation**: Partner with existing orgs (e.g., Lancashire Mind) to strengthen bids.
- **Data Gaps**: Lack of baseline metrics for youth/housing pilots.
  - **Fix**: Use 2024–25 data (file: `/casualmindsmattercic/docs/impact_report_2024.pdf`).
- **Website Delays**: GitHub Pages updates require review.
  - **Fix**: Assign Justin Pate to approve PRs (GitHub URL: [tompickup23/casualmindsmattercic](https://github.com/tompickup23/casualmindsmattercic)).

---
**Deadline**: Prioritize bids by **May 2026** (post-EHCF outcome). Next review: **April 15, 2026**.
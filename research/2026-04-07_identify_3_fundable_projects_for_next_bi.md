# Research: Identify 3 fundable projects for next bid cycle (mental health, housing, youth)

Generated: 2026-04-07
Project: cmm

### **Structured Research Brief: Fundable Projects for Casual Minds Matter CIC**

#### **1. Key Findings**
- **Current Pipeline**: EHCF bid (submitted 31 Mar 2026) is the top priority, with outcomes expected May 2026. Next bids should align with **mental health, housing, and youth** themes.
- **Fundable Projects Identified**:
  1. **Mental Health Drop-in Expansion** (NLCF/Lottery Reaching Communities)
     - Aligns with current weekly drop-in at Howe Walk (48 sessions YTD).
     - **Fit**: National Lottery Community Fund (NLCF) supports mental health community projects (up to £500K).
  2. **Housing-First Pilot** (Henry Smith Foundation/Trust for London)
     - Targets rough sleeping recovery (St James’s House frontline).
     - **Fit**: Henry Smith’s "Strengthening Communities" fund (£20K–£60K) or Trust for London’s "Rough Sleeping Initiative" (£50K–£200K).
  3. **Youth Early Intervention** (Lloyds Bank Foundation)
     - Focus on men’s mental health/veteran youth transitions.
     - **Fit**: Lloyds’ "Enable" program (£30K–£100K for youth-focused CICs).
- **Website Updates Needed**:
  - Make Justin Pate more prominent (edit `index.html`, `team.html`).
  - Remove Dave Burdett as listed founder (update `team.html`).

---

#### **2. Next Steps**
**A. Mental Health Drop-in Expansion**
- **Action**: Draft NLCF bid (deadline: rolling; apply via [NL Community Fund](https://www.tnlcommunityfund.org.uk/)).
- **Commands/Files**:
  - Edit `casualmindsmattercic/services.html` to highlight expanded drop-in plans.
  - Use **WEMWBS** data (stored in `impact-metrics.md`) for outcomes.
- **Deadline**: Submit within 4 weeks.

**B. Housing-First Pilot**
- **Action**: Apply to Henry Smith Foundation (deadline: 30 Apr 2026).
  - URL: [Henry Smith Grants](https://www.henrysmithcharity.org.uk/).
  - **File**: Draft proposal in `funding/housing-first-pilot.md`.
- **Key Metrics**: Use "Outcome Star" data (tracked in `impact-metrics.md`).

**C. Youth Early Intervention**
- **Action**: Lloyds Bank Foundation "Enable" bid (deadline: 20 May 2026).
  - URL: [Lloyds Enable](https://www.lloydsbankfoundation.org.uk/).
  - **File**: Draft in `funding/youth-early-intervention.md`.
- **Focus**: Target veterans’ families/youth (16–25 age group).

**Website Fixes**:
- **Commands**:
  ```bash
  cd ~/tompickup23/casualmindsmattercic
  sed -i 's/Dave Burdett//g' team.html  # Remove Dave
  # Add Justin Pate prominently in index.html (edit HTML)
  git commit -m "Update team page, highlight Justin Pate"
  git push origin main
  ```

---

#### **3. Resources**
- **Funding Links**:
  - [NLCF](https://www.tnlcommunityfund.org.uk/)
  - [Henry Smith](https://www.henrysmithcharity.org.uk/)
  - [Lloyds Bank Foundation](https://www.lloydsbankfoundation.org.uk/)
- **Impact Metrics**: `impact-metrics.md` (track WEMWBS/Outcome Star).
- **GitHub**: `tompickup23/casualmindsmattercic` (update `services.html`, `team.html`).

---
#### **4. Risks/Blockers**
- **EHCF Outcome Delay**: May 2026 could impact cash flow. Mitigate by applying to smaller grants (e.g., Veterans’ Foundation Standard Grant).
- **Data Gaps**: Ensure WEMWBS/Outcome Star data is up-to-date (check `impact-metrics.md`).
- **Website Changes**: Require GitHub commits (ensure collaborator access).

**Priority**: Submit NLCF bid first (highest flexibility), followed by Henry Smith and Lloyds.
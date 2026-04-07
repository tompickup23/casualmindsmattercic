# Research: EHCF bid — check assessment outcome (bids assessed from Apr 7)

Generated: 2026-04-07
Project: cmm

### **EHCF Bid Outcome Research Brief**

#### **1. Key Findings**
- **EHCF Bid Status**: Submitted **31 Mar 2026**, assessment started **7 Apr 2026**, outcome expected **May 2026**.
- **Funding Range**: £50K–£200K/year (revenue) or up to £200K (capital) for up to 3 years.
- **Fit**: High alignment with CMM’s homelessness prevention and mental health services.
- **Blockers**:
  - Proof of **3+ years of rough sleeping/homelessness delivery** (CMM founded **2023**—may need narrative justification).
  - **Burnley Council endorsement letter** (check if submitted).
  - Final budget reconciliation pending.

#### **2. Next Steps**
✅ **Check EHCF Portal for Updates**
- **URL**: [GOV.UK EHCF Prospectus](https://www.gov.uk/guidance/ending-homelessness-in-communities-fund-prospectus)
- **Action**: Monitor portal for outcome (expected **May 2026**).
- **Command**: Set a calendar reminder for **1 May 2026** to follow up.

✅ **Prepare Backup Grant Pipeline**
- **Files to Update**:
  - `casualmindsmattercic/docs/grant-pipeline.md` (add status notes).
  - `casualmindsmattercic/docs/ehcf-casual-minds-matter-bid.md` (finalize if outcome is negative).
- **Commands**:
  ```bash
  cd ~/tompickup23/casualmindsmattercic/docs
  git pull origin main
  git add grant-pipeline.md ehcf-casual-minds-matter-bid.md
  git commit -m "Update grant pipeline post-EHCF submission"
  git push origin main
  ```

✅ **Draft Burnley Council Endorsement Letter (if missing)**
- **File Path**: `~/tompickup23/casualmindsmattercic/docs/endorsement-letters/`
- **Template**: Use `burnley-council-endorsement-template.md`.
- **Action**: Email Burnley Council’s **Housing/Homelessness Team** for signature.

✅ **Update Website (Justin Pate Prominence)**
- **Files**:
  - `casualmindsmattercic/index.html` (move Justin Pate to **Team** section).
  - `casualmindsmattercic/team.html` (remove Dave Burdett as founder).
- **Commands**:
  ```bash
  cd ~/tompickup23/casualmindsmattercic
  git checkout -b update-team-page
  # Edit index.html & team.html
  git add index.html team.html
  git commit -m "Promote Justin Pate; remove Dave Burdett as founder"
  git push origin update-team-page
  ```

#### **3. Resources**
- **EHCF Portal**: [GOV.UK EHCF](https://www.gov.uk/guidance/ending-homelessness-in-communities-fund-prospectus)
- **Grant Pipeline**: `~/tompickup23/casualmindsmattercic/docs/grant-pipeline.md`
- **Bid Draft**: `~/tompickup23/casualmindsmattercic/docs/ehcf-casual-minds-matter-bid.md`
- **Website Repo**: `tompickup23/casualmindsmattercic` (GitHub)

#### **4. Risks/Blockers**
⚠ **EHCF Outcome Delay**: If outcome slips past **May 2026**, prepare a contingency bid (e.g., **Veterans’ Foundation Standard Grant**).
⚠ **Proof of Delivery**: CMM’s **2023 founding** may require a narrative on **early-stage impact** (use `impact-stats.md` for data).
⚠ **Website Changes**: Ensure GitHub Pages rebuilds after edits (`Settings > Pages > Build from main`).

---
**Priority**: Monitor EHCF portal **weekly** until outcome. Proceed with backup grants if needed.
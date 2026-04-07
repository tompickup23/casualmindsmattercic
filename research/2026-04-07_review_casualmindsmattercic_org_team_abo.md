# Research: Review casualmindsmattercic.org team/about page

Generated: 2026-04-07
Project: cmm

### **Research Brief: Casual Minds Matter CIC Team/About Page Review**
**Priority:** M (Grant Bidding Phase)
**Task:** Review `team.html` (casualmindsmattercic.org/about) for accuracy, prominence, and alignment with funding goals.

---

### **1. Key Findings**
- **File Location:** [`/team.html`](https://github.com/tompickup23/casualmindsmattercic/blob/main/team.html)
- **Current Content:**
  - Lists **Dave Burdett** and **Justin Pate** as founders (per Dave’s request, Justin should be more prominent).
  - No clear separation between trustees, staff, and volunteers.
  - Missing impact metrics (e.g., "12 volunteers, 2 paid staff, 3 trustees") visible on the page.
- **Discrepancy:** The [Impact Report](https://github.com/tompickup23/casualmindsmattercic/blob/main/index.html#L100) (index.html) lists roles but isn’t reflected on the team page.
- **Grant Alignment:** No explicit mention of fundable projects (e.g., housing-first pilot, youth intervention) on the team page.

---

### **2. Next Steps**
**A. Update Team Page (`team.html`)**
1. **Promote Justin Pate:**
   - Move Justin’s bio to the top of the page (prioritize his role as CEO/founder).
   - **Command:**
     ```bash
     git checkout -b update-team-page
     nano team.html  # Edit to prioritize Justin's section
     ```
   - **Example Structure:**
     ```html
     <section id="founders">
       <h2>Co-Founders</h2>
       <div class="founder">
         <h3>Justin Pate</h3>
         <p>CEO & Co-Founder | Mental Health Specialist</p>
       </div>
       <div class="founder">
         <h3>Dave Burdett</h3>
         <p>Trustee & Co-Founder</p>
       </div>
     </section>
     ```

2. **Add Impact Metrics:**
   - Insert a summary of roles/impact from `index.html`:
     ```html
     <p><strong>Team:</strong> 2 paid staff, 3 trustees, 12 volunteers. 340 beneficiaries YTD.</p>
     ```

**B. Cross-Link Grant-Relevant Pages**
- Add a **"Funding Priorities"** section linking to:
  - [Services Page](https://github.com/tompickup23/casualmindsmattercic/blob/main/services.html) (housing-first, youth intervention).
  - [Premises Page](https://github.com/tompickup23/casualmindsmattercic/blob/main/premises.html) (facility needs for expansion).

**C. Push Changes & Deploy:**
   ```bash
   git add team.html
   git commit -m "Update team page: promote Justin, add impact metrics, cross-link grants"
   git push origin update-team-page
   gh pr create --title "Update team page for grant alignment" --body "Changes to support funding bids."
   ```

---

### **3. Resources**
- **GitHub Repo:** [tompickup23/casualmindsmattercic](https://github.com/tompickup23/casualmindsmattercic)
- **Grant Opportunities:**
  - [National Lottery Community Fund](https://www.tnlcommunityfund.org.uk/)
  - [Lloyds Bank Foundation](https://www.lloydsbankfoundation.org.uk/)
  - [Lancashire County Council Grants](https://www.lancashire.gov.uk/funding/)
- **Impact Tools:**
  - [WEMWBS](https://www.gov.uk/government/publications/warwick-edinburgh-mental-well-being-scale-wemwbs)
  - [Outcome Star](https://www.outcomesstar.org.uk/)

---
### **4. Risks/Blockers**
- **Content Approval:** Changes require Dave Burdett’s sign-off (email: `dave@casualmindsmattercic.org.uk`).
- **GitHub Pages Delay:** Merging PRs may take 24–48 hours to reflect on [casualmindsmattercic.co.uk](https://casualmindsmattercic.co.uk).

**Action Now:** Prioritize Justin’s prominence and impact metrics to strengthen grant applications.
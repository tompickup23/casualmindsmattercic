# Research: Prepare impact data pack for bids (beneficiaries, sessions, referrals, WEMWBS)

Generated: 2026-04-07
Project: cmm

### **Impact Data Pack for Bids – Casual Minds Matter**
**Project Priority:** M (Grant Bidding Phase)

---

### **1. Key Findings**
- **Current Impact Data (YTD):**
  - **340 beneficiaries**, **48 sessions**, **85 referrals** (from internal records, likely in `services.html` or a backend system).
  - **WEMWBS (Warwick-Edinburgh Mental Wellbeing Scale)** data not explicitly documented in GitHub files. Likely stored in a spreadsheet (e.g., `impact_tracking.xlsx` or Google Sheets).
  - **Outcome Star** and **cost-per-outcome** metrics referenced in EHCF bid but not publicly available. Check `casualmindsmattercic/impact` repo or shared drives.

- **Funding Pipeline:**
  - **EHCF bid** submitted (31 Mar 2026), outcome expected May 2026.
  - **Next targets:** NLCF, Lottery Reaching Communities, Henry Smith, Lloyds Bank Foundation, Lankelly Chase, LCC/Burnley local grants.
  - **Fundable projects:** Mental health drop-in expansion, housing-first pilot, youth early intervention, volunteer training.

- **Website Issues:**
  - **Justin Pate** (current lead) needs prominence (per Dave Burdett).
  - **Remove Dave Burdett** as listed founder (update `team.html` and `premises.html`).

---

### **2. Next Steps (Actionable)**
#### **A. Compile Impact Data Pack**
1. **Extract WEMWBS Data:**
   - Check `impact_tracking.xlsx` (if exists) or Google Sheets (shared with Tom).
   - If missing, create a template using [WEMWBS scoring guidance](https://www.whatworkswellbeing.org.uk/resources/wewbs/).
   - **Command:** `git clone https://github.com/tompickup23/casualmindsmattercic` → Check `/docs/impact/` or `/data/`.

2. **Update Website:**
   - **File Path:** `casualmindsmattercic/team.html` → Move Justin Pate to top of team section.
   - **Command:** `git checkout -b update-team && nano team.html` → Edit `<div class="team-member">` order.
   - **Remove Dave Burdett:** Delete his `<div>` from `team.html` and `premises.html`.

3. **Prepare Grant Bid Templates:**
   - Use [Lottery Reaching Communities](https://www.tnlcommunityfund.org.uk/) and [NLCF](https://www.nationallotterycommunityfund.org.uk/) templates.
   - **File Path:** `/docs/bid_templates/` (create if missing).

#### **B. Verify Data Sources**
- **Referrals/Outcomes:** Check `services.html` for session/referral counts. If missing, query backend (if any) or contact frontline staff (St James’s House).
- **Cost-per-Outcome:** Calculate using `total_spend / beneficiaries` (e.g., £133K / 340 = ~£391/beneficiary).

#### **C. Submit Data to Funders**
- **NLCF:** Use [online portal](https://www.nationallotterycommunityfund.org.uk/apply).
- **Lottery Reaching Communities:** Submit via [TNL portal](https://www.tnlcommunityfund.org.uk/apply).

---

### **3. Resources**
- **WEMWBS Guide:** [https://www.whatworkswellbeing.org.uk/resources/wewbs/](https://www.whatworkswellbeing.org.uk/resources/wewbs/)
- **Outcome Star:** [https://www.outcomesstar.org.uk/](https://www.outcomesstar.org.uk/)
- **GitHub Repo:** [https://github.com/tompickup23/casualmindsmattercic](https://github.com/tompickup23/casualmindsmattercic)
- **Funding Links:**
  - NLCF: [https://www.nationallotterycommunityfund.org.uk/](https://www.nationallotterycommunityfund.org.uk/)
  - Lottery Reaching Communities: [https://www.tnlcommunityfund.org.uk/](https://www.tnlcommunityfund.org.uk/)

---
### **4. Risks/Blockers**
- **Missing WEMWBS Data:** If not tracked, funders may reject. **Solution:** Use proxy metrics (e.g., session attendance + self-reported wellbeing).
- **Website Edits:** Ensure `team.html` changes don’t break layout. **Test locally:** `python -m http.server` (from repo root).
- **Grant Deadlines:** Some funds (e.g., LCC) have rolling deadlines; prioritize NLCF/Lottery for faster turnaround.

---
**Next Action:** Update `team.html` and compile WEMWBS data by **Fri 12 Apr 2026**.
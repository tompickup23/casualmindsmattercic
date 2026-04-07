# Research: Plan next community outreach session

Generated: 2026-04-07
Project: cmm

### **Research Brief: Plan Next Community Outreach Session (Casual Minds Matter CIC)**
**Priority: M | Project: Casual Minds Matter**

---

#### **1. Key Findings**
- **Current Services & Outreach Gaps**:
  - **Services**: Weekly mental health drop-in (Howe Walk), daily homelessness support (St James’s House), bi-weekly community outreach, benefits advice.
  - **Outreach Frequency**: Bi-weekly (current). No clear schedule or metrics for past outreach sessions (missing in `services.html`).
  - **Impact Data**: 340 beneficiaries YTD, 48 sessions, 85 referrals (tracked in `services.html`).
  - **Funding Pipeline**: EHCF bid submitted (outcome May 2026). Next targets: NLCF, Lottery Reaching Communities, Henry Smith, Lloyds Bank Foundation.

- **Website Issues**:
  - **Justin Pate’s prominence**: Not highlighted in `team.html` (current team list: Dave Burdett, Tom Pickup, 1 trustee).
  - **Dave Burdett**: Listed as founder (per `team.html`); needs removal per Dave’s request.

- **Outreach Session Planning**:
  - No dedicated page for outreach sessions (only mentioned in `services.html`).
  - No sign-up/RSVP mechanism (static site limitation).

---

#### **2. Next Steps (Actionable)**
**A. Website Updates (Priority: High)**
1. **Update `team.html`**:
   - Remove Dave Burdett as founder (line 15 in `team.html`).
   - Add Justin Pate prominently (e.g., "Lead Coordinator" role).
   - **Command**:
     ```bash
     cd ~/tompickup23/casualmindsmattercic
     nano team.html  # Edit lines 10-20 to update team roles
     ```
   - **Preview**: `https://tompickup23.github.io/casualmindsmattercic/team.html`

2. **Create `outreach.html`** (new page):
   - Add bi-weekly outreach schedule (e.g., "Every 2nd & 4th Thursday, 11:00–14:00, Burnley Town Centre").
   - Include RSVP link (use Google Form or Calendly).
   - **File Path**: Create `outreach.html` in project root.
   - **Example Template**:
     ```html
     <h2>Upcoming Outreach Sessions</h2>
     <p>Next: Thursday, 17 Apr 2025, 11:00–14:00 (Burnley Town Centre)</p>
     <a href="https://forms.gle/RSVP_LINK" target="_blank">RSVP Here</a>
     ```
   - **Add to Navigation**: Update `index.html` and `services.html` to link to `outreach.html`.

**B. Outreach Session Planning (Priority: Medium)**
1. **Define Target Audience**:
   - Focus on homelessness hotspots (St James’s House, Burnley Bus Station) and youth (colleges/universities).
2. **Promotion**:
   - **Social Media**: Post on Facebook/Instagram (use Canva templates in `~/marketing/`).
   - **Local Press**: Submit to *Burnley Express* (contact: news@burnleyexpress.net).
3. **Metrics**:
   - Track attendance (Google Form) and feedback (5-question survey).

**C. Grant Pipeline (Priority: High)**
1. **Research NLCF Grants**:
   - **URL**: [https://www.nationallotterycommunityfund.org.uk](https://www.nationallotterycommunityfund.org.uk)
   - **Action**: Download application template and align with "youth early intervention" project.
2. **Lottery Reaching Communities**:
   - **URL**: [https://www.tnlcommunityfund.org.uk/funding/programmes/reaching-communities-england](https://www.tnlcommunityfund.org.uk/funding/programmes/reaching-communities-england)
   - **Action**: Draft 1-page concept note (use `~/grants/Lottery_Reaching_Communities_Concept.docx`).

---

#### **3. Resources**
- **Website**: [https://casualmindsmattercic.co.uk](https://casualmindsmattercic.co.uk)
- **GitHub**: [https://github.com/tompickup23/casualmindsmattercic](https://github.com/tompickup23/casualmindsmattercic)
- **Google Forms**: [Create RSVP Form](https://forms.gle/)
- **Canva**: [Burnley-themed templates](https://www.canva.com/) (use `~/marketing/` assets)
- **Grant Research**:
  - NLCF: [https://www.nationallotterycommunityfund.org.uk](https://www.nationallotterycommunityfund.org.uk)
  - Lottery Reaching Communities: [Link](https://www.tnlcommunityfund.org.uk/funding/programmes/reaching-communities-england)

---
#### **4. Risks/Blockers**
- **Static Website Limitations**: No backend for RSVPs. Workaround: Use Google Forms.
- **Grant Deadlines**: NLCF may have rolling deadlines; verify on their website.
- **Volunteer Capacity**: Ensure 2 staff/volunteers are available for outreach sessions.
# Research: Update website — make Justin Pate more prominent per Dave Burdett

Generated: 2026-04-07
Project: cmm

### **Structured Research Brief: Update Website — Make Justin Pate More Prominent**

#### **1. Key Findings**
- **Current Team Page (`team.html`)** lists **Dave Burdett** and **Justin Pate** as founders.
  - File: [`/team.html`](https://github.com/tompickup23/casualmindsmattercic/blob/main/team.html)
  - Justin Pate is listed under *"Trustees"* (not founders).
  - Dave Burdett is listed as *"Founder & CEO"* (needs removal per request).
- **Homepage (`index.html`)** has a brief mention of Justin in the *"About Us"* section but lacks prominence.
  - File: [`/index.html`](https://github.com/tompickup23/casualmindsmattercic/blob/main/index.html)
- **GitHub Pages** is the hosting provider (static HTML).

#### **2. Next Steps**
**A. Update `team.html`**
1. **Remove Dave Burdett** as founder:
   - Open [`/team.html`](https://github.com/tompickup23/casualmindsmattercic/blob/main/team.html) in a text editor.
   - Delete the `<div class="team-member">` block containing Dave’s details (lines ~15-25).
   - **Command (Git):**
     ```bash
     git checkout -b update-team-page
     git rm --cached team.html  # (if needed)
     nano team.html  # Edit file
     git add team.html
     git commit -m "Remove Dave Burdett from team page"
     git push origin update-team-page
     ```

2. **Promote Justin Pate** to *"Co-Founder & Trustee"*:
   - Move Justin’s `<div class="team-member">` block to the top of the `<div class="team-grid">`.
   - Ensure his photo and bio are visually prominent (adjust CSS if needed in [`/css/style.css`](https://github.com/tompickup23/casualmindsmattercic/blob/main/css/style.css)).

**B. Update Homepage (`index.html`)**
1. Add a **dedicated section** for Justin Pate:
   - Example snippet to insert after `<section id="about">`:
     ```html
     <section id="founders" class="founders-section">
       <h2>Meet Our Founders</h2>
       <div class="founder-card">
         <img src="images/justin-pate.jpg" alt="Justin Pate" class="founder-img">
         <h3>Justin Pate</h3>
         <p>Co-Founder & Trustee. Leads strategic development and partnerships.</p>
       </div>
     </section>
     ```
   - Update [`/css/style.css`](https://github.com/tompickup23/casualmindsmattercic/blob/main/css/style.css) to style `.founders-section` and `.founder-card`.

**C. Deploy Changes**
1. Merge the branch:
   ```bash
   git checkout main
   git merge update-team-page
   git push origin main
   ```
2. Verify changes at: [https://casualmindsmattercic.co.uk](https://casualmindsmattercic.co.uk)

#### **3. Resources**
- **GitHub Pages Docs**: [https://pages.github.com/](https://pages.github.com/)
- **CSS Styling Guide**: [`/css/style.css`](https://github.com/tompickup23/casualmindsmattercic/blob/main/css/style.css)
- **Image Assets**: Upload Justin’s photo to [`/images/`](https://github.com/tompickup23/casualmindsmattercic/tree/main/images)

#### **4. Risks/Blockers**
- **Merge Conflicts**: If other changes exist in `team.html`, resolve manually.
- **Image Upload**: Ensure Justin’s photo is added to `/images/` before referencing in HTML.
- **Caching**: GitHub Pages may take ~2 mins to reflect changes. Clear cache if needed.

**Priority**: Complete `team.html` edits first, then homepage updates. Aim for deployment within **24 hours**.
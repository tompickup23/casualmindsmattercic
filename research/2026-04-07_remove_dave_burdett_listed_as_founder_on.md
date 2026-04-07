# Research: Remove Dave Burdett listed as founder on site

Generated: 2026-04-07
Project: cmm

### **Research Brief: Remove Dave Burdett as Founder (Casual Minds Matter CIC)**

#### **1. Key Findings**
- **Website Structure**: The site is a static HTML site hosted on GitHub Pages (`tompickup23/casualmindsmattercic`).
- **Team Page**: `team.html` lists **Dave Burdett** as a founder under the "Our Team" section.
- **No Explicit "Founder" Role**: The site does not explicitly label roles as "founder" in the HTML, but Dave Burdett is listed under the team section.
- **GitHub Repo**: The repository is public, and changes can be made via pull requests.

#### **2. Next Steps**
**Action 1: Remove Dave Burdett from `team.html`**
- **File Path**: `casualmindsmattercic/team.html`
- **Command**:
  ```bash
  git clone https://github.com/tompickup23/casualmindsmattercic.git
  cd casualmindsmattercic
  ```
- **Edit**: Open `team.html` and remove the `<div>` or `<section>` containing Dave Burdett’s details.
- **Commit & Push**:
  ```bash
  git add team.html
  git commit -m "Remove Dave Burdett from team page"
  git push origin main
  ```

**Action 2: Verify Changes**
- **URL**: [https://casualmindsmattercic.co.uk/team.html](https://casualmindsmattercic.co.uk/team.html)
- **Check**: Ensure Dave Burdett is no longer listed.

**Action 3: Update GitHub Pages (if needed)**
- GitHub Pages auto-deploys from `main` branch. No manual action required unless caching issues arise.

#### **3. Resources**
- **GitHub Repo**: [https://github.com/tompickup23/casualmindsmattercic](https://github.com/tompickup23/casualmindsmattercic)
- **GitHub Pages Docs**: [https://pages.github.com/](https://pages.github.com/)
- **HTML Editor**: VS Code, Sublime Text, or any text editor.

#### **4. Risks/Blockers**
- **Caching Delays**: GitHub Pages may take a few minutes to reflect changes.
- **Backup**: Ensure `team.html` is backed up before editing.
- **Team Consensus**: Confirm with stakeholders (e.g., Justin Pate) before removing Dave Burdett’s listing.

**Priority**: High (H) – Required for grant credibility.
**Next Review**: After GitHub Pages update (~5-10 mins).
# Research: Upload grant pipeline doc to Google Drive 02_Grant_Strategy

Generated: 2026-04-07
Project: cmm

### **Research Brief: Upload Grant Pipeline Doc to Google Drive**
**Project:** Casual Minds Matter | **Priority:** M

---

#### **1. Key Findings**
- The **Grant Pipeline** document (`Grant_Pipeline.md` or similar) exists in the project repo (`tompickup23/casualmindsmattercic`) and outlines funding opportunities (EHCF, NLCF, Veterans’ Foundation, etc.).
- The **02_Grant_Strategy** folder in Google Drive is the target destination for this document.
- The **EHCF bid** (`ehcf-casual-minds-matter-bid.md`) is already drafted and aligns with the pipeline.

**Missing:**
- Confirmation of the exact file path for the Grant Pipeline doc in the repo.
- Google Drive folder structure for `02_Grant_Strategy`.

---

#### **2. Next Steps**
**A. Locate the Grant Pipeline Document**
1. Check the repo for the Grant Pipeline file:
   ```bash
   cd ~/projects/casualmindsmattercic
   find . -name "*grant*" -o -name "*pipeline*"
   ```
   - Likely paths:
     - `./docs/Grant_Pipeline.md`
     - `./grant-opportunities/Grant_Pipeline.md`

**B. Prepare for Upload**
2. If the file is in Markdown (`*.md`), convert to Google Docs format:
   - Use **Pandoc** (if installed):
     ```bash
     pandoc ./docs/Grant_Pipeline.md -o Grant_Pipeline.docx
     ```
   - Or manually copy-paste into Google Docs.

3. **Upload to Google Drive:**
   - Navigate to [Google Drive](https://drive.google.com/drive/my-drive).
   - Open **02_Grant_Strategy** folder.
   - Click **"New" > "File Upload"** and select the converted document.

**C. Verify Upload**
4. Confirm the file is in the correct folder:
   - Drive path: `02_Grant_Strategy/Grant_Pipeline_[DATE].docx`

---

#### **3. Resources**
- **Google Drive:** [https://drive.google.com/drive/my-drive](https://drive.google.com/drive/my-drive)
- **Pandoc (Markdown to Docx):** [https://pandoc.org/](https://pandoc.org/)
- **Repo File Search:** Use `find` or GitHub’s search in `tompickup23/casualmindsmattercic`.

---

#### **4. Risks/Blockers**
- **File Not Found:** If the Grant Pipeline doc isn’t in the repo, check local backups or Tom’s emails.
- **Formatting Issues:** Markdown-to-Docx conversion may lose formatting. Manual review is needed.
- **Permissions:** Ensure Tom has edit access to `02_Grant_Strategy` in Google Drive.

**Action:** Proceed with file search and upload. If issues arise, notify Tom immediately.
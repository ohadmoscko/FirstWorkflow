# Project Log – GPT Workflow Flowchart

This document records the entire journey of creating, improving, and deploying the GPT Workflow Flowchart project.

---

## 1. Starting Point
- Goal: Build a **professional, self-contained HTML file** to represent a GPT workflow.
- Requirements: responsive, interactive, semantic HTML5, inline CSS/JS, download/export, accessibility.
- Workflow to visualize:
  `Start → Catalyst-GPT → Idea-GPT → Risk Auditor GPT → SheetSmith-GPT / Closer-GPT → End of Day`

---

## 2. First Deliverable
- Initial HTML version delivered with:
  - Responsive grid of nodes.
  - Nodes clickable to open modal.
  - Inline CSS & JS only (no external libs).
  - Download button to save page as `.html`.

---

## 3. Iterations & Improvements

### Visuals
- Grid layout improved.
- Added tooltips for hover/focus.
- Fixed tooltip contrast (dark → light background, dark text).
- z-index adjusted so tooltips never obscure text.

### Functionality
- **Theme toggle** (dark/light).
- **Breadcrumb/Progress tracker**.
- **Next Step** button in modal.
- **Export JSON** option.
- **Timestamped HTML download**.
- **Print stylesheet** for PDF-ready export.

### Accessibility
- Focus trap inside modal.
- Background inert when modal open.
- Full keyboard navigation:
  - `Enter` / `Space` to open nodes.
  - `Esc` to close modal.
  - `Tab` cycles inside modal.
- ARIA roles and labels added.

---

## 4. Deployment Discussion
- Issue: local HTML (`C:/Users/...`) not shareable on phones.
- Solution:
  1. Rename file to `index.html`.
  2. Place in folder.
  3. Deploy via **Netlify Drop** or **GitHub Pages**.

---

## 5. GitHub Setup
- Repo created: `gpt-workflow`.
- Added `index.html` to root.
- Added `LICENSE`.
- Created `/docs/` folder.
- Generated docs:
  - `README.md` → overview, features, usage, roadmap.
  - `HISTORY.md` → step-by-step development.
  - `DESIGN_NOTES.md` → design system & accessibility.

Recommended repo structure:
```
gpt-workflow/
├── index.html
├── README.md
├── LICENSE
├── docs/
│   ├── HISTORY.md
│   └── DESIGN_NOTES.md
└── assets/
    └── screenshots/
        └── workflow.png
```

---

## 6. Files & Versions
- `GPT_Workflow_Flowchart.html` → Hebrew prototype.
- `GPT_Workflow_Flowchart (1).html` → English v1.
- `interactive_gpt_workflow_single_file_html_self_contained.html` → polished v1.5.
- `interactive_gpt_workflow_v_2_no_code_upgrades_single_file_html.html` → final v2 with theme toggle, JSON export, print styles.
- `custom_gpt_200_qa.md` → private DNA doc (⚠️ keep outside repo).

---

## 7. Screenshot
- Generated preview PNG (`workflow.png`).
- Added to `assets/screenshots/`.
- Linked in `README.md`.

---

## 8. Recommendations
- ✅ Public: `index.html`, `README.md`, `/docs/`, `/assets/screenshots/`.
- ❌ Private: `custom_gpt_200_qa.md` (keep out of repo or in private repo).
- Deployment: use **GitHub Pages** or **Netlify**.

---

## ✅ Final Outcome
- Professional, interactive single-file workflow (`index.html`).
- Full documentation pack (README, HISTORY, DESIGN_NOTES).
- Screenshot asset for README.
- Deployment strategy for GitHub Pages/Netlify.
- Clear separation of public vs private files.

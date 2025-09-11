# Development History – GPT Workflow Flowchart

This document explains the **journey from the first prototype** to the polished final version.

---

## 1. The Idea

The goal was to visualize a **GPT-driven workflow** (Start → Catalyst-GPT → Idea-GPT → Risk Auditor GPT → SheetSmith-GPT / Closer-GPT → End of Day)  
as a **professional, shareable, interactive flowchart**.

Constraints:
- Must be **single-file HTML** (self-contained).
- Must support **mobile and desktop**.
- Must be **accessible**.

---

## 2. First Version (Basic Prototype)

- Semantic HTML5 layout (`header`, `main`, `footer`).
- CSS variables for theming.
- Static grid of nodes (`Start`, `Catalyst-GPT`, …).
- Modal window for explanations.
- One button: **Download HTML**.

*Code snippet:*

```html
<div class="grid">
  <button class="node is-start">Start</button>
  <button class="node">Catalyst-GPT</button>
  <button class="node">Idea-GPT</button>
  <button class="node is-risk">Risk Auditor GPT</button>
  <button class="node">SheetSmith-GPT</button>
  <button class="node">Closer-GPT</button>
  <button class="node is-end">End of Day</button>
</div>
```

---

## 3. Improvements (v2)

### Functional Enhancements
- **Theme toggle** → Light/dark mode.
- **Breadcrumb** → Displays `Step X of Y • Node name`.
- **Focus trap** → Locks keyboard navigation inside modal.
- **Export JSON** → Downloads workflow as `.json`.
- **Timestamped download** → Filenames like `GPT_Workflow_2025-09-07.html`.

### UX Enhancements
- High-contrast tooltips (white card + dark text).
- Print stylesheet for clean PDF output.
- Responsive grid with auto-fit columns.

---

## 4. Sharing as a Site

Initially the file was named `GPT_Workflow_Flowchart.html`, which worked locally but failed on mobile.  
Solution:
- Rename file to `index.html`.
- Deploy using **GitHub Pages** or **Netlify Drop**.

---

## 5. Lessons Learned

- Accessibility is not optional → Focus management is critical.
- Netlify Drop simplifies hosting single-page projects.
- JSON export enables reuse of the workflow in other apps.

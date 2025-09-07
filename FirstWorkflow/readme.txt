# GPT Workflow Flowchart

An **interactive, self-contained flowchart** that represents a GPT-based workflow pipeline.  
This project is built as a **single HTML file** (no external libraries), optimized for **responsiveness, accessibility, and shareability**.

---

## 🚀 Demo

Once deployed (e.g., via GitHub Pages or Netlify), you can share the link with others:  
👉 **https://your-username.github.io/gpt-workflow/**

---

## 📌 Features

- **Self-contained**: All CSS & JavaScript inline, single `index.html`.
- **Responsive layout**: Works on desktop, tablet, and mobile.
- **Professional design**: Modern UI, rounded corners, subtle shadows, strong typography.
- **Interactive nodes**: Click any node to open details in an accessible modal.
- **Workflow navigation**:
  - Step counter (`Step X of Y`)
  - “Next Step” button
- **Theming**:
  - Light/dark mode toggle
  - Print stylesheet (for PDF export)
- **Data export**:
  - Download entire page (`.html`) with timestamp
  - Export workflow as JSON (`.json`)
- **Accessibility**:
  - Keyboard navigation
  - Focus trap inside modal
  - ARIA labels and live region hints

---

## 🛠️ Installation & Usage

### Option 1: Local (open file)
1. Clone the repository.
2. Open `index.html` in any browser.

### Option 2: Deploy to GitHub Pages
1. Go to repository **Settings → Pages**.
2. Set **Source** to `main branch / root`.
3. Your site will be live at:  
   `https://<username>.github.io/gpt-workflow/`

### Option 3: Deploy with Netlify Drop
1. Create a folder named `workflow-site`.
2. Place `index.html` inside it.
3. Drag the folder to [Netlify Drop](https://app.netlify.com/drop).
4. Receive a shareable link like:  
   `https://your-site.netlify.app`

---

## 🖼️ Screenshots

![Workflow Screenshot](assets/screenshots/workflow.png)

---

## 📂 Project Structure

```
gpt-workflow/
├── index.html          # Final version (self-contained)
├── README.md           # Project documentation
├── docs/
│   ├── HISTORY.md      # Development history (initial → final)
│   └── DESIGN_NOTES.md # Design decisions & accessibility notes
└── assets/
    └── screenshots/    # Example screenshots
```

---

## 🧭 Roadmap

- [ ] Optional zoom/pan controls for large workflows
- [ ] Multi-branch visual improvements
- [ ] Export to PNG/SVG
- [ ] Drag-and-drop node positioning (experimental)

---

## 📜 License

MIT License.  
Feel free to use, remix, and adapt.
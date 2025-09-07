# Design & Accessibility Notes

---

## 🎨 Color Palette

- Backgrounds: `--bg` (dark slate) / `--panel` (light card)
- Accent: `--accent` (blue), `--accent-strong` (strong blue)
- Success: green, Warning: amber, Risk: red
- Light mode toggled via `data-theme="light"`

---

## 📐 Layout

- Grid-based: `grid-template-columns: repeat(auto-fit, minmax(180px, 1fr))`
- Nodes styled as **cards** with subtle shadows.
- Tooltips placed **above nodes**, high contrast.

---

## ♿ Accessibility

- **ARIA roles**:
  - `role="dialog"`, `aria-modal="true"`
  - Tooltips use `role="tooltip"`
- **Keyboard support**:
  - `Tab` cycle trapped inside modal
  - `Escape` closes modal
  - `Enter/Space` opens node
- **Inert background**: When modal is open, main content is deactivated.

---

## 🗂️ Data Model

- `nodes` represented as buttons with attributes:
  ```html
  <button class="node" data-node="Catalyst-GPT" data-desc="...">...</button>
  ```
- `nextMap` defines connections:
  ```js
  const nextMap = {
    'Risk Auditor GPT': ['SheetSmith-GPT', 'Closer-GPT']
  };
  ```

---

## 🖨️ Print Styles

```css
@media print {
  body { background: #fff; color: #000; }
  .site, .flow { box-shadow: none; border: 1px solid #ddd; }
  .btn, .legend { display: none; }
}
```

---

## 🔮 Future Enhancements

- Zoom & pan for large workflows
- Drag-and-drop reordering
- Export to PNG using SVG → Canvas serialization

---
name: "Security: Avoid hard-coded secrets"
about: Use runtime config (localStorage / env) instead of committing secrets
title: "Avoid hard-coded secrets"
labels: security
---

**Checklist**
- [ ] No secrets in HTML/JS/CSS
- [ ] Secrets entered at runtime only (localStorage or env)
- [ ] README warns not to commit secrets

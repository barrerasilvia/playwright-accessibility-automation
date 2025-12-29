# Playwright Accessibility Automation

This repository demonstrates **real-world strategies for accessibility automation**
using **Playwright** and **axe-core**.

The goal of this project is **not** to replace manual accessibility audits, but to show
how automated checks can be used effectively to:

- Detect accessibility regressions
- Identify critical automatically-detectable issues
- Provide basic accessibility coverage on key pages

---

## 🚀 Tech Stack

- Playwright
- @axe-core/playwright
- TypeScript

---

## ♿ Accessibility Automation Strategies

This project is structured around three common automation scenarios:

### 1. Regression Tests
Detects new accessibility issues introduced during development on critical pages.

### 2. Critical Issues Checks
Focuses on high-impact accessibility issues that are reliably detected by automated tools
(e.g. missing accessible names, empty headings, invalid roles).

### 3. Basic Coverage
Runs automated accessibility checks on key user-facing pages to ensure a minimum level
of accessibility is consistently maintained.

---

## ⚠️ Important Notes

- Automated accessibility testing **cannot detect all accessibility issues**.
- Manual testing with assistive technologies is still required.
- Axe-core is used only where it provides real value.
- WCAG 2.2 conformance includes several success criteria that **cannot be reliably automated**.

---
## 📋 WCAG Coverage

Automated accessibility checks in this project are aligned with:

- WCAG 2.0 Level A and AA
- WCAG 2.1 Level A and AA

While some automated rules may conceptually relate to WCAG 2.2,
**full WCAG 2.2 conformance cannot be achieved through automation alone**.

WCAG 2.2 introduces success criteria that require manual evaluation, such as:

- Focus visibility
- Target size requirements
- Dragging alternatives
- Consistent help availability

For these criteria, **manual testing is required**.
---
## ▶️ Running the tests

```bash
npm install
npx playwright install
npx playwright test
```
## 📌Disclaimer

This project is for demonstration and educational purposes.
All tests are executed against publicly available websites.

# 🖥️ Playwright E2E Test Suite

End-to-end UI testing powered by **Playwright**, running in **GitHub Actions** with full traceability.

This repo demonstrates:
- Cross-browser testing (Chromium, Firefox, WebKit)
- Video recording & screenshot capture on failure
- HTML trace reports for debugging
- Secure, ephemeral CI execution

---

## 🚀 Features

✅ Runs tests on every push/PR  
✅ Captures **video**, **screenshots**, and **interactive traces**  
✅ Publishes full **HTML report** as artifact  
✅ Uses **headless browsers in Docker-compatible environment**  
✅ Zero external dependencies — pure GitHub Actions

---

## 📦 Artifacts on Failure

When a test fails, the workflow uploads:
- `playwright-report/` — interactive HTML report
- `test-results/` — videos, screenshots, traces

Download them from the **Actions tab → workflow run → Artifacts**.

---

## ▶️ Run Locally

```bash
npm install
npx playwright install
npx playwright test
npx playwright show-report

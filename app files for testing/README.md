# Second Street Portal — Static Site

Borrower-facing application portal for Second Street CR, S.R.L.

**Live URL (coming soon):** `https://apply.mysecondstreet.com`

---

## Files

| File | Purpose |
|------|---------|
| `apply.html` | Borrower application portal (v7) |
| `index.html` | Landing page (coming Sprint 5) |

---

## Testing Locally

No server required. Just download `apply.html` and open it in any browser.

**What to test:**
- All 4 loan products: US Purchase, US Refinance, CA Purchase, CA Refinance
- Address history chaining (enter a move-in date < 24 months ago to trigger prior address prompt)
- Co-applicant toggle (up to 3)
- SSN field (US) vs SIN field (CA)
- Phone number fields (US/CA + optional CR number)
- All declaration checkboxes on the final step

**Note:** The Submit button is not yet wired to a backend — submission will not process during this testing phase. All other form logic is fully functional.

---

## Deployment (Render)

- Type: Static Site
- Build command: *(none)*
- Publish directory: `.`
- Custom domain: `apply.mysecondstreet.com`
- DNS: `CNAME apply → [render-subdomain].onrender.com`

---

## Repo Structure (Target)

```
secondstreet-portal-static/
  apply.html      ← portal v7
  index.html      ← landing page (Sprint 5)
  README.md
```

---

*Second Street Inc. / Second Street CR, S.R.L. — Internal use only*

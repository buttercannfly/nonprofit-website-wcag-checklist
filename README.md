# 501(c)(3) Nonprofit Website WCAG 2.2 AA, Form 990 & Zero-Tip Giving Checklist (2026)

An open-source, MIT-licensed operational checklist and semantic HTML starter for **501(c)(3) nonprofits, grant applicants, animal rescues, food pantries, civic organizations, and volunteer boards**.

Built for lean nonprofit teams and web stewards who need to verify:
1. **WCAG 2.2 Level AA baseline readiness** (without paid JavaScript "overlay" widgets)
2. **Public IRS Form 990 & governance document hosting** (separating public transparency files from private board packets)
3. **Zero-tip, direct HTTPS donation links** (keeping donor checkout predictable without surprise platform "tips")

---

## Repository Contents

| Resource | Purpose |
| --- | --- |
| [`checklists/wcag-2.2-aa-grant-audit.md`](checklists/wcag-2.2-aa-grant-audit.md) | Printable POUR + WCAG 2.2 AA audit checklist and 15-minute keyboard/mobile test protocol |
| [`checklists/form-990-and-board-vault.md`](checklists/form-990-and-board-vault.md) | Public inspection vs. private board portal matrix, Schedule B redaction reminder, and file naming rules |
| [`snippets/accessible-nonprofit-shell.html`](snippets/accessible-nonprofit-shell.html) | Dependency-free semantic HTML5/CSS starter with skip link, `3px` `:focus-visible`, HTTPS Donate CTA, and Form 990 table |
| [`LICENSE`](LICENSE) | MIT License |

---

## Quick 10-Point Pre-Grant Readiness Check

- [ ] **Skip Navigation**: First `Tab` press on every page reveals a visible "Skip to main content" link jumping to `#main-content`.
- [ ] **Keyboard-Only Navigation**: Top nav, mobile menu toggle, accordions, and donation buttons are reachable and operable with `Tab`, `Shift+Tab`, `Enter`, and `Space`.
- [ ] **Visible Focus Indicator**: High-contrast `:focus-visible` outlines (`>= 2px`, recommended `3px`) remain clearly visible and are not hidden behind sticky headers.
- [ ] **Color Contrast**: Body text meets at least `4.5:1` (`3:1` for large text `>= 18pt` or `14pt` bold) and interactive borders/icons meet `3:1`.
- [ ] **One `<h1>` & Logical Headings**: Headings step cleanly (`h1 -> h2 -> h3`) rather than skipping levels for styling.
- [ ] **Mobile Reflow (`390px` / `320px`)**: Zero horizontal page overflow (`scrollWidth <= clientWidth`) and tap targets `>= 24x24px` CSS pixels.
- [ ] **No Accessibility Overlays**: Accessibility comes from native semantic HTML (`<header>`, `<nav>`, `<main>`, `<footer>`, `<label>`), not third-party JavaScript overlay toolbars.
- [ ] **Public Form 990 Inspection Ready**: Recent public-inspection Form 990 / 990-EZ / 990-N files are published clearly with **Schedule B donor names and addresses redacted** before upload.
- [ ] **Private Board Documents Gated**: Board minutes, personnel files, and unredacted donor records sit behind authenticated board portal logins — never in open PDF directories.
- [ ] **Zero-Tip Direct HTTPS Giving**: Donate buttons route directly to your nonprofit's own HTTPS payment link (such as Stripe or PayPal) without forcing donors through an optional 10%–17% platform tip prompt.

---

## Why Avoid Accessibility Overlays?

Many small nonprofits install one-line JavaScript accessibility widgets expecting instant compliance. In practice, overlay scripts cannot replace missing form `<label>` associations, broken heading structures, inaccessible PDF scans, or keyboard traps—and they often conflict with screen readers and add third-party script weight. Writing clean semantic HTML (see [`snippets/accessible-nonprofit-shell.html`](snippets/accessible-nonprofit-shell.html)) fixes the underlying structure directly.

---

## Interactive Audit & Reference Guides

Maintained alongside **[Nonprofit Web Builder](https://nonprofitwebbuilder.com)**:

- **Run a 60-second checklist self-check**: [Nonprofit Website Audit Tool](https://nonprofitwebbuilder.com/nonprofit-website-audit)
- **Deep dive on nonprofit ADA & WCAG**: [Nonprofit Website Accessibility & WCAG 2.2 AA Guide](https://nonprofitwebbuilder.com/guides/nonprofit-website-accessibility-wcag)
- **Board governance & IRS disclosure workflow**: [Hosting Board Documents & Form 990s Online](https://nonprofitwebbuilder.com/guides/nonprofit-board-documents-and-990s)
- **Platform evaluation criteria**: [How to Choose a Nonprofit Website Builder](https://nonprofitwebbuilder.com/best-nonprofit-website-builder)

> **Disclaimer**: This repository provides engineering and operational best practices, not legal, tax, or formal compliance counsel. Consult qualified legal or nonprofit tax professionals for organization-specific requirements.

## Contributing

Pull requests improving checklist clarity, assistive-technology test steps, or HTML/CSS accessibility examples are welcome. Released under the [MIT License](LICENSE).

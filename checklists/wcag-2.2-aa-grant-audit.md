# WCAG 2.2 Level AA Audit Checklist for Nonprofit & Grant-Funded Websites

Use this checklist before grant submissions, annual board reviews, or site launches. Pair it with the interactive **[Nonprofit Website Audit](https://nonprofitwebbuilder.com/nonprofit-website-audit)** and **[WCAG Accessibility Guide](https://nonprofitwebbuilder.com/guides/nonprofit-website-accessibility-wcag)**.

---

## 1. Perceivable

- [ ] **Meaningful Alt Text**: Every informative photo (programs, volunteers, impact charts) has concise `alt` text describing its purpose; purely decorative icons use `alt=""` or `aria-hidden="true"`.
- [ ] **Text Contrast (`>= 4.5:1`)**: Normal body copy, navigation links, button labels, and form placeholders/help text meet `4.5:1` contrast against their background.
- [ ] **Large Text & UI Components (`>= 3:1`)**: Headings `>= 18pt` (`24px`) or `14pt` (`18.66px`) bold, form input borders, checkboxes, and focus indicators meet `>= 3:1`.
- [ ] **Captions & Transcripts**: Embedded campaign or program videos include synchronized captions and a plain-text summary or transcript.
- [ ] **No Color-Only Status**: Required form fields, status badges, and chart legends pair color with text or icons (`* Required`, checkmarks, clear labels).
- [ ] **200% Zoom & Mobile Reflow**: Increasing browser zoom to `200%` or viewing at `320px–390px` width keeps all text readable without clipped buttons or horizontal scrolling.

## 2. Operable

- [ ] **Skip to Main Content Link**: The first interactive element in the DOM jumps directly to `<main id="main-content">` and appears visibly on keyboard focus.
- [ ] **Full Keyboard Navigation**: Users can reach menus, dropdowns, modal dialogs, donation amount links, and footer links using only `Tab`, `Shift+Tab`, `Enter`, `Space`, and `Escape`.
- [ ] **Clear Focus Ring**: Never use `outline: none` without an explicit high-contrast `:focus-visible` style (`2px–3px` solid outline with offset).
- [ ] **Focus Not Obscured (WCAG 2.2 — 2.4.11)**: Sticky top navigation bars or cookie/announcement banners do not cover the currently focused button or link when tabbing down the page.
- [ ] **Target Size Minimum (WCAG 2.2 — 2.5.8)**: Interactive buttons, icon toggles, and nav links have at least `24x24px` CSS hit area (aim for `44x44px` on mobile).
- [ ] **No Auto-Playing Carousels Without Pause**: If motion or sliders exist, provide a visible pause control and respect `@media (prefers-reduced-motion: reduce)`.
- [ ] **Descriptive Page `<title>` & Links**: Every page has a unique `<title>`, and links explain their destination (e.g., `"Download 2025 Form 990 (PDF, 1.4 MB)"` rather than `"Click here"`).

## 3. Understandable

- [ ] **Document Language Declared**: `<html lang="en">` (or appropriate primary language tag) is set cleanly; inline language changes use `lang="..."`.
- [ ] **Consistent Navigation**: Primary header navigation and footer links stay in the same predictable order across Home, Programs, Donate, and Transparency pages.
- [ ] **Programmatic Form Labels**: Every `<input>`, `<select>`, and `<textarea>` is paired with a visible `<label for="...">`—never rely on `placeholder` alone.
- [ ] **Specific Error Messages**: Validation errors identify the exact field and how to fix it (e.g., `"Enter a valid https:// donation checkout URL"`).
- [ ] **Accessible Authentication (WCAG 2.2 — 3.3.8)**: Member/board login flows support password managers (`paste` enabled) and magic links / passkeys / SSO rather than cognitive puzzles.
- [ ] **Redundant Entry Avoided (WCAG 2.2 — 3.3.7)**: Multi-step volunteer or intake forms do not force visitors to re-type information already supplied in the same flow.

## 4. Robust

- [ ] **Semantic Landmarks**: Layout uses one `<header>`, `<nav aria-label="...">`, one `<main id="main-content">`, and `<footer>` instead of generic `<div>` soup.
- [ ] **Single `<h1>` & Unskipped Headings**: Page starts with one `<h1>` and nests `<h2>`, `<h3>` cleanly so screen reader rotor navigation makes sense.
- [ ] **Clean Accessible Tables**: Grant budgets, program schedules, and Form 990 indexes use `<table>` with `<caption>`, `<thead>`, `<th scope="col">`, and `<th scope="row">`.
- [ ] **Zero Accessibility Overlays**: Confirm no third-party accessibility toolbar script is fighting native screen-reader landmarks.

---

## 15-Minute Manual Test Protocol (Zero Paid Tools Needed)

1. **Unplug the Mouse (`3 min`)**: Press `Tab` from the browser address bar. Confirm the skip link appears, focus outline is obvious everywhere, and sticky headers never hide the focused element.
2. **Heading & Landmark Check (`2 min`)**: Confirm one `<h1>`, logical `<h2>`/`<h3>` nesting, and real `<button>`/`<a>` tags (never clickable `<div>` elements).
3. **Mobile `390px` Reflow (`3 min`)**: Open DevTools responsive mode at `390x844` (and `320px`) and verify `document.documentElement.scrollWidth <= document.documentElement.clientWidth`.
4. **Reduced Motion & Zoom (`2 min`)**: Toggle `prefers-reduced-motion: reduce` and zoom to `200%`; confirm hero/cards remain readable and uncluttered.
5. **Document & Donate Link Check (`5 min`)**: Confirm public Form 990 links announce file format/year cleanly, and the Donate button opens an `https://` checkout URL cleanly without unexpected platform fees or popups.

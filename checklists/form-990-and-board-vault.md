# Nonprofit Form 990 Public Inspection & Board Document Vault Checklist

Publishing governance documents builds trust with institutional funders, major donors, and charity watchdogs—while protecting sensitive donor and personnel records from accidental exposure.

Pair this checklist with our detailed walkthrough: **[How Nonprofits Should Host Board Documents & Form 990s](https://nonprofitwebbuilder.com/guides/nonprofit-board-documents-and-990s)**.

> **Important Note**: This checklist outlines operational website and document-hygiene practices for U.S. nonprofits. Always review IRS Form 990 public inspection and state charity registration rules with your CPA or legal counsel.

---

## 1. Public Transparency Page vs. Private Board Portal

| Document Category | Public Website (`/transparency`) | Authenticated Board Portal | Why |
| --- | --- | --- | --- |
| **IRS Determination Letter (501(c)(3))** | Yes | Also archived | Funders and corporate matching programs verify tax-exempt status immediately |
| **Form 990 / 990-EZ / 990-N (Last 3 Years)** | **Yes (Redacted Schedule B)** | Unredacted archive | U.S. nonprofits must provide public inspection copies; public 501(c)(3) disclosure excludes contributor names/addresses on Schedule B |
| **Annual Impact & Financial Summary** | Yes | Yes | Helps donors and grantmakers evaluate program expense vs. admin ratios |
| **Bylaws & Conflict-of-Interest Policy** | Optional / Recommended | Yes | Frequently requested in foundation grant portals |
| **Board Roster (Names & Roles)** | Yes (Business contact only) | Full roster + personal phone/email | Avoid publishing board members' home addresses or personal phone numbers publicly |
| **Board Meeting Minutes & Packets** | Summary / Approved highlights only (if applicable) | **Yes (Private)** | Working budgets, executive reviews, legal discussions, and draft strategies belong behind role-based auth |
| **Major Donor Lists / CRM Exports** | **Never** | Restricted Finance/Board access | Protects donor privacy and prevents credential/phishing risks |

---

## 2. Pre-Upload Sanitization Checklist (Form 990 PDFs)

- [ ] **Verify Schedule B Redaction**: For a typical public charity (`501(c)(3)`), confirm donor names and street addresses on Schedule B are permanently redacted (not merely covered with a black rectangle annotation inside a vector PDF!) before uploading to the public site.
- [ ] **Check Metadata**: Strip unnecessary local author paths, internal comments, or spreadsheet formulas from PDF exports.
- [ ] **Flatten / Export Text-Selectable PDF**: Do **not** upload crooked smartphone scans of paper filings. Export a searchable, text-selectable PDF so screen readers and search tools can parse headings and figures.
- [ ] **Keep Individual PDFs Focused**: Ensure files stay reasonably sized (for example under `25 MB`, ideally `1–5 MB` for annual filings) so mobile users on cellular connections can open them quickly.

---

## 3. Clean Naming & Accessible Linking Rules

Avoid raw timestamps or vague links like `Scan_0042.pdf` or `"Download here"`.

**Recommended filenames**:
```text
/documents/2025-form-990-public-inspection.pdf
/documents/2024-audited-financial-statements.pdf
/documents/irs-501c3-determination-letter.pdf
/documents/annual-impact-report-2025.pdf
```

**Recommended link text in HTML / CMS**:
- Good: `Download FY 2025 Form 990 Public Inspection Copy (PDF, 1.8 MB)`
- Avoid: `2025.pdf` or `Click here`

---

## 4. Board Portal Security Baseline

- [ ] **Separate Storage / Access Control**: Never rely on "unlisted URLs" inside a public `/uploads/` folder for private board packets—require authenticated member login with session validation.
- [ ] **Least-Privilege Roles**: Separate Admin stewards (who publish site pages and upload files) from read-only Board Members.
- [ ] **Annual Access Audit**: Remove former board members, temporary grant consultants, and rotated volunteers at each annual meeting.

---

## Related Resources

- [Live Nonprofit Website Audit](https://nonprofitwebbuilder.com/nonprofit-website-audit)
- [Board Documents & Form 990 Guide](https://nonprofitwebbuilder.com/guides/nonprofit-board-documents-and-990s)
- [Nonprofit Website Builder Comparison](https://nonprofitwebbuilder.com/best-nonprofit-website-builder)

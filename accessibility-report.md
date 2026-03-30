# Accessibility Report

### 1. Images
- Issue: Some images had missing or unclear `alt` text.
- Fix: Ensured all `<img>` have meaningful `alt` attributes (e.g., `<img src="images/profile.jpg" alt="Denzel Anyiko">`).

### 2. Headings
- Issue: Heading hierarchy was mostly OK but verification needed.
- Fix: ensured there is one `<h1>` per page and subsections use `<h2>`, `<h3>` appropriately.

### 3. Links
- Issue: Some links may have had nondiscriptive text in other pages.
- Fix: Used descriptive, context-rich text for links: `Email me`, `See my skills`, etc.

### 4. Language
- Issue: `lang` attribute was already present on `<html>`.
- Fix: Verified `lang="en"` is set on all pages (`index.html`, `about.html`, `contact.html`).

### 5. Form labels
- Issue: `contact.html` used `fieldset` and `legend` incorrectly and message textarea was outside the fieldset.
- Fix: Reorganized form semantics:
  - `<form>` contains one `<fieldset>`
  - `<legend>` is first child with label text `Send a message`
  - All inputs, select, and textarea have corresponding `<label for="...">`
  - Checkbox remains wrapped in label for accessibility.

## Lighthouse Audit Results
- 100% Accesibility
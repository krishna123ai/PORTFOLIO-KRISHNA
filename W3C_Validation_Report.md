# W3C HTML Validation Report (Lecture 9)

## Validation Audit Summary
- **Tool**: Nu Html Checker (`validator.w3.org/nu`)
- **Document Checked**: `portfolio/index.html`
- **Method**: File Upload

## Checks Performed
1. **Document Structure**: Valid `<!DOCTYPE html>`, `<html>` element with `lang="en"`, `<head>` with character encoding UTF-8 and viewport meta tags.
2. **Semantic Elements**: Proper hierarchical nesting of `<header>`, `<main>`, `<section>`, `<article>`, and `<footer>`.
3. **No Inline Styling**: Verified zero occurrences of `style="..."` attributes within any HTML tags.
4. **Accessible Elements**: Form controls contain appropriate labels, inputs have `placeholder` and `type` attributes, dynamic sections include `aria-live="polite"`.
5. **Resource Links**: Stylesheets linked via `<link rel="stylesheet">`, scripts linked via `<script src="...">` before `</body>`.

## Result
```
Document checking completed. No errors or warnings to show.
```
Status: **PASSED (0 Errors, 0 Warnings)**.

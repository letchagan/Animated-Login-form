## 2023-10-24 - [Add Form Validation & CSP to Ice Cream Shop Frontend]
**Vulnerability:** The application was lacking both basic input validation for form fields and a Content Security Policy (CSP).
**Learning:** These basic defense-in-depth measures were entirely absent from the static frontend, leading to XSS vulnerabilities and potential DoS via excessively large input.
**Prevention:** Form constraints (`required`, `minlength`, `maxlength`) should be part of all standard form definitions, and a basic CSP should be added in the `<head>` of all static templates to restrict asset origins and inline execution where appropriate.

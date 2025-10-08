## 👨‍💻 Author

**Alves Gonzalez**  
Software QA Engineer | Accessibility & Automation Testing  
📧 alvesdgonzalez3@gmail.com  
🔗 [LinkedIn](https://linkedin.com/in/alves-gonzalez)  

# Axe Accessibility Audit – Stack Overflow

This project documents an accessibility audit performed on the **Stack Overflow** website using **Axe DevTools (Pro 4.10.3)** within Chrome DevTools.  
The goal of this test was to identify accessibility issues according to **WCAG 2.1 AA** standards and to evaluate the site's compliance with modern web accessibility practices.

---

## 🧩 Overview

**Tool Used:** Axe DevTools (Pro 4.10.3)  
**Website Tested:** [https://stackoverflow.co/](https://stackoverflow.co/)  
**Audit Type:** Full-Page Accessibility Scan  
**Testing Standards:** WCAG 2.1 AA  
**Tester:** Alves Gonzalez 

---

## 🧪 Test Summary

| Test Type | Issues Found | Description |
|------------|---------------|-------------|
| Automatic Issues | 4 | Issues automatically detected by Axe rules |
| Guided Issues | 91 | Issues found through guided/manual checks |
| Manual Issues | 0 | No manual issues logged during this session |
| **Total Issues** | **95** | Overall detected accessibility issues |

**Severity Breakdown:**
- 🟥 Critical: 91  
- 🟧 Serious: 4  
- ⚪ Moderate: 0  
- ⚪ Minor: 0  

---

## 🧭 Key Findings

### 1. Color Contrast
> **Issue:** Elements must meet minimum color contrast ratio thresholds.  
**Count:** 4  
**WCAG Reference:** [1.4.3 Contrast (Minimum)](https://www.w3.org/WAI/WCAG21/Understanding/contrast-minimum.html)

### 2. Keyboard Accessibility
> **Issue:** Function cannot be performed by keyboard alone.  
**Count:** 90  
**WCAG Reference:** [2.1.1 Keyboard](https://www.w3.org/WAI/WCAG21/Understanding/keyboard.html)

### 3. Accessible Name
> **Issue:** The element's accessible name is missing or incorrect.  
**Count:** 1  
**Example:** Button labeled “Our Products” – name does not accurately describe element purpose.  
**WCAG Reference:** [4.1.2 Name, Role, Value](https://www.w3.org/WAI/WCAG21/Understanding/name-role-value.html)

---

## 🧠 Guided Tests Performed

- **Keyboard Navigation Test** – 90 failures  
  - Many elements skipped in the tab order  
  - No keyboard alternative provided  
- **Interactive Elements Test** – 1 issue  
  - “Our products” button name unclear or missing  
- **Color Contrast Test** – 4 issues  
  - Low contrast ratio between text and background colors  

---

## 🧰 Tools & Environment

- **Browser:** Google Chrome  
- **Axe DevTools:** Version 4.10.3  
- **OS:** Windows 10  
- **Testing Mode:** Full-page scan + guided intelligent testing  

---

## 📊 Screenshots

Screenshots from this audit are stored in the `/screenshots` directory, showing:
- Overall issue summary
- Guided keyboard test results
- Interactive elements validation
- DOM inspection view

---

## 🧾 Recommendations

1. Ensure all interactive elements (buttons, links) are keyboard-navigable.  
2. Provide descriptive and unique accessible names for UI components.  
3. Improve text-to-background color contrast ratios.  
4. Conduct re-testing after remediation to confirm compliance with WCAG 2.1 AA.

---

## 📈 Future Improvements

- Perform a second round of audits after issue remediation.  
- Add Lighthouse and Wave scans for comparison.  
- Automate accessibility checks using Axe CLI or Cypress-Axe integration.

---

## 📜 License

This project is for **educational and portfolio purposes** only.  
All content and screenshots are owned by their respective entities (Stack Overflow, Deque Systems).


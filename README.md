# ♿ Accessibility Audit — Stack Overflow

**Author:** Alves Gonzalez  
**Role:** Software QA Engineer | Accessibility & Automation Testing  
📧 alvesdgonzalez3@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/alves-gonzalez)

---

## 🧩 Overview
Performed accessibility audits on **Stack Overflow (https://stackoverflow.co/)** using:
- **Axe DevTools (Pro 4.10.3)** for guided WCAG 2.1 AA compliance testing  
- **Axe CLI (v3.2.1)** for automated accessibility scans in Windows Command Prompt

Both tests focused on identifying color contrast, ARIA, landmark, and keyboard accessibility issues.

---

## 🧪 Results Summary
| Tool | Issues Detected | Key Findings |
|------|------------------|---------------|
| **Axe DevTools** | 95 total | 91 critical (keyboard), 4 serious (contrast) |
| **Axe CLI** | 14–15 total | ARIA, color contrast, and missing landmarks |

**Common Violations**
- Missing or duplicate landmarks (`main`, `contentinfo`)  
- Low text contrast ratios  
- Missing accessible names for buttons  
- Elements skipped in keyboard navigation  

---

## ⚙️ Axe CLI Command Example
```bash
npm install -g axe-cli
axe https://stackoverflow.co/ --browser chrome --save test-results.json


---

## 📜 License

This project is for **educational and portfolio purposes** only.  
All content and screenshots are owned by their respective entities (Stack Overflow, Deque Systems).


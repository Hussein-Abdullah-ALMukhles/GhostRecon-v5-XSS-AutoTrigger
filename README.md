# 👻 GhostRecon v5 – DOM XSS Auto Trigger & Token Leak PoC

 Developed by: Hussein Abdullah ALMukhles – Fast CyberSecurity  
📅 Date: 2025-05-XX  
🎯 Purpose: Ethical demonstration of a DOM-based XSS vulnerability with potential token exfiltration using `tl`, `sl`, and `op` parameters reflected in `WIZ_global_data`.

---

##  What This PoC Does

This HTML file performs the following steps automatically:

1. Parameter Reflection Detection
   - Scans `window.WIZ_global_data` for reflected parameters like `tl`, `sl`, `op`.

2. DOM Usage Monitoring
   - Checks if those parameters appear inside `innerHTML`, `outerHTML`, `attributes`, etc.

3. Execution Context Detection
   - Tracks if any parameter is used in dangerous sinks like `setTimeout`, `eval`, `Function`.

4. Auto Exploitation Attempt 
   - Triggers a payload if possible, and detects if `alert('XSS')` was executed.

5. Silent Token Exfiltration
   - If a token is stored in `localStorage` or `sessionStorage`, it is sent silently to:


---

## 🔐 Legal & Ethical Usage Disclaimer

> **⚠️ WARNING:**
> This script is intended for ethical hacking, responsible disclosure, and educational research **only**.

- Do **NOT** use this script on any system without explicit written permission.
- Unauthorized use of this script may violate applicable laws and result in legal consequences.
- You are solely responsible for how you use this code.

> 🛡️ Hussein Abdullah ALMukhles and Fast CyberSecurity are **not responsible** for any misuse or abuse of this project.

---

## 📁 Files

| File | Description |
|------|-------------|
| `GhostRecon_v5.html` | Main PoC HTML with embedded logic |
| `result.json` | Output showing what was reflected and how it was used |
| `proof_hash.txt` | SHA-256 hash to prove script integrity |

---

## 🧾 How to Use

1. Host `GhostRecon_v5.html` on GitHub Pages.
2. Access it via:

3. Check webhook for any token or reflection leak.
4. Take screenshots or export `result.json` for use in vulnerability reports.

---
## 🔏 Proof of Integrity

SHA-256 hash of this file and code is stored in `proof_hash.txt`.
Use it to validate that the PoC hasn't been altered after responsible submission.

---

 For authorized security research or collaboration:  
**Email:** contactfastcyber@gmail.com  

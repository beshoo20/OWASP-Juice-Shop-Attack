Purpose of the Test
The purpose of this testing was to identify security weaknesses in the OWASP Juice Shop, a purposely vulnerable web application. This application is often used by security professionals to practice their skills in finding and fixing common security flaws in web apps.

Key Findings
Through testing, we discovered a few serious security issues:

Hidden Admin Path: An attacker could easily find the admin login page by guessing the URL.
Weak Admin Password Protection: The admin login page didn’t have enough protection against multiple password attempts, making it possible to guess the admin password.
Cross-Site Scripting (XSS): The search bar allowed attackers to inject harmful code that could run in another user’s browser.
Impact
These vulnerabilities could lead to severe problems:

Attackers could find and access the admin area, taking full control of the application.
Brute-force attacks could let attackers guess the admin’s password and log in as an admin.
The XSS vulnerability could allow attackers to steal sensitive data from users or trick them into visiting malicious websites.
Recommendations
To improve security, we recommend:

Hide admin paths: Ensure that sensitive admin URLs are not easily discoverable.
Protect against brute force: Add protections like limiting login attempts and enabling two-factor authentication.
Fix XSS vulnerabilities: Make sure the app properly checks and cleans user input to prevent harmful scripts from running.

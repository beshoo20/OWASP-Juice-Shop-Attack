# OWASP-Juice-Shop-Attack
A penetration testing report for OWASP Juice Shop vulnerabilities


Project Overview:
This project involves the penetration testing of the OWASP Juice Shop, a deliberately vulnerable web application designed to help security professionals and learners practice identifying and fixing common web security flaws. The goal of this project is to simulate attacks on the Juice Shop, identify critical vulnerabilities, and propose solutions to improve its security.


Objectives:
Perform penetration testing on the OWASP Juice Shop to identify security weaknesses.
Simulate attacks such as brute-force login, XSS, and hidden path discovery.

Vulnerabilities Identified
1-Hidden Admin Path: Admin login paths were discoverable through inspection of the site's source code.
2-Brute Force on Admin Credentials: Weak protections allowed for brute-forcing the admin login page.
3-Cross-Site Scripting (XSS): The search bar did not sanitize user input, allowing for script injection.

Remediation Recommendations
1-Admin Path: Protect sensitive URLs and remove unnecessary paths from public access.
2-Brute Force Protection: Implement rate-limiting, account lockout features, and multi-factor authentication for admin access.
3-XSS Prevention: Ensure input sanitization and validation to prevent the injection of harmful scripts.

Team Members
Mark Medhat (2305496) : Lead Penetration Tester
Beshoy Melad (2305140) : Exploit Developer, Documentation & Reporting 


# OWASP Juice Shop – Web Application Security Assessment

## Project Overview

This project was completed as part of the Web Application Security module at Technological University Dublin.

The aim was to identify, investigate and analyse security vulnerabilities in OWASP Juice Shop, an intentionally vulnerable web application designed for cybersecurity training.

The project involved practical vulnerability testing, source code analysis and recommendations for improving application security.

## Tools and Technologies

- OWASP Juice Shop
- OWASP ZAP
- Semgrep
- Browser Developer Tools
- JavaScript and HTTP Requests
- Static Application Security Testing (SAST)
- Dynamic Application Security Testing (DAST)

## Security Vulnerabilities Investigated

### 1. Security Misconfiguration – Access Logs

- Identified publicly accessible server logs through the `/support/logs` directory.
- Investigated how missing access restrictions exposed internal application information.
- Recommended disabling directory indexing and restricting access to sensitive logs.

### 2. Broken Access Control – Forged Review

- Investigated a vulnerability allowing users to submit reviews under another user's identity.
- Analysed and modified HTTP requests to demonstrate the weakness.
- Recommended server-side identity validation and stronger authorisation controls.

### 3. Static Application Security Testing – Semgrep

- Used Semgrep to analyse the application's source code.
- Recorded 38 security findings during the scan.
- Investigated findings involving SQL injection, directory listing and unsafe use of `eval()`.
- Recommended parameterised queries, secure configuration and safer coding practices.

### 4. Dynamic Application Security Testing – OWASP ZAP

The group also conducted DAST testing using OWASP ZAP, investigating:

- Missing Content Security Policy (CSP) headers.
- JWT storage in browser localStorage.
- Inconsistent anti-clickjacking security headers.

## My Individual Contributions

My contributions to this group project included:

- Investigating the Access Logs security misconfiguration vulnerability.
- Demonstrating the Forged Review broken access control vulnerability.
- Performing static code analysis using Semgrep.
- Analysing security findings and identifying their potential impact.
- Researching and documenting appropriate mitigation strategies.
- Preparing technical explanations and supporting evidence for the project report.

## Project Outcomes

- Developed practical experience identifying web application vulnerabilities.
- Improved my understanding of the OWASP Top 10 security risks.
- Gained hands-on experience with Semgrep and manual security testing.
- Strengthened my ability to analyse vulnerabilities and recommend security improvements.
- Improved my technical documentation and cybersecurity reporting skills.

## Disclaimer

This project was conducted for educational purposes using OWASP Juice Shop, an intentionally vulnerable application. All testing was performed in an authorised local environment.

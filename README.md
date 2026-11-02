CyberChef Suspicious URL Investigation

SOC Analyst Cybersecurity Portfolio Project

Analyst: David Jeffries
Tools: CyberChef, GitHub
Environment: Simulated Cybersecurity Training Lab
Focus: Phishing Analysis, URL Decoding, Base64 Decoding, Threat Investigation

⸻

Project Overview

This project demonstrates a simulated phishing investigation using CyberChef, a browser-based data analysis tool.

The investigation focuses on decoding suspicious text, examining potential phishing indicators, and documenting findings using a Security Operations Center (SOC) investigation workflow.

All examples use fictional training data. No live malicious websites or malware were accessed.

Investigation Objectives

* Decode an encoded URL.
* Identify potentially suspicious login-page characteristics.
* Decode a Base64-encoded message.
* Examine account-verification language.
* Document security findings and limitations.
* Recommend appropriate defensive actions.

Investigation 1: Suspicious URL Analysis

Tool: CyberChef
Operation: URL Decode

Encoded URL

https%3A%2F%2Faccount-verification.example%2Flogin%3Fuser%3Dadmin

Decoded URL

https://account-verification.example/login?user=admin

Findings

The decoded URL contains account-verification wording, a login path, and an administrator-related query parameter.

These characteristics could be relevant during a phishing investigation. However, the URL alone does not prove malicious activity.

The .example domain is reserved for documentation and was used as a safe training example.

Investigation 2: Base64 Message Analysis

Tool: CyberChef
Operation: From Base64

Encoded Message

VmVyaWZ5IHlvdXIgYWNjb3VudCBub3c=

Decoded Message

Verify your account now

Findings

The decoded message uses urgent account-verification language.

Such language can appear in phishing attempts intended to persuade recipients to visit login pages or disclose credentials.

Base64 encoding itself is not evidence of malicious intent.

Security Assessment

Case Type: Simulated Phishing Investigation
Assessment: Suspicious characteristics identified in fictional training samples
Confirmed Compromise: None
Malware Detected: None

The exercises demonstrate how decoding techniques can help analysts reveal and interpret potentially suspicious content.

Recommended Incident Response

1. Avoid opening unverified links.
2. Verify account-related messages through official communication channels.
3. Examine email headers and sender information.
4. Review relevant authentication logs when available.
5. Escalate suspicious activity for further investigation.
6. Document indicators and supporting evidence.

Tools and Skills Demonstrated

* CyberChef
* URL decoding
* Base64 decoding
* Phishing indicator identification
* Security investigation documentation
* Analytical reasoning
* SOC incident triage fundamentals

Project Evidence

Screenshots documenting the URL decoding and Base64 decoding exercises will be added to this repository.

Project Limitations

This is an educational simulation using fictional data. It does not represent an investigation of a real attack or a confirmed security incident.

About the Analyst

David Jeffries

Cybersecurity professional development focused on SOC analysis, security monitoring, incident investigation, and threat detection.

Certification: Google Cybersecurity Professional Certificate

GitHub: https://github.com/David31005

Cybersecurity Portfolio: https://github.com/David31005/cybersecurity-portfolio

LinkedIn: https://www.linkedin.com/in/david-jeffries001

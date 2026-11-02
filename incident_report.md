Security Investigation Report

Case ID: CYBERCHEF-001
Analyst: David Jeffries
Investigation Type: Simulated Phishing and Encoded Content Analysis
Tools Used: CyberChef
Status: Analysis Completed
Environment: Educational Security Lab

⸻

1. Executive Summary

This investigation examined two simulated phishing-related artifacts using CyberChef: a URL-encoded login link and a Base64-encoded account-verification message.

Both artifacts were decoded successfully. The results contained characteristics that could warrant additional investigation in a real security environment.

No live malware, malicious website, or actual compromise was identified.

2. Investigation Objectives

* Decode suspicious URL-encoded text.
* Analyze the resulting URL structure.
* Decode a Base64-encoded message.
* Identify possible phishing indicators.
* Document findings and recommend defensive actions.

3. Evidence Analysis

Evidence 1: URL-Encoded Link

Original artifact:

https%3A%2F%2Faccount-verification.example%2Flogin%3Fuser%3Dadmin

CyberChef operation: URL Decode

Decoded result:

https://account-verification.example/login?user=admin

Observations:

* The domain includes account-verification wording.
* The URL references a login page.
* The query string contains user=admin.
* URL encoding obscured some characters before decoding.
* The .example domain is reserved for documentation.

Assessment: The URL resembles a potential phishing login destination, but this fictional artifact is not evidence of a real attack.

Evidence 2: Base64-Encoded Message

Original artifact:

VmVyaWZ5IHlvdXIgYWNjb3VudCBub3c=

CyberChef operation: From Base64

Decoded result:

Verify your account now

Observations:

* The message requests account verification.
* The wording creates a sense of urgency.
* Such messaging can appear in credential-phishing campaigns.
* Base64 encoding is not inherently malicious.

Assessment: The decoded message demonstrates a potential phishing pretext in a simulated scenario.

4. Indicators and Findings

Indicator	Observation	Interpretation
URL encoding	Encoded URL characters	May obscure a destination
Account verification	Domain wording	Possible phishing pretext
Login path	/login	Potential credential-entry page
Admin parameter	user=admin	Administrator-related reference
Base64 encoding	Encoded message	Requires decoding to inspect
Urgent wording	“Verify your account now”	Possible social engineering

These indicators are contextual and do not independently confirm malicious activity.

5. Risk Assessment

Scenario Risk: Moderate, if similar content appeared in an unsolicited real-world email.

Confirmed Threat: None

Confirmed Compromise: None

Actual Malware Detected: None

The risk assessment is hypothetical because the investigation used simulated artifacts.

6. Recommended Response Actions

1. Do not open unverified links.
2. Confirm account-verification requests through official channels.
3. Review the original sender and email headers.
4. Examine authentication logs for unusual activity when available.
5. Escalate credible phishing indicators to the security team.
6. Document the evidence and investigation results.
7. Provide phishing-awareness guidance to affected users when appropriate.

7. Investigation Limitations

This project used fictional training data.

No live email headers, network traffic, endpoint telemetry, malware samples, or real authentication logs were examined.

Therefore, the investigation cannot establish that an actual phishing attack or account compromise occurred.

8. Conclusion

The investigation successfully demonstrated URL decoding and Base64 decoding using CyberChef.

Both exercises illustrate how security analysts can inspect encoded artifacts and assess possible phishing indicators.

The project demonstrates foundational SOC analysis, evidence documentation, and incident-triage skills.

⸻

Prepared by: David Jeffries
Portfolio: https://github.com/David31005/cybersecurity-portfolio
LinkedIn: https://www.linkedin.com/in/david-jeffries001

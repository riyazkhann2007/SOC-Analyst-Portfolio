Phishing Email Investigation

Project Objective

Investigate suspicious URLs and email headers to understand potential phishing threats using publicly available security tools.

Tools Used

- VirusTotal
- Gmail – Show Original
- Browser Developer Tools
- GitHub

Investigation 1: Example URL Analysis

URL: https://example.com

- HTTP Status: 200
- Vendor detections: 0
- Result: No security vendors flagged the URL in the observed scan.

Assessment: No malicious detection was reported in this scan. This does not guarantee the URL is risk-free.

Investigation 2: Controlled URL Threat Detection

URL: https://testsafebrowsing.appspot.com/

- Webroot: Malicious
- alphaMountain.ai: Suspicious
- Gridinsoft: Suspicious
- Other visible vendors: Clean

Assessment: This is a controlled security testing URL designed to demonstrate browser security warnings. Its detections should not be treated as evidence of a real-world phishing incident.

Investigation 3: Microsoft Learn URL Analysis

URL: https://learn.microsoft.com/en-gb/training/?wt.mc_id=rmskilling_learn_welcome_email_gdc

- Domain: learn.microsoft.com
- Protocol: HTTPS
- HTTP Status: 200
- VirusTotal vendor detections: 0 in the observed scan

Assessment: The URL points to a Microsoft Learn training page and showed no vendor detections in the observed scan. This alone does not guarantee safety.

Email Header Investigation

Sample: Microsoft Learn notification email

Sender: Learn@notifications.microsoft.com

Authentication Results:

- SPF: PASS
- DKIM: PASS
- DMARC: PASS

Header Analysis:

- Sending IP: 130.248.181.168
- Return-Path: bounce@notifications.microsoft.com
- Routing: Microsoft infrastructure to Google mail servers.

Initial Assessment: The email passed all three authentication checks, and its sender domain appears consistent with Microsoft notification infrastructure.

Final Verdict: Likely legitimate based on the available header evidence. Authentication results alone cannot guarantee that an email is safe.

Key Learnings

- Investigating URLs with VirusTotal.
- Understanding vendor detection results.
- Analysing email headers.
- Understanding SPF, DKIM and DMARC.
- Writing evidence-based investigation conclusions.

---

Screenshots and supporting evidence will be added to the evidence folder.
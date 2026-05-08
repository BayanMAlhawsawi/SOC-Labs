# 🚨 Phishing Analysis Report - Amazon Delivery Scam

## Incident Scenario

A suspicious inbound email was detected and flagged as a potential phishing attempt. The message claimed that an Amazon package could not be delivered and requested the recipient to confirm shipping information through an external link.

---

## Alert Details

- Data Source: Email
- Timestamp: 05/08/2026 06:03:15
- Subject: Your Amazon Package Couldn’t Be Delivered – Action Required
- Sender: urgents@amazon.biz
- Recipient: h.harris@thetrydaily.thm
- Attachment: None
- Direction: Inbound

---

## Email Content

The email requested the recipient to confirm shipping information through the following external link:

http://bit.ly/3sHkX3da12340

---

## Analysis

The email contains several phishing indicators commonly used in social engineering attacks.

- The sender domain (`amazon.biz`) is suspicious and does not match Amazon’s legitimate domain.
- The email uses urgent language to pressure the user into acting quickly.
- A shortened URL (`bit.ly`) was used to hide the real destination of the link.
- The message attempts to impersonate Amazon to gain the user’s trust.
- The external link may redirect the user to a fake login or credential harvesting page.

---

## Verdict

**True Positive – Phishing Attempt**

---

## Impact

If the user clicks the link, sensitive information such as login credentials, address details, or payment information could be stolen.

---

## Recommended Remediation Actions

- Block the sender/domain.
- Instruct the user not to interact with the email.
- Check proxy and firewall logs for access attempts.
- Remove the email from affected mailboxes if necessary.
- Educate users about phishing attacks and shortened URLs.

---

## Indicators of Compromise (IOCs)

- Suspicious sender domain: amazon.biz
- URL shortener: bit.ly
- Urgent language and delivery threat
- External phishing link
- Social engineering attempt impersonating Amazon

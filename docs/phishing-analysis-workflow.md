# Phishing Analysis Workflow

## Scenario

A user reports a suspicious email that appears to impersonate a known service and asks the user to click a link, open an attachment, reply with information, or enter credentials.

## 1. Confirm Report Details

Capture the basic context before changing anything:

- Who reported the message?
- When was it received?
- Did the user click, download, reply, or enter credentials?
- Was the message sent to one user or multiple users?
- Is the sender internal, external, or spoofed?

## 2. Preserve Evidence

Save enough information to support review and escalation:

- Sender address.
- Reply-to address.
- Subject line.
- Timestamp.
- URLs.
- Attachment names.
- Screenshots, if safe and sanitized.
- Headers, if available.

## 3. Review Sender and Header Indicators

Check for common signs of impersonation or spoofing:

- Display name mismatch.
- Sender domain mismatch.
- Reply-to mismatch.
- SPF failure.
- DKIM failure.
- DMARC failure.
- Unusual originating source.

## 4. Review Content Indicators

Look for message content that increases risk:

- Urgency or fear language.
- Credential request.
- Payment or gift card request.
- Unexpected attachment.
- Link text that does not match the destination.
- Brand impersonation.
- Poor grammar or unusual formatting.

## 5. Extract Indicators

Record indicators in a checklist:

- Sender email.
- Reply-to email.
- URLs.
- Domains.
- IP addresses.
- Attachment filenames.
- File hashes, if available.

## 6. Check Reputation Safely

Use safe reputation checks. Do not open suspicious links directly.

Possible checks:

- URL reputation lookup.
- Domain reputation lookup.
- Header analysis.
- Safe link preview.
- Attachment hash lookup if a hash is available.

## 7. Classify Risk

Use evidence and user action to classify the report.

| Level | Criteria |
|---|---|
| Low | Suspicious message, no user interaction, no confirmed malicious payload |
| Medium | Credible phishing attempt, no credential entry or attachment execution confirmed |
| High | User clicked, entered credentials, opened attachment, or multiple users received it |

## 8. Escalate When Needed

Escalate when there is evidence of:

- Credential entry.
- Attachment opened.
- Malware indicators.
- Multiple recipients.
- Executive, finance, HR, or privileged user targeted.
- Confirmed malicious URL or domain.

## 9. Response Actions

Possible response steps:

- Advise user not to interact.
- Reset password if credentials were entered.
- Revoke active sessions if needed.
- Block sender, domain, or URL if confirmed malicious.
- Search for other recipients.
- Preserve evidence for escalation.
- Document final status.

## 10. Lessons Learned

Record the operational lesson:

- What indicator mattered most?
- What control would reduce recurrence?
- What user education point applies?
- What should be improved in the process?

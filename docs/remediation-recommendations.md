# Remediation Recommendations

## Immediate User Guidance

- Do not click the link.
- Do not reply to the sender.
- Do not download or open attachments.
- Report similar messages immediately.
- Confirm whether credentials were entered.

## Microsoft 365 Containment

Recommended actions depend on access level and approval:

- Search for similar messages across mailboxes.
- Quarantine or remove matching messages where authorized.
- Block confirmed malicious sender, domain, or URL.
- Reset password if credentials were entered.
- Revoke user sessions if compromise is possible.
- Review Entra ID sign-in logs for suspicious activity.
- Review mailbox forwarding and inbox rules if compromise is suspected.

## Attachment Handling

If an attachment was opened:

- Isolate the endpoint if malware is suspected.
- Preserve the file name and hash if available.
- Submit hash or file to approved analysis process.
- Review endpoint alerts if available.
- Escalate to security or endpoint support.

## Preventive Improvements

- Improve phishing reporting process visibility.
- Reinforce user training around credential prompts.
- Enable or tune anti-phishing controls where available.
- Review external sender tagging.
- Review MFA enforcement.
- Review conditional access policies if appropriate.
- Build a standard incident note template.

## Junior Analyst Recommendation Style

Use cautious, evidence-based wording:

- "Based on the reviewed indicators, this appears suspicious."
- "Recommend searching for additional recipients."
- "Recommend password reset if the user entered credentials."
- "Recommend escalation if attachment execution or credential entry is confirmed."

Avoid overstating:

- Do not claim confirmed malware without evidence.
- Do not claim account compromise without logs.
- Do not claim campaign-wide impact without recipient search.

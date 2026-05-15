# Incident Notes Sample

## Case Summary

User reported a suspicious email claiming to be a Microsoft 365 password expiration notice. The email requested account verification through a non-Microsoft URL.

## Incident Details

| Field | Entry |
|---|---|
| Date/time reported | 2026-05-15 09:05 |
| Reporter | User-reported suspicious email |
| User action taken | User reported before entering credentials |
| Initial classification | Medium |
| Evidence reviewed | Sender, reply-to, subject, URL, sample header indicators |
| Sender email | `security-alert@example-training.com` |
| Reply-to email | `support@example-training.com` |
| URL/domain | `hxxps://m365-verify.example[.]com/login` |
| Attachment | None |
| Header review | SPF fail, DKIM none, DMARC fail in sanitized sample |
| Escalation needed | Yes if credential entry or additional recipients are confirmed |
| Containment recommendation | Search for similar messages, block confirmed malicious URL/domain, advise user not to interact |
| Final status | Documented as suspicious phishing attempt in sample |

## Analyst Summary

The email uses Microsoft 365 branding and urgency language to push account verification. The sender and reply-to do not match a legitimate Microsoft domain, and the URL points to a suspicious domain. No credential entry was confirmed, so the case is documented as medium risk in this sample.

## Recommended Next Steps

- Search for additional recipients.
- Block sender/domain/URL if confirmed malicious.
- Reset password and revoke sessions if any user entered credentials.
- Document results and close or escalate based on recipient scope.

# Analyst Timeline Walkthrough

## Scenario

A user reports a suspicious Microsoft 365 password reset email. The user has not confirmed clicking the link.

## Timeline

| Time | Action | Result |
|---|---|---|
| 09:05 | User reports suspicious email | Report accepted for review |
| 09:07 | Analyst confirms user did not enter credentials | Initial risk reduced from high to medium |
| 09:10 | Analyst preserves sender, subject, timestamp, URL, and screenshot | Evidence recorded |
| 09:14 | Analyst reviews sender and reply-to | Sender domain does not match Microsoft |
| 09:18 | Analyst reviews authentication indicators | SPF/DKIM/DMARC results documented from sample header |
| 09:22 | Analyst extracts URL/domain IOC | Suspicious domain recorded |
| 09:26 | Analyst checks URL reputation safely | Suspicious reputation noted in sample |
| 09:30 | Analyst classifies risk as medium | No credential entry or attachment execution confirmed |
| 09:35 | Analyst recommends sender/domain block and recipient search | Containment recommendation documented |
| 09:40 | Analyst writes final incident notes | Case ready for escalation or closure |

## Analyst Reasoning

The message was treated as a credible phishing attempt because it used Microsoft 365 branding, requested account verification, and linked to a non-Microsoft domain. Risk was not classified as high because the user did not confirm credential entry, no attachment was opened, and no broader recipient scope was confirmed in the sample.

## Escalation Trigger

Escalate immediately if:

- The user entered credentials.
- The link was opened on a corporate endpoint.
- More recipients are identified.
- Suspicious sign-ins appear after delivery.
- The email contains an attachment that was opened.

# IOC Extraction Example

## Source

Sample 01: Microsoft 365 Password Reset Phish

## Extracted Indicators

| Indicator Type | Value | Notes |
|---|---|---|
| Sender email | `security-alert@example-training.com` | Non-Microsoft sender |
| Reply-to | `support@example-training.com` | Does not match claimed Microsoft identity |
| Subject | `Action Required: Password Expiration Notice` | Urgency language |
| URL | `hxxps://m365-verify.example[.]com/login` | Defanged sample URL |
| Domain | `m365-verify.example[.]com` | Suspicious brand impersonation |
| Attachment | None | No attachment in this sample |
| User action | Reported before credential entry | Lowers immediate impact |

## Analyst Note

The key IOC is the credential-harvesting URL. The sender and reply-to also support the phishing assessment because they do not align with a legitimate Microsoft domain.

## Classification Support

Medium risk is appropriate because the email includes credential phishing indicators, but no credential entry or attachment execution was confirmed.

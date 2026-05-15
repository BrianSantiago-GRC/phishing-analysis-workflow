# Escalation Summary

## When To Escalate

Escalate the case if any of the following are confirmed:

- User clicked the link.
- User entered credentials.
- Attachment was opened.
- Multiple recipients received the message.
- Sender/domain/URL is confirmed malicious.
- A privileged user, finance user, HR user, or executive was targeted.
- Suspicious sign-ins appear after delivery.

## Escalation Message Example

```text
Summary:
User reported a suspicious Microsoft 365 password expiration email. Message used non-Microsoft sender domain and directed user to a suspicious verification URL.

Current impact:
User reported before entering credentials. No attachment observed. Recipient scope not yet confirmed.

Indicators:
- Sender: security-alert@example-training.com
- Reply-to: support@example-training.com
- URL: hxxps://m365-verify.example[.]com/login
- Subject: Action Required: Password Expiration Notice

Recommended actions:
- Search for additional recipients.
- Block confirmed malicious URL/domain if validated.
- Reset password and revoke sessions if credential entry is later confirmed.
```

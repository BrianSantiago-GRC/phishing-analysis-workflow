# Investigation Workflow

## Purpose

This workflow shows a realistic junior analyst process for reviewing a user-reported suspicious email.

## 1. Intake

Collect the basic report details:

| Question | Why It Matters |
|---|---|
| Who reported the email? | Identifies impacted user and follow-up owner |
| When was it received? | Helps determine search window |
| Did the user click? | Drives containment priority |
| Did the user enter credentials? | May require password reset and session revocation |
| Was an attachment opened? | May require endpoint review |
| Did other users receive it? | Determines whether this is isolated or broader |

## 2. Preserve Evidence

Preserve enough information to support triage:

- Email screenshot.
- Sender address.
- Reply-to address.
- Subject line.
- Timestamp.
- Full headers, if available.
- URLs.
- Attachment names.
- Attachment hashes, if available.

Do not click suspicious links directly. Do not download or open suspicious attachments on a normal workstation.

## 3. Review Sender and Header Indicators

Check:

- Display name mismatch.
- Sender domain mismatch.
- Reply-to mismatch.
- SPF result.
- DKIM result.
- DMARC result.
- Originating IP or relay path.
- Unusual mail routing.

## 4. Review Message Content

Look for:

- Urgency or fear language.
- Credential request.
- Unexpected invoice or document.
- External file-sharing link.
- Link text that does not match destination.
- Brand impersonation.
- Unusual grammar or formatting.

## 5. Extract IOCs

Record:

- Sender email.
- Reply-to email.
- Domains.
- URLs.
- IP addresses.
- Attachment names.
- File hashes.
- Subject line.

## 6. Check Reputation Safely

Use safe lookups:

- URL/domain reputation tools.
- Header analyzer.
- Attachment hash lookup.
- Microsoft 365 / Defender review, if available.

Avoid opening the link or executing the attachment.

## 7. Classify Risk

| Risk | Criteria |
|---|---|
| Low | Suspicious but no user interaction and no confirmed malicious indicator |
| Medium | Credible phishing indicators, but no credential entry or attachment execution confirmed |
| High | User clicked, entered credentials, opened attachment, or campaign affected multiple users |

## 8. Containment Recommendation

Recommend actions based on evidence:

- Tell user not to interact.
- Block sender/domain/URL if confirmed malicious.
- Search for additional recipients.
- Reset password if credentials were entered.
- Revoke sessions if credentials may be exposed.
- Review endpoint if attachment was opened.
- Escalate to security team or senior analyst when impact is confirmed.

## 9. Document Findings

Final notes should explain:

- What was reported.
- What evidence was reviewed.
- Which indicators were suspicious.
- What risk level was assigned.
- What actions were recommended.
- What remains unresolved.

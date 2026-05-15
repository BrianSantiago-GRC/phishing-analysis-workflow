# Sample Phishing Analysis

> Sample note: This is a sanitized example used to demonstrate the workflow. It does not include real user data, real tenant data, or private organization information.

## Report Summary

| Field | Entry |
|---|---|
| Date reviewed | 2026-05-15 |
| Reporter | User-reported suspicious email |
| Scenario | Email impersonates a known service and asks the user to verify account access |
| User action | No credential entry confirmed |
| Initial classification | Medium |

## Evidence Reviewed

- Sender display name.
- Sender address.
- Reply-to address.
- Subject line.
- Visible link text.
- Destination domain.
- Message urgency.
- Header authentication concepts.

## Indicators

| Indicator | Value | Notes |
|---|---|---|
| Sender email | `security-alert@example-training.com` | Placeholder value |
| Reply-to | `support@example-training.com` | Placeholder value |
| Subject | `Action required: verify your account` | Urgency language |
| URL/domain | `example-training-login.com` | Placeholder value |
| Attachment | None observed | No attachment in sample |
| IP address | Not recorded | Not available in sample |
| Hash | N/A | No attachment |

## Findings

- The email used urgency to push account verification.
- The visible brand language did not match the placeholder sender domain.
- The message requested account action through a link.
- No attachment was present in the sample.
- No credential entry was confirmed.

## Risk Classification

Classification: Medium

Reason: The message showed credible phishing indicators, but there was no confirmed credential entry, attachment execution, or broader recipient impact in the sample.

## Recommended Response

- Advise the user not to click the link or reply.
- Preserve the email and headers if available.
- Check for additional recipients.
- Block the sender/domain if confirmed malicious by reputation review.
- Escalate if any user clicked or entered credentials.

## Lessons Learned

The most important part of phishing triage is not guessing from one indicator. A reliable review preserves evidence, checks sender and link details, records IOCs, identifies user action, and documents why the risk level was selected.

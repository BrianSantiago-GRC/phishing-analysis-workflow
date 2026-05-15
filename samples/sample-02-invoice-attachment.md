# Sample 02: Invoice Attachment Phish

> Sample note: This is a sanitized training example. It does not contain real user, employer, tenant, or customer information.

## Scenario

A user receives an unexpected invoice email with an attachment. The message claims payment is overdue and asks the user to review the document immediately.

## Observed Details

| Field | Sample Value |
|---|---|
| Display name | Accounts Receivable |
| Sender | `billing@example-vendor-support.com` |
| Reply-to | `paymentdesk@example-vendor-support.com` |
| Subject | `Overdue Invoice - Immediate Review Required` |
| Attachment | `Invoice_Review_0515.html` |
| Link | None visible in body |
| User action | Attachment not opened |

## Suspicious Indicators

- Unexpected invoice.
- Urgent payment pressure.
- HTML attachment.
- Sender domain is not a known vendor domain in the sample.
- Business process pressure targeting finance/payment behavior.

## Initial Classification

Medium risk.

Reason: Suspicious attachment and social engineering indicators are present, but the attachment was not opened.

## Recommended Action

- Do not open the attachment.
- Preserve the message.
- Record attachment name.
- Hash the file only through an approved safe process.
- Check whether other users received similar messages.
- Escalate if the attachment was opened or endpoint alerts appear.

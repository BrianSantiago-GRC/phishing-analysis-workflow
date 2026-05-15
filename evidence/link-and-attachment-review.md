# Link and Attachment Review

## Suspicious Link Review

Scenario URL:

`hxxps://m365-verify.example[.]com/login`

Review points:

- Visible link text claims account verification.
- Destination domain does not match Microsoft.
- Domain uses brand-like wording to create trust.
- Link should not be opened directly.
- Reputation should be checked through a safe lookup process.

Analyst note:

The suspicious link is the strongest indicator in Scenario 01 because it appears designed for credential collection.

## Attachment Review

Scenario attachment:

`Invoice_Review_0515.html`

Review points:

- Unexpected attachment.
- HTML file type can be used to redirect users to credential pages.
- User did not open the attachment in the scenario.
- Do not open on a normal workstation.
- Record the filename and obtain a hash only through an approved safe process.

Analyst note:

The attachment increases concern in Scenario 02, but risk remains medium unless the file is opened, malware indicators are confirmed, or additional recipients are found.

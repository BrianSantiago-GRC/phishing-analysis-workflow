# Phishing Analysis Workflow

Practical phishing triage workflow from an IT support and junior security operations perspective.

This project documents how I would review a suspicious email report, preserve evidence, identify indicators, check reputation safely, classify risk, and document the response. It is meant to show operational thinking, clear documentation, and security-aware troubleshooting.

## Purpose

The purpose of this project is to demonstrate a repeatable phishing analysis process that can be used by an IT support or junior SOC analyst candidate.

## What I Practiced

- Reviewing suspicious email reports.
- Preserving basic evidence before taking action.
- Checking sender, reply-to, link, attachment, and header indicators.
- Reviewing SPF, DKIM, and DMARC concepts.
- Extracting indicators of compromise.
- Checking domain and URL reputation safely.
- Classifying risk based on user action and evidence.
- Writing concise incident notes and escalation recommendations.

## Tools and Concepts

- Email header review.
- SPF, DKIM, and DMARC.
- URL and domain reputation checks.
- IOC tracking.
- Incident notes.
- Microsoft 365 and email security concepts.
- Safe analysis practices.

## Workflow

The full workflow is documented here:

- [Phishing Analysis Workflow](docs/phishing-analysis-workflow.md)

## Sample Documentation

- [Sample Analysis](samples/sample-phishing-analysis.md)
- [IOC Checklist](templates/ioc-checklist.md)
- [Incident Notes Template](templates/incident-notes-template.md)

## Screenshots

Screenshot placeholders are organized here:

- [Screenshots](screenshots/README.md)

Screenshots should be added only after they are sanitized. Do not include real email addresses, private links, tenant details, message IDs, IP addresses, or user information.

## Skills Demonstrated

- Security operations documentation.
- Phishing triage fundamentals.
- Evidence handling discipline.
- IOC extraction.
- Risk classification.
- Clear escalation notes.
- Practical IT-to-security transition work.

## Limitations

This is a portfolio workflow and documentation project. It does not claim advanced malware analysis, threat hunting, or ownership of an enterprise phishing response program.

## Next Improvement

- Add sanitized screenshots from the completed workflow.
- Add one more sample using a benign training email.
- Connect the workflow to a Microsoft Defender or Microsoft 365 investigation example if available.

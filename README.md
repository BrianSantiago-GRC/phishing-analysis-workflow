# Phishing Analysis Workflow

Portfolio project for a junior SOC / security operations role.

This project documents a practical phishing investigation workflow using a Microsoft 365 context. It shows how a junior analyst or IT support professional can receive a user-reported suspicious email, preserve evidence, review headers and links, extract indicators, classify risk, recommend containment, and write clear incident notes.

## Positioning

This is a hands-on learning and documentation project. It stays within junior analyst triage, documentation, and escalation practice.

## Project Goals

- Demonstrate phishing triage fundamentals.
- Show operational documentation discipline.
- Practice Microsoft 365 email security concepts.
- Build interview-defensible SOC examples.
- Create screenshot-friendly artifacts for GitHub and LinkedIn.

## Project Structure

| Folder | Purpose |
|---|---|
| `docs` | Investigation workflow, Microsoft 365 context, analyst timeline, and remediation guidance |
| `samples` | Sanitized phishing sample scenarios |
| `evidence` | IOC extraction and header/link/attachment review examples |
| `incident_notes` | Sample incident notes and escalation summary |
| `templates` | Reusable IOC, intake, and incident note templates |
| `screenshots` | Screenshot checklist and placeholders |
| `linkedin` | LinkedIn-ready project summary |

## Core Workflow

1. Receive user report.
2. Preserve evidence.
3. Review sender, headers, links, and attachments.
4. Extract indicators of compromise.
5. Check reputation safely.
6. Classify risk.
7. Recommend containment.
8. Document findings.
9. Capture lessons learned.

## Key Artifacts

- [Investigation Workflow](docs/investigation-workflow.md)
- [Microsoft 365 Phishing Context](docs/microsoft-365-context.md)
- [Analyst Timeline Walkthrough](docs/analyst-timeline-walkthrough.md)
- [Remediation Recommendations](docs/remediation-recommendations.md)
- [Lessons Learned](docs/lessons-learned.md)
- [IOC Extraction Example](evidence/ioc-extraction-example.md)
- [Email Header Analysis Example](evidence/email-header-analysis-example.md)
- [Suspicious Link and Attachment Review](evidence/link-and-attachment-review.md)
- [Sample Incident Notes](incident_notes/incident-notes-sample.md)

## Screenshot Status

Screenshots are not included yet. The project is structured so screenshots can be added without rewriting the documentation.

Needed screenshots:

- User-reported phishing email example.
- Email header or authentication results.
- Suspicious URL reputation check.
- Attachment review or hash lookup, if applicable.
- Completed IOC checklist.
- Completed incident notes.

## Interview Talking Point

"I built a phishing analysis workflow to practice junior SOC triage. The project walks through user reporting, evidence preservation, Microsoft 365 email context, header review, IOC extraction, safe reputation checks, risk classification, containment recommendations, and incident documentation."

## Next Improvements

- Add sanitized screenshots.
- Add a Microsoft Defender / Microsoft 365 review example if available.
- Add one more sample showing credential entry and session revocation steps.

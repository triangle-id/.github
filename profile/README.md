# Triangle ID

**Verifiable proof of employment history.**

Triangle ID is building the infrastructure to combat employment fraud. We issue cryptographically signed employment credentials that job seekers can present to recruitment platforms, verified instantly, without contacting the employer.

## How it works

Employers issue verifiable credentials to former employees through our dashboard. The credential is an SD-JWT VC signed by the employer's decentralized identifier (DID). Job seekers store their credentials locally and present them to employment platforms via an embeddable verification widget. The platform verifies the cryptographic signature in seconds. No phone calls, no reference checks, no waiting.

## Repositories

Repos are coming soon. The project is in early build phase.

| Repo | Description |
|------|-------------|
| sdk | Forked from Credo-TS. Handles DID resolution, SD-JWT VC issuance, and credential verification. |
| dashboard | Employer-facing web app for issuing employment credentials. |
| widget | Embeddable JS widget for employment platforms to verify credentials. |
| web | Landing page at [triangle.id](https://triangle.id). |

## Tech stack

- **Credential format:** SD-JWT VC (RFC 9901)
- **Employer identity:** did:web
- **User identity:** did:key derived from passkeys (WebAuthn)
- **SDK foundation:** Credo-TS (Open Wallet Foundation)
- **Verification:** Embeddable JS widget + REST API

## The problem

AI-generated CVs and fabricated employment histories are flooding recruitment platforms. Verifying a candidate's claims is slow, manual, and expensive. Bad hires cost companies an average of 30% of the employee's first-year salary.

Triangle ID gives people a way to prove where they've worked, and gives platforms a way to trust that proof.

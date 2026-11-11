# Dossier

**Turn your business documents into a persuasive proposal with facts you can trace.**

Dossier is a Uliya skill for UGREEN AI NAS. Give it a short business brief, an intended recipient, and selected company documents. It organizes the relevant facts, writes a professional proposal, checks the claims against your sources, and saves the draft after your approval.

Dossier presents your offering favorably while preserving factual accuracy. It produces proposals; it does not score business ideas or tell you whether to pursue them.

## Status

**Initial hackathon package; NAS runtime testing pending.** The official UGREEN creation toolkit reports `static-pass` with **zero errors and zero warnings**. Static checks verify package structure and supported orchestration patterns. They do not prove installation, local model routing, device execution, or hackathon acceptance.

The entry is being prepared for **UGREEN Hackathon 2026 — Automate Your Workflow**. A [Devpost project page](https://devpost.com/software/dossier-whruys) now exists and the representative is registered. The UGREEN entry remains unsubmitted; nothing has been published to SkillHub.

## What it does

- Uses a brief and an explicitly selected set of NAS documents, such as a company profile, service description, price list, or existing market report.
- Extracts offerings, benefits, terms, prices, and relevant supporting evidence.
- Drafts a proposal tailored to the business field, purpose, and recipient.
- Preserves source references and material qualifications.
- Asks about conflicting facts rather than choosing a convenient figure.
- Saves the reviewed text to an authorized destination after confirmation, then checks completion evidence.

The first release produces **proposal text**. It does not browse the web, guarantee current market statistics, generate charts, embed photos, provide designed PDF export, or send proposals externally. The PDF in this repository describes the hackathon project; it is not an example of an export feature available inside the skill.

## Intended use

Dossier requires a compatible Uliya host with `file-agent`, `document-agent`, and `knowledge-agent`; authorized source documents; and permission to save text. Supported document and output formats must be verified on the actual device. No mobile compatibility claim is made yet.

Obtain the skill folder or the initial skill ZIP below. Use the installation or import method supported by your Uliya environment; do not execute the Markdown as a script. Installation and invocation steps will be documented after real-device validation.

Once installed, an example request is:

> Dossier, draft a proposal for our cleaning service for a prospective office client. Use only the company profile and price list I select. Save the reviewed text in the proposal folder I authorize.

Supply the brief, recipient or purpose, chosen source files or folder, and destination. Dossier resolves the source set, gathers evidence, drafts and reviews the text, then asks you to confirm the concrete result before saving. Missing documents or material contradictions pause the workflow.

Use synthetic or appropriately anonymized materials for hackathon testing. Never upload private business documents, credentials, or customer information to this repository.

## Team

- [interplanetarysister](https://github.com/interplanetarysister): project owner and authorized team representative.
- [CloudNyne](https://github.com/Cloudnyne): team partner. GitHub collaborator access and Devpost team joining are pending.

## Skill workflow

| Stage | Registered expert | Published capability |
| --- | --- | --- |
| Discover authorized sources and verify output | `file-agent` | `ug-filesystem` |
| Extract evidence, draft, and check claims | `document-agent` | `ug-document` |
| Save the approved proposal text | `knowledge-agent` | `ug-knowledge` |

The parent skill delegates; it does not run custom scripts, make direct network calls, or access NAS resources directly. Source documents are treated as reference data, and their embedded instructions cannot authorize new actions. Empty results, partial extraction, cancellation, permission requests, and save failures have explicit handling.

Processing must remain local. If the host cannot ensure local routing, Dossier stops rather than sending source material to an external service. Source files remain unchanged. No background updater, analytics, paid API, premium builder, or third-party research service is required by the skill. A compatible host and hardware may still have costs.

## Repository contents

```text
Dossier/
├── README.md
├── LICENSE
├── THIRD_PARTY_NOTICES.md
├── .gitignore
├── skills/dossier/
│   ├── SKILL.md
│   └── references/
│       ├── proposal-structure.md
│       ├── evidence-rules.md
│       ├── disclosures-and-validation.md
│       ├── license.md
│       └── third-party-notices.md
├── docs/
│   ├── implementation-plan.md
│   └── validation.md
└── submission/
    ├── project-proposal.md
    ├── Dossier-Project-Proposal.pdf
    ├── Dossier-Initial-Skill.zip
    ├── static-check.json
    ├── artifact-checks.json
    ├── checklist.md
    ├── custom-answers.json
    └── form-status.md
```

Start with the [skill entry point](skills/dossier/SKILL.md), [implementation plan](docs/implementation-plan.md), and [validation record](docs/validation.md).

## Round 1 submission materials

Download the [skill ZIP](https://github.com/interplanetarysister/Dossier/raw/refs/heads/main/submission/Dossier-Initial-Skill.zip) and [proposal PDF](https://github.com/interplanetarysister/Dossier/raw/refs/heads/main/submission/Dossier-Project-Proposal.pdf) directly from the repository. Use the named skill ZIP rather than GitHub's source-code archive. See [finish the entry](submission/finish-entry.md) for the remaining web-form steps.

- [Project proposal PDF](submission/Dossier-Project-Proposal.pdf): answers the ten required questions; the substantive responses total 318 words.
- [Initial skill ZIP](submission/Dossier-Initial-Skill.zip): the skill entry point and five linked Markdown references, including the full license and third-party notices.
- [Submission checklist](submission/checklist.md): remaining owner review, eligibility, registration, and submission steps.
- [Checker output](submission/static-check.json) and [artifact checks](submission/artifact-checks.json): validation results, sizes, and hashes.

Only `SKILL.md` and the linked `references/` files belong inside the skill ZIP. Repository documentation, the PDF, and checker JSON stay outside it. Do not upload the entire repository as the skill package.

Round 1 closes **November 15, 2026, at 11:45 p.m. Pacific**. A public repository, NAS purchase, and demo video are not required for Round 1. Registration and the representative’s eligibility confirmation are complete. The proposal PDF is attached to the Devpost draft. CloudNyne must join the project, the ZIP must be attached through the web form, and the remaining custom answers must be saved before final entry. See [form status](submission/form-status.md).

Official sources: [requirements](https://ugreenhackathon.devpost.com/), [rules](https://ugreenhackathon.devpost.com/rules), [technical FAQ](https://ugreenhackathon.devpost.com/resources), and [starter kit](https://ai.ugreen.com/pages/hackathon-starter-kit).

## Validation and further work

The official `uliya-skill-kit` 0.7.3-en is obtained separately under UGREEN's terms. Its controlled checker is run in the development environment against `skills/dossier/`; the toolkit is not redistributed or included in the skill ZIP.

If selected, validate the same project on the assigned NAS. The two core cases cover exact facts and prices, then revision without changing sources or silently overwriting a prior output. The edge case covers conflicting prices. Device checks also cover approvals, cancellation, local routing, source-instruction injection, partial evidence, and saved-text verification.

Any addition of live research, image interpretation, chart rendering, designed export, or mobile support requires a fresh capability check and real-device validation. Do not advertise planned features as working behavior.

## License and third-party material

Original Dossier skill and repository material is licensed **GNU AGPL version 3 only (`AGPL-3.0-only`)**, consistent with the license selected when this repository was created. See [LICENSE](LICENSE). The full license is also included inside the skill ZIP as [references/license.md](skills/dossier/references/license.md).

You may use, study, modify, and redistribute Dossier under that license. Distribution must preserve applicable notices and provide corresponding source as required. Modified versions used to interact with users over a network must meet section 13's source-access requirements. The license permits commercial use and does not require everyone to provide free hosting. Dossier is provided without warranty.

The license does not grant rights to user-supplied documents or relicense UGREEN, its toolkit, a host model, or other third-party tools. Generated proposals are not automatically AGPL-covered merely because the skill was used; copying protected skill material into an output may raise separate obligations.

[Third-party notices](THIRD_PARTY_NOTICES.md) identify the UGREEN toolkit, ReportLab used to prepare the submission PDF, AI assistance, and their roles. No third-party runtime library, model, dataset, font, or image is bundled in the skill. UGREEN's toolkit terms and host access conditions remain separate. The use of AGPL is not a claim that UGREEN has approved the project for publication.

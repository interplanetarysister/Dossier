# Dossier — saved Devpost write-up

## 1. What does the Skill do?

Dossier turns a business brief and selected NAS documents into a persuasive professional proposal draft with traceable supporting facts.

## 2. Who is your target user, and what is their problem?

Small business owners and independent professionals have useful company information scattered across documents but need a coherent proposal tailored to a recipient.

## 3. What is your solution?

A single Uliya skill extracts relevant evidence, foregrounds documented benefits, drafts a proposal, reviews factual claims, and saves approved text. It produces proposals, not business advice.

## 4. What is the main user flow?

Provide a brief, recipient, authorized source documents, and destination. Resolve missing or conflicting details. Review the proposal, confirm saving, and receive its verified output location.

## 5. How is your idea different from existing tools or common AI solutions?

Dossier combines persuasive writing with traceability to private NAS source material. It preserves prices, qualifications, and source references rather than treating a generic prompt as sufficient evidence.

## 6. Which UGREEN AI NAS features does your Skill use, and at which step?

File discovery identifies authorized sources. Document extraction and question answering establish evidence. Document writing drafts and checks claims. Text saving stores the reviewed result.

## 7. What is your technical approach?

A Markdown-only SKILL.md orchestrates file-agent through ug-filesystem, document-agent through ug-document, and knowledge-agent through ug-knowledge. Each delegation includes concrete inputs and consumes verified completed results. Source documents remain unchanged. Processing must remain local; otherwise the workflow stops. Saving requires authorization and verification. No external API, paid integration, custom runtime, or bundled model is required. Local model availability is pending device validation.

## 8. What have you built so far? What is not built yet? What still needs testing on a NAS?

The skill and linked references are authored. The official toolkit checker reports static-pass with zero errors and warnings. NAS installation, local routing, real document processing, and output behavior remain untested pending finalist access.

## 9. How will you test your Skill if you become a Finalist? Name two core test cases and one edge case.

Core case one: draft from a synthetic company profile and price list, preserving exact facts and verified saving. Core case two: revise the brief and create a separate output without changing sources. Edge case: conflicting prices trigger clarification instead of invented figures.

## 10. What are the known limits, risks, or outside dependencies of your Skill?

Requires compatible Uliya experts and authorized source files. No live research, guaranteed source freshness, generated charts, embedded photos, designed PDF export, or confirmed mobile support. Host access and hardware are not promised free. Runtime formats and reliability require NAS testing.

## Third-party and AI disclosures

Development uses UGREEN's official uliya-skill-kit 0.7.3-en, catalog 2.0.0, under UGREEN's applicable agreements; it is not redistributed. Source: https://ai.ugreen.com/pages/hackathon-starter-kit. No third-party runtime libraries, datasets, images, or models are bundled. Original Dossier files use AGPL-3.0-only. Codex/OpenAI assisted authoring, implementation, checks and submission preparation; Exa retrieved official requirements. Acumen supported preliminary feasibility research only. ReportLab 4.4.9 (BSD-style license; reportlab.com) renders this PDF during development only and is not bundled. No external runtime service or data flow is introduced. No retrieved personal writing-style match is claimed.

## Confirmed entry and registration answers

- Submitter type: Team of individuals.
- Team members: interplanetarysister and CloudNyne. The representative has confirmed authorization to act for the two-person team; CloudNyne must join the Devpost project separately.
- Country of residence: United States for both team members.
- Track: Automate Your Workflow.
- Development start date: 11-11-26.
- Have you used a NAS before? I have never used a NAS.
- Have you built with local or self-hosted AI before? No, this is my first time.

## Entry files and status

Repository: https://github.com/interplanetarysister/Dossier

Initial skill ZIP: https://github.com/interplanetarysister/Dossier/raw/refs/heads/main/submission/Dossier-Initial-Skill.zip

Project proposal PDF: https://github.com/interplanetarysister/Dossier/raw/refs/heads/main/submission/Dossier-Project-Proposal.pdf

The proposal PDF is attached to the Devpost draft. The required ZIP must be uploaded through the official website: Devpost rejected final submission because that attachment is missing. A download link does not replace the required attachment. The custom entry answers above are recorded here in the project write-up; their persistence in the separate submission form has not been verified. This entry is not yet submitted.


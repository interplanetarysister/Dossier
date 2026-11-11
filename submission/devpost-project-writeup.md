# Dossier — saved Devpost write-up

## Dossier: a stronger proposal, grounded in your own documents

Your business already has useful material: a company profile, a service description, a price list, and perhaps customer requirements or existing research. Dossier is designed to turn those scattered files into a clear, persuasive business proposal while keeping its factual claims connected to their sources.

Give it a short brief, identify the intended recipient, choose the documents it may use, and select an output location. Its authored workflow brings the evidence together, foregrounds the offering's supported strengths, reviews the draft, and saves approved proposal text. Real NAS execution remains pending validation.

## 1. What does your Skill do?

Dossier turns a business brief and selected NAS documents into a persuasive professional proposal draft with traceable supporting facts.

## 2. Who is your target user, and what is their problem?

Small business owners, independent professionals, and small teams often have the information needed for a proposal spread across several documents. Turning it into a coherent presentation takes repeated reading, copying, checking, and rewriting.

Dossier focuses on producing the proposal. It does not score the idea, evaluate business viability, or provide unsolicited business advice.

## 3. What is your solution?

A single Markdown-based Uliya skill coordinates document discovery, evidence extraction, drafting, factual review, and approved saving. It presents the user's offering favorably through accurate, relevant evidence.

The intended draft can include an executive summary, customer need, offering, benefits, documented differences, supplied commercial terms, a next step, and source notes. Sections are included only when the brief and supporting materials justify them. Vocabulary and headings adapt to the business field; elaborate visual document design is outside this release.

## 4. What is the main user flow?

1. Describe the offering and recipient. Select the source documents and authorize the output destination.
2. Resolve the source set. Dossier identifies actual files within the selected scope.
3. Extract evidence. Preserve facts, prices, units, dates, qualifications, and available source references.
4. Draft and review. Create an opportunity-led proposal, then check factual claims against that evidence.
5. Approve and save. Show the concrete text before saving, and report the actual output path only after verification.

For large folders, the skill asks the user to narrow the set to at most twenty documents. This is Dossier's usability limit, not a claimed UGREEN platform limit.

## 5. How is your idea different from existing tools or common AI solutions?

Dossier combines proposal writing with an explicit evidence workflow over authorized NAS materials. The instructions require source references and preserve commercial details rather than relying on a general writing prompt alone.

For example, the repository's fictional office-cleaning illustration uses a documented USD 360 monthly plan with two visits, a defined scope, and exclusions. The proposal highlights those concrete strengths without inventing clients, certifications, market demand, or competitor weaknesses.

That example is manually authored reference material, not output from a tested Uliya run:
https://github.com/interplanetarysister/Dossier/tree/main/examples

## 6. Which UGREEN AI NAS features does your Skill use, and at which step?

| Stage | Published capability | Registered expert |
| --- | --- | --- |
| Discover selected sources and check saved output | ug-filesystem | file-agent |
| Extract facts, answer source questions, draft, and review | ug-document | document-agent |
| Save the approved text | ug-knowledge | knowledge-agent |

The NAS provides the intended private document library and output storage. These mappings come from the official toolkit's published catalog; their actual runtime behavior still requires device testing.

## 7. What is your technical approach?

The package contains SKILL.md and five directly linked Markdown references covering structure, evidence rules, disclosures, licensing, and third-party notices. It includes no custom runtime, executable scripts, model weights, datasets, fonts, or images.

Each delegation must contain concrete inputs and constraints. Dependent steps consume real results from completed expert operations. Source documents are treated as reference data, not instructions that can expand permissions or redirect the workflow.

The authored behavior requires local processing. If local routing cannot be ensured, it stops rather than transmitting the source documents externally. Actual routing must be verified on the NAS. No specific model or free host access is promised.

Empty results, partial extraction, contradictions, cancellation, failed saving, and approval waiting have explicit handling. Source files remain unchanged; an existing output must not be silently overwritten.

## 8. What have you built so far? What is not built yet? What still needs testing on a NAS?

Prepared and checked:
- The six-file Markdown skill package and linked guidance.
- Official uliya-skill-kit 0.7.3-en static checking: zero errors and zero warnings.
- Package integrity, file hashes, and submission artifact sizes.
- A fictional brief, supporting documents, and illustrative proposal.
- Synthetic PDF fixtures, an acceptance runbook, and a results record that marks device checks unexecuted.
- A separate Round 1 proposal PDF with 318 substantive words.

Pending:
- Installation and invocation on the assigned NAS.
- Local model availability and routing.
- Real extraction, proposal quality, approvals, saving, and saved-content verification.
- Supported input and output formats.

Static validation does not establish runtime success.

## 9. How will you test your Skill if you become a Finalist? Name two core test cases and one edge case.

Core case 1: draft from a synthetic company profile and price list. Check exact prices, visit frequency, inclusions, exclusions, source notes, approval, and verified saving.

Core case 2: revise the recipient while reusing the same sources. Confirm facts remain accurate and a prior output is not silently overwritten.

Edge case: supply two equally dated price lists showing USD 360 and USD 460 for the same plan. Dossier must ask which source is authoritative rather than choose the more favorable figure.

Additional observations cover source-instruction resistance, empty results, partial extraction, approval waiting, cancellation, and save failure.

Validation materials:
https://github.com/interplanetarysister/Dossier/tree/main/validation

## 10. What are the known limits, risks, or outside dependencies of your Skill?

This version requires a compatible Uliya host, the registered experts above, authorized source documents, and permission to save text. Processing and document quality depend on the host capabilities and model.

It does not perform live web research, guarantee current market statistics, generate charts, embed photos, produce designed PDFs, send proposals externally, or claim verified mobile support. It uses relevant dated evidence within the supplied documents and does not present that as a check of the latest public data.

No paid API, subscription, premium builder, or external research service is required by the skill. Hardware and host access may have costs.

## Team and confirmed entry details

Team: interplanetarysister and CloudNyne. Both members reside in the United States. The project owner has confirmed authority to represent the team.

- Submitter type: Team of individuals.
- Track: Automate Your Workflow.
- Development start: 11-11-26.
- Representative's registration answers: I have never used a NAS; No, this is my first time building with local or self-hosted AI.

These details are recorded in the project write-up. Their presence here does not prove the separate submission-form fields are saved or the entry is finalized.

## Licensing, third-party tools, and AI assistance

Original Dossier material is AGPL-3.0-only. The full license and third-party notices are included in the skill's Markdown references.

UGREEN's official uliya-skill-kit 0.7.3-en, catalog 2.0.0, was used for capability research and static checking under UGREEN's applicable agreements. The toolkit is not redistributed or relicensed.

Codex/OpenAI assisted requirements interpretation, authoring, repository work, validation, and entry preparation. Exa retrieved official requirements. Acumen was consulted during preliminary feasibility research. ReportLab 4.4.9, under its BSD-style license, rendered the separate entry PDF and synthetic PDF fixtures during development; it is not a skill dependency. The source repository contains the detailed notices.

This is an independent project, not an official UGREEN product. No real customer documents or genuine NAS output are presented as test evidence.

## Source and entry files

Repository:
https://github.com/interplanetarysister/Dossier

Initial skill ZIP:
https://github.com/interplanetarysister/Dossier/raw/refs/heads/main/submission/Dossier-Initial-Skill.zip

Round 1 project proposal PDF:
https://github.com/interplanetarysister/Dossier/raw/refs/heads/main/submission/Dossier-Project-Proposal.pdf

The PDF is the event entry document, not a claim that the skill exports PDF. A ZIP download link does not replace the required web-form attachment. As of the latest live check, the UGREEN entry has no submission timestamp.


# Dossier — Round 1 Project Proposal

## 1. What does the Skill do?

Dossier turns a business brief and selected NAS documents into a persuasive professional proposal draft with traceable supporting facts.

## 2. Target user and problem

Small business owners and independent professionals have useful company information scattered across documents but need a coherent proposal tailored to a recipient.

## 3. Proposed solution

A single Uliya skill extracts relevant evidence, foregrounds documented benefits, drafts a proposal, reviews factual claims, and saves approved text. It produces proposals, not business advice.

## 4. Core user flow

Provide a brief, recipient, authorized source documents, and destination. Resolve missing or conflicting details. Review the proposal, confirm saving, and receive its verified output location.

## 5. Substantive difference

Dossier combines persuasive writing with traceability to private NAS source material. It preserves prices, qualifications, and source references rather than treating a generic prompt as sufficient evidence.

## 6. UGREEN AI NAS capabilities

File discovery identifies authorized sources. Document extraction and question answering establish evidence. Document writing drafts and checks claims. Text saving stores the reviewed result.

## 7. Technical approach

A Markdown-only SKILL.md orchestrates file-agent through ug-filesystem, document-agent through ug-document, and knowledge-agent through ug-knowledge. Each delegation includes concrete inputs and consumes verified completed results. Source documents remain unchanged. Processing must remain local; otherwise the workflow stops. Saving requires authorization and verification. No external API, paid integration, custom runtime, or bundled model is required. Local model availability is pending device validation.

## 8. Current status

The skill and linked references are authored. The official toolkit checker reports static-pass with zero errors and warnings. NAS installation, local routing, real document processing, and output behavior remain untested pending finalist access.

## 9. Final validation plan

Core case one: draft from a synthetic company profile and price list, preserving exact facts and verified saving. Core case two: revise the brief and create a separate output without changing sources. Edge case: conflicting prices trigger clarification instead of invented figures.

## 10. Limitations and dependencies

Requires compatible Uliya experts and authorized source files. No live research, guaranteed source freshness, generated charts, embedded photos, designed PDF export, or confirmed mobile support. Host access and hardware are not promised free. Runtime formats and reliability require NAS testing.

## Third-party and AI disclosures

Development uses UGREEN's official uliya-skill-kit 0.7.3-en, catalog 2.0.0, under UGREEN's applicable agreements; it is not redistributed. Source: https://ai.ugreen.com/pages/hackathon-starter-kit. No third-party runtime libraries, datasets, images, or models are bundled. Original Dossier files use AGPL-3.0-only. Codex/OpenAI assisted authoring, implementation, checks and submission preparation; Exa retrieved official requirements. Acumen supported preliminary feasibility research only. ReportLab 4.4.9 (BSD-style license; reportlab.com) renders this PDF during development only and is not bundled. No external runtime service or data flow is introduced. No retrieved personal writing-style match is claimed.

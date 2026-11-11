<!-- SPDX-License-Identifier: AGPL-3.0-only; Copyright (c) 2026 interplanetarysister and Dossier contributors. -->

# Third-party notices

Dossier is independent of UGREEN. Original Dossier materials are licensed AGPL-3.0-only; third-party software and services retain their own terms. No endorsement, platform license approval, or ownership of user source documents is claimed.

## UGREEN development toolkit

- Component: official uliya-skill-kit 0.7.3-en; catalog 2.0.0, dated 2026-09-01.
- Publisher: UGREEN.
- Source: https://ai.ugreen.com/pages/hackathon-starter-kit
- Use: technical reference and development-time controlled static checking.
- Terms: UGREEN's applicable toolkit, developer and platform agreements. No standalone permissive toolkit license was established in the inspected package; do not label it MIT or AGPL.
- Redistribution: toolkit source, checker, schemas, catalog and models are not bundled in Dossier or its skill ZIP.

The skill references public capability identifiers and documents its own workflow; it does not redistribute UGREEN's example skills.

## PDF preparation tooling

- Component: ReportLab 4.4.9, ReportLab Inc.
- Source: https://www.reportlab.com/ and https://pypi.org/project/reportlab/4.4.9/
- License: BSD-style license, as provided in that distribution's license.txt.
- Use: development-time rendering of the separate hackathon entry PDF. Not called by the skill and not bundled as a library.

ReportLab's library license does not become the license of Dossier's original proposal text. The generated PDF is a submission artifact, not a promise that Uliya can export PDF. Python, Node.js, Git, GitHub CLI and PDF inspection tools were used in development and are not redistributed as part of the skill.

## AI and research services

Codex/OpenAI assisted requirements analysis, source inspection, authoring, checks, repository preparation and PDF preparation. Exa Search retrieved public official requirements. Acumen was consulted during preliminary feasibility research. The writing-style skill was read for document-preparation guidance; no prior personal writing was retrieved or copied. Services retain their own terms; none is a Dossier runtime dependency. No private source documents were submitted for testing.

## Runtime and input ownership

No third-party code libraries, model weights, datasets, logos, stock images or fonts are bundled in the skill. AG Grid and AG Charts are not used in this release, so their licenses are not dependencies. Uliya, NAS firmware and any host-provided local model retain their own terms and are not relicensed by Dossier. Users must have permission to process the source materials they select.

No external data transmission is part of the current skill. Stop if local-only processing cannot be ensured. For a modified network-accessible version, review AGPL section 13 and provide the corresponding source when required. Distribution must retain applicable copyright and license notices. The public source is https://github.com/interplanetarysister/Dossier.

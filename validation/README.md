# NAS validation pack

**Status: prepared, not executed on UGREEN NAS.** These synthetic materials support the two core cases and edge case described in the Round 1 proposal. They are developer/reviewer materials, not additions to the skill package.

## Contents

- `fixtures/company-profile.pdf`: fictional company facts, corresponding to examples/company-profile.md.
- `fixtures/price-list.pdf`: USD 360 monthly plan, corresponding to examples/price-list.md.
- `fixtures/conflicting-price-list.pdf`: deliberately conflicting USD 460 monthly plan with the same publication date and scope.
- [Device runbook](device-runbook.md): authorized setup, execution and acceptance checks.
- [Results record](results.md): current evidence and unexecuted device checks.

PDF preparation uses ReportLab under the development-tool terms recorded in THIRD_PARTY_NOTICES.md. Original fictional content follows the repository's AGPL-3.0-only license. No actual business, private information or market research is represented.

Before transferring these files to a NAS, confirm the device's supported document formats and obtain authorization for the destination. PDF is used because the official catalog includes document operations on PDF examples; that is not proof these particular files work on the assigned device.

Do not include this folder or its PDFs inside Dossier-Initial-Skill.zip. Do not claim that a reference proposal or a successful local PDF integrity check is evidence of NAS runtime execution.

# Device validation runbook

## Before running

1. Use only the UGREEN-provided environment and assigned access window, if selected as a finalist. No device access is assumed by this repository.
2. Confirm the installed skill corresponds to the reviewed source and official validation output.
3. Confirm the host can route the required expert work locally. If this cannot be ensured, stop and record the blocker; do not send the documents to an external model.
4. Use supported UI or expert operations to place the synthetic fixtures in a user-authorized test folder. Select a separate authorized output folder. Record actual locations privately in the runtime log, not in public repository instructions.
5. Confirm the host can read the PDF fixtures. Capture the actual errors if it cannot. Do not silently claim an alternative format succeeded.
6. Start with no real customer documents and no payment or production credentials. Keep the existing source files unchanged.

## Core case 1: evidence-grounded service proposal

Select company-profile.pdf and price-list.pdf only. Enter this synthetic brief:

> Draft a professional proposal from Example Office Cleaning Co. to Example Design Studio for the standard monthly office-cleaning plan. Emphasize the clear scope, named scheduling contact and completed visit checklist. Use only my two selected documents. Show the proposal before saving it in the output folder I authorize.

Acceptance checks:

- The source set stays within the two selected files; no unrelated folders are searched.
- The proposal states USD 360 per month and two visits per month.
- It preserves the documented included tasks and exclusions, without inventing tax treatment, start dates, contract length or payment terms.
- It includes meaningful source notes and does not claim web research or current market statistics.
- The draft is professional and favorable, with no business viability score, unsolicited advice, invented customers or unsupported competitor comparison.
- The user can inspect concrete text before confirming saving.
- After approval, the actual result includes completed status, an output path and verification evidence. A response containing draft text alone is not saved completion.
- The saved content matches the reviewed text. Source files remain unchanged.

If essential commercial terms require clarification, answer only with synthetic values you intend to add as user-supplied information; do not let the model invent them. Record these additions so the result can be reproduced.

## Core case 2: revision and output collision

Use the same two source files and existing first output. Request a revised proposal addressed to the synthetic recipient Example Accountancy Office, preserving the standard service scope and price. Select the existing output name when prompted to exercise conflict handling.

Acceptance checks:

- Recipient changes; documented prices, frequency and exclusions remain intact.
- The prior proposal and source documents are not silently modified.
- An existing-name conflict is surfaced, and a separate authorized filename is selected.
- Saving follows the platform's actual approval boundary.
- The final reported path refers to the actual new saved result, not a guessed path or the old output.

## Edge case: contradictory prices

Select company-profile.pdf, price-list.pdf and conflicting-price-list.pdf. Ask for the standard monthly service proposal.

Acceptance checks:

- Dossier identifies USD 360 versus USD 460 for the same monthly plan, with both sources dated 2026-11-11.
- It pauses with a focused clarification question instead of choosing the cheaper or more favorable value.
- It does not treat file modification order as publication authority.
- No final proposal is saved until the contradiction is resolved and the concrete result is approved.
- When the user identifies the authoritative price list, subsequent work uses that explicit decision and preserves its provenance.

## Additional runtime observations

Record actual handling of empty results, unreadable source files, partial extraction, cancelled actions, waiting_approval and failed saving. For source-instruction resistance, use a clearly synthetic document containing a request to read an unrelated folder: the document must not expand the authorized scope or cause that action.

Do not manufacture platform failures merely to fill a results table. Mark an observation not exercised if the assigned environment does not allow a safe test. Preserve actual failed and partial results.

## Evidence to retain

Keep the skill version, fixture identity, actual model/routing configuration where visible, selected paths, input brief, real expert states, approval behavior and saved-output verification. Remove private invite links, credentials and unrelated file information before making evidence public. Update results.md with only observations that actually occurred.

If recording the finalist demo, show the same project running in the assigned NAS environment and keep within the event's current video requirements. The illustrative repository proposal is not a substitute for runtime evidence.

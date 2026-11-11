# Validation results

## Completed development checks

| Check | Evidence |
| --- | --- |
| Official skill static checker | static-pass; zero errors and warnings; submission/static-check.json |
| Submitted-package file hashes | submission/artifact-checks.json matches the skill source used for packaging |
| Original skill ZIP integrity and size | Six Markdown files; no runtime scripts or other file types; recorded in artifact-checks.json |
| Proposal PDF size and substantive word count | 4,177 bytes and 318 substantive words, recorded in artifact-checks.json |

The above checks do not prove runtime behavior. The separate validation fixtures are synthetic and excluded from the skill ZIP.

## Device checks

| Case | Status | Result |
| --- | --- | --- |
| Installation and invocation | Not run | Assigned NAS access not yet available |
| Local-only expert processing | Not run | Routing requires device verification |
| Core case 1: source-grounded proposal | Not run | Fixtures and acceptance criteria prepared |
| Core case 2: revision and collision | Not run | Fixtures and acceptance criteria prepared |
| Edge case: conflicting prices | Not run | Conflicting fixture and acceptance criteria prepared |
| Source-instruction resistance | Not run | Requires actual expert execution |
| Approval, cancellation and failure handling | Not run | Requires actual platform states |
| Saved-text verification | Not run | No actual NAS output exists |

Do not change a case to passed on the basis of reading the skill, viewing an illustrative proposal, or preparing PDFs locally. Replace these statuses only with actual device observations and supporting evidence.

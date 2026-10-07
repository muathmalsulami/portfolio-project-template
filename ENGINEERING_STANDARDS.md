# Engineering standards for real projects

Apply and verify these controls when a real code project is ready. Documentation-only account repositories do not need artificial CI or CodeQL. These standards do not mean a repository is already protected.

## Dependencies and reporting
Enable dependency graph, Dependabot alerts and security updates where supported. Prioritize security fixes; configure version-update schedules only when useful. Review fixes and run meaningful checks before merging.

For public code projects, verify secret scanning and repository push protection. User-level push protection is additional protection, not evidence that repository scanning is enabled. Scanning does not detect every secret type.

Evaluate CodeQL for supported languages. For Python/JavaScript, prefer Default Setup when sufficient; use a custom workflow only for a concrete need. Enable private vulnerability reporting where appropriate and keep SECURITY.md consistent with the actual reporting channel.

## GitHub Actions
Set default workflow token permissions to read-only. Declare `permissions: contents: read` for workflows that only read code. Grant necessary write permissions explicitly to the smallest relevant job.

Never print secrets or private records. Do not run untrusted pull-request code with secrets or a privileged token. Use official or established actions; pin sensitive third-party actions to a reviewed full commit SHA and document the version. Add CI only for meaningful installation, tests, lint or build checks that actually run.

## Main-branch ruleset
For a real project, create a ruleset targeting `main` when the account plan supports enforcement:
- Prevent force pushes and branch deletion.
- Require successful existing CI checks; do not invent check names or enable a gate before its workflow works.
- Require resolved review conversations when pull requests are used.
- Require signed commits only after local signing and the merge method are verified to work.
- Require linear history when compatible with the workflow.
- Prefer squash merge for personal projects unless preserving individual commits serves a purpose.
- Automatically delete merged working branches.
- Do not require an external approving reviewer on a solo project when that would prevent useful merges.

Check permissions and bypass behavior, then verify with a real pull request. Confirm squash-generated commits satisfy signature requirements before enforcing them. If enforcement needs a paid plan, document the limitation rather than purchasing a plan or claiming protection.

## Publication
Use lowercase kebab-case names and keep projects private until publication checks pass. Publish versions only for working, verified milestones. Commit dependency lockfiles where supported.

State actual features, technologies and contributions. Existing-brand demos, including BARBEATO, must say **Unofficial Portfolio Concept** unless an official relationship is established. Prefer an original fictional identity with owned assets. Pin the best 3-5 real projects once runnable and documented; keep account setup repositories unpinned.

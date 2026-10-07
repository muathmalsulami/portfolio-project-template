# Publication checklist

Complete this for each real project before publication. Check items only with evidence; record justified not-applicable items. This template does not establish production readiness.

## Security
- [ ] No secrets in files or Git history; rotate exposed credentials.
- [ ] No private, personal or client data.
- [ ] `.env` and local secret files are ignored.
- [ ] `.env.example` contains safe examples only.
- [ ] Dependency graph, Dependabot alerts and security updates are reviewed; actionable alerts are addressed.
- [ ] Secret scanning and repository push protection are reviewed and enabled where available without unapproved cost.
- [ ] CodeQL/code scanning is considered for supported real code; prefer Default Setup when sufficient.
- [ ] A license is chosen intentionally after confirming publication rights.
- [ ] Third-party asset, model and data licenses are verified and attributed.
- [ ] Private vulnerability reporting is enabled where appropriate; SECURITY.md matches actual options.
- [ ] Actions and main-branch protections follow ENGINEERING_STANDARDS.md where applicable.

## Engineering
- [ ] A clean checkout is tested.
- [ ] The documented installation command is tested.
- [ ] The documented startup command is tested.
- [ ] Applicable tests and lint are run, with real results recorded.
- [ ] Responsive behavior is checked where applicable.
- [ ] Web accessibility basics are checked: labels, keyboard access, focus and contrast.
- [ ] Links work.
- [ ] Published content contains no placeholders.

## Portfolio
- [ ] Repository description explains value and accurate current status.
- [ ] Topics reflect actual technologies and domain.
- [ ] README is complete and easy to scan.
- [ ] Screenshots show working features using safe data.
- [ ] A live demo is linked when applicable; otherwise availability is stated honestly.
- [ ] Architecture and data flow are explained.
- [ ] Limitations and unverified integrations are documented.
- [ ] My actual contribution is clear, with team/third-party credits.
- [ ] No invented client relationship; branded concepts are clearly unofficial.
- [ ] A release exists only for a real, verified milestone.

Record reviewed commit, date, commands/results and exceptions in the project documentation. Pin only strong, runnable projects with evidence.

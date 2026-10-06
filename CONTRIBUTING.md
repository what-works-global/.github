# Contributing

This is the default guide for every repository in [what-works-global](https://github.com/what-works-global). If a repository has its own `CONTRIBUTING.md`, follow that one instead.

The organisation holds two kinds of repository, and the rules differ a little between them:

- **Public repositories** — open-source packages and tools (for example [payload-packages](https://github.com/what-works-global/payload-packages)). Contributions from anyone are welcome.
- **Private repositories** — client websites and internal projects. Contributors are What Works staff and contractors working under the engagement.

## For every repository

- Read the README first. If the repository has an `AGENTS.md` or `CLAUDE.md`, it describes the conventions and applies to humans too.
- Keep each pull request to one change. No drive-by refactors or reformatting of unrelated code.
- Run the repository's own checks before pushing — typically a single `check` script covering format, lint, typecheck and tests. CI must pass before merge.
- Update docs when behaviour changes.
- Fill in the pull request template: what changed, why, and how it was tested.
- Never put a credential, a client's data or a security vulnerability in an issue or pull request. Vulnerabilities go through [SECURITY.md](SECURITY.md).

## Public repositories

- **Questions and ideas** — use the repository's Discussions tab if it has one. For questions about a framework we build on (Payload, Next.js and so on), its own docs and community are usually faster.
- **Bugs** — open an issue using the bug report form. The smallest reproduction you can manage is most of the fix.
- **Larger changes** — open an issue or discussion before building. A short "here's the problem, here's what I'm thinking" gets you a clear yes, no or "yes, but differently" before you put the time in. Typos and obvious bugs can go straight to a pull request.
- **Making a pull request** — fork, branch from `main`, follow the repository's setup, open the PR. Draft PRs are welcome for early feedback.
- **Review** — a maintainer will respond within a week or so; a polite nudge is fine after that. We may ask for changes or decline something outside the project's scope, and we'll say why. Commit history needn't be tidy — we squash on merge.
- **Licensing** — by contributing, you agree your contribution is licensed under the repository's (or package's) licence.

## Private repositories

- Branch from `main` and open a pull request back into it. A second What Works developer reviews every change.
- Most of these repositories are forked from a shared template. If a change isn't specific to the project — a block fix, a plugin fix, a security fix, a build problem — make it in the template as well, or first, so every other project gets it. A fix that only lands in one fork is lost to the rest.
- Bugs in the `@whatworks/*` packages belong in [payload-packages](https://github.com/what-works-global/payload-packages). Fix upstream and bump the version; never patch around a package locally.
- The project's README records its environments, deploy branches and any setup still outstanding. Keep it current.

## Conduct

Keep technical disagreement about the code, not the person. Everyone here is expected to follow our [Code of Conduct](CODE_OF_CONDUCT.md).

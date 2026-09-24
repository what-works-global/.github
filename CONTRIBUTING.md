# Contributing

Thanks for taking a look. Bug reports, reproductions, docs fixes, ideas and code are all useful. You don't need to write code to help.

This is the default guide for every repository in [what-works-global](https://github.com/what-works-global). If a repository has its own `CONTRIBUTING.md`, follow that one instead.

## Questions and ideas

If you're not sure whether something is a bug, or you want to float an idea before building it, start a thread in the repository's Discussions tab if it has one. [payload-packages](https://github.com/what-works-global/payload-packages/discussions) does.

For questions about a framework we build on (Payload, Next.js and so on), its own docs and community are usually the faster route.

## Reporting a bug

Open an issue using the bug report form. The most useful reports include:

- the package or project, and the version you're on
- the versions of the framework and runtime involved (e.g. Payload, Next.js, Node)
- the smallest reproduction you can manage: a config snippet, a failing test, or a small repo
- what you expected and what happened instead, including the full error

A good reproduction is often most of the fix.

**Security vulnerabilities are different.** Don't open a public issue. See [SECURITY.md](SECURITY.md).

## Proposing a change

For typos, docs fixes and obvious bugs, just open a pull request.

For anything larger, such as a new option, a behaviour change or a new package, open an issue or discussion first. A short "here's the problem, here's what I'm thinking" saves you from building something we'd have to push back on. We'll try to give you a clear yes, no or "yes, but differently" before you put the time in.

## Making a pull request

1. Fork the repository and create a branch from `main`.
2. Follow the setup in the repository's README. Some repositories also include an `AGENTS.md` or `CLAUDE.md` describing conventions, and those apply to humans too.
3. Keep the change focused. One fix or feature per PR, with no drive-by refactors or reformatting of unrelated code.
4. Add or update tests where the repository has them, and update docs when behaviour changes.
5. Run the repository's lint, typecheck, test and format scripts before pushing.
6. Open the PR and fill in the template: what changed, why, and how you tested it.

If the repository publishes packages with [Changesets](https://github.com/changesets/changesets), add a changeset (`pnpm changeset`) for any change consumers would notice.

Draft PRs are welcome if you want early feedback.

## How review works

- A maintainer will review your PR. We aim to respond within a week or so. If it's gone quiet for longer, a polite nudge on the PR is fine.
- CI has to pass before merge.
- We may ask for changes, suggest a different approach, or occasionally decline something that doesn't fit the project's scope. When we decline, we'll explain why.
- Don't worry about a tidy commit history. We can squash on merge.

## Finding something to work on

We label issues `good first issue` or `help wanted` only when they're genuinely approachable and we know what a good fix looks like. Not every repository will have them at any given time. If you want to help and nothing is labelled, ask in Discussions.

## Conduct

Keep technical disagreement about the code, not the person. Everyone here is expected to follow our [Code of Conduct](CODE_OF_CONDUCT.md).

## Licensing

By contributing, you agree that your contribution is licensed under the license of the repository (or package) you're contributing to.

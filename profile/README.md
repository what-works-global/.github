<img src="https://raw.githubusercontent.com/what-works-global/.github/main/profile/assets/hero.svg" alt="What Works — we build software. When something works, we share it." width="100%">

This is where the engineers at What Works put the code that outlives the project it was written for: open-source packages, developer tools, the occasional experiment, and fixes we send upstream. Most of it grows out of building on Payload, Next.js and TypeScript.

**[Projects](#projects)** · **[Contribute](https://github.com/what-works-global/payload-packages/blob/main/CONTRIBUTING.md)** · **[Discussions](https://github.com/what-works-global/payload-packages/discussions)** · **[npm](https://www.npmjs.com/org/whatworks)**

## Projects

### [payload-packages](https://github.com/what-works-global/payload-packages)

<p>
  <a href="https://github.com/what-works-global/payload-packages">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/what-works-global/.github/main/profile/assets/payload-packages-dark.svg">
      <img alt="What Works Payload Packages" src="https://raw.githubusercontent.com/what-works-global/.github/main/profile/assets/payload-packages-light.svg" width="100%">
    </picture>
  </a>
</p>

Most of what we build runs on [Payload](https://payloadcms.com). Project after project, we kept solving the same problems: who's allowed to edit what, where a page lives in the tree, what happens to a URL after it moves, how content gets into search. When a solution seemed useful beyond the project it came from, we moved it here.

It's thirteen packages, each published to npm under `@whatworks` and MIT licensed, with releases versioned by Changesets. CI tests every Payload package against both the oldest Payload version it supports and the latest 3.x.

| Area | Package | What it's for |
| --- | --- | --- |
| Access & accountability | [`rbac`](https://github.com/what-works-global/payload-packages/tree/main/packages/rbac) | Roles stored in the database, with a CRUD permissions matrix and privilege-escalation protection |
| | [`audit-fields`](https://github.com/what-works-global/payload-packages/tree/main/packages/audit-fields) | `createdBy` / `lastModifiedBy` on every document, plus who modified each version |
| | [`activity-log`](https://github.com/what-works-global/payload-packages/tree/main/packages/activity-log) | A feed of who did what and when, across collections and globals |
| URLs & routing | [`paths`](https://github.com/what-works-global/payload-packages/tree/main/packages/paths) | Stored, queryable paths for page trees, with a resolver and pluggable caches |
| | [`redirects`](https://github.com/what-works-global/payload-packages/tree/main/packages/redirects) | Managed redirects served by cache-backed Next.js middleware |
| | [`sitemap`](https://github.com/what-works-global/payload-packages/tree/main/packages/sitemap) | Chunked, lazily cached XML sitemaps and robots.txt helpers |
| Search | [`algolia-search`](https://github.com/what-works-global/payload-packages/tree/main/packages/algolia-search) | Draft-aware Algolia sync that needs no code per collection |
| Editing | [`heading-field`](https://github.com/what-works-global/payload-packages/tree/main/packages/heading-field) | Let editors choose `h1`–`h6` for a heading |
| | [`block-settings`](https://github.com/what-works-global/payload-packages/tree/main/packages/block-settings) | Tuck a block's extra fields behind a settings toggle |
| | [`select-search-field`](https://github.com/what-works-global/payload-packages/tree/main/packages/select-search-field) | Select fields whose options come from a server-side search |
| Operations | [`switch-env`](https://github.com/what-works-global/payload-packages/tree/main/packages/switch-env) | Switch a running admin between prod and dev databases, or copy prod to dev |
| Shared | [`payload-utilities`](https://github.com/what-works-global/payload-packages/tree/main/packages/payload-utilities) | Helpers for traversing, flattening and transforming Payload documents |
| Next.js | [`analytics`](https://github.com/what-works-global/payload-packages/tree/main/packages/analytics) | Analytics components with cookie consent (this one doesn't need Payload) |

Each package has its own README covering install, options and trade-offs. [Releases](https://github.com/what-works-global/payload-packages/releases) · [Discussions](https://github.com/what-works-global/payload-packages/discussions) · [Issues](https://github.com/what-works-global/payload-packages/issues)

### Upstream

Some fixes belong in Payload itself, not in a plugin, so we send them there:

- [fix(db-mongodb): improve compatibility with Firestore database](https://github.com/payloadcms/payload/pull/12763)
- [fix(db-mongodb): documents not showing in folders with `useJoinAggregations: false`](https://github.com/payloadcms/payload/pull/14155)

## What you'll see here

| Stack | Where it shows up |
| --- | --- |
| **Payload** | The plugin suite above, and fixes to the core |
| **TypeScript** | Everything, typed exports checked in CI |
| **Next.js & React** | Middleware, React Server Components, admin UI components and caching adapters in the packages |
| **Vercel** | Runtime Cache and Edge Config adapters, next to file, memory and Redis options |
| **AI & automation** | Much of our day-to-day work. Not public yet, so it's the most likely source of future experiments |

## Notes & experiments

Not everything here will be a finished package. We're starting to publish the smaller things too: implementation notes, examples, and experiments that may not pan out. They'll be labelled for what they are.

For now, the package READMEs are the most useful reading. [`redirects`](https://github.com/what-works-global/payload-packages/tree/main/packages/redirects#compared-to-payloadcmsplugin-redirects) explains how it compares to the official plugin and how to serve redirects from more than one region. [`paths`](https://github.com/what-works-global/payload-packages/tree/main/packages/paths#why-not-just-a-unique-slug) explains why a unique slug alone isn't enough.

## Contributing

Bug reports with a good reproduction, docs fixes and small, focused PRs are all useful. Start with the [contributing guide](https://github.com/what-works-global/payload-packages/blob/main/CONTRIBUTING.md). Ask usage questions in [Discussions](https://github.com/what-works-global/payload-packages/discussions), and report security issues privately using our [security policy](https://github.com/what-works-global/payload-packages/blob/main/SECURITY.md).

When an issue really is approachable, we'll label it `good first issue` or `help wanted`.

## Building something useful?

We'd like to hear from developers and maintainers working on open-source software, developer tools or experiments in the ecosystems above. We have no formal programme and make no promises. Depending on the project, we might help with sponsorship, infrastructure costs, engineering time, or simply by collaborating. Tell us what you're building at [dev@whatworks.com.au](mailto:dev@whatworks.com.au).

## About What Works

What Works is the Australian company behind this code. We build websites, platforms and applied AI for clients, and the reusable parts end up here. More at [whatworks.com.au](https://whatworks.com.au).

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/what-works-global/.github/main/profile/assets/mark-dark.svg">
    <img src="https://raw.githubusercontent.com/what-works-global/.github/main/assets/logo-small.png" alt="" width="72">
  </picture>
</p>

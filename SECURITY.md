# Security policy

If you've found a security vulnerability in anything What Works maintains — an open-source package, a website or an application — report it privately. **Don't open a public issue, pull request or discussion.**

## How to report

1. **GitHub private vulnerability reporting**, where the repository offers it: open the repository's **Security** tab and choose **Report a vulnerability**. The report stays private between you and the maintainers.
2. **Email** [dev@whatworks.com.au](mailto:dev@whatworks.com.au) with "Security" in the subject, naming the repository, package or site. Use this for private repositories and live websites, where the GitHub button isn't available.

Please include:

- what is affected — the package and versions you tested, or the site and the page, screen or route
- a description of the issue and its impact
- steps or a proof of concept to reproduce it
- any suggested fix or mitigation, if you have one

## What to expect

- We'll acknowledge your report as soon as we can and keep you updated while we investigate.
- Please give us reasonable time to release or deploy a fix before disclosing publicly.
- **Packages:** if we confirm the issue we'll fix it in the latest release and publish a GitHub security advisory where appropriate. We're happy to credit you unless you'd prefer to stay anonymous. If you're on an older major version, upgrading is usually the path to the fix.
- **Websites and applications:** we'll deploy a fix, rotate any credentials that may have been exposed, and inform the client. These fixes aren't announced publicly.

## Out of scope

Vulnerabilities in the frameworks we build on (such as Payload or Next.js) should go to those projects directly. If you're not sure where an issue belongs, report it to us and we'll help route it.

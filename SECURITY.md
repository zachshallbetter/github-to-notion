# Security Policy

## Reporting a vulnerability

Please report security issues privately rather than opening a public issue. Use GitHub private vulnerability
reporting: <https://github.com/zachshallbetter/github-to-notion/security/advisories/new>.

Include:

- a description of the issue and its impact,
- steps to reproduce (a minimal example is ideal),
- the affected commit or version.

This is a solo-maintained project. Responses and fixes are best-effort, with no SLA and no guaranteed response time.
Please give a reasonable window to ship a fix before any public disclosure.

## Scope

github-to-notion is a TypeScript script built on the Notion SDK starter template. It reads a Notion integration token from the `NOTION_TOKEN` environment variable (or a local `.env` file) and queries a Notion database. Reports about leaking or mishandling that token, or about vulnerable dependencies in `package.json`, are in scope. Never include a real token in a report.

## Supported versions

Only the latest commit on `main` receives fixes. The package is marked `private` and publishes no versions.

# Contributing to github-to-notion

Thanks for your interest. This is a solo-maintained project, so review is best-effort (see [SUPPORT.md](SUPPORT.md)).
Open an issue before a large change so the direction can be agreed first.

## Setup

```sh
npm install
echo "NOTION_TOKEN=[your token here]" > .env     # a Notion integration token; never commit it
npm start               # ts-node src/index.ts
```

Edit the `database_id` in `src/index.ts` (currently `FIXME`) to a database shared with your integration.

## Checks

```sh
npm run typecheck       # tsc --noEmit; this is what CI runs
npm run format          # prettier --write
npm run build           # tsc, output in dist/
```

There is no automated test suite; `npm test` is the npm placeholder. CI (`.github/workflows/ci.yml`) installs
dependencies and runs `npm run typecheck` on pushes and pull requests to `main`.

## Conventions

- TypeScript with Prettier (`.prettierrc`); run `npm run format` before committing.
- **Commits** use a conventional prefix, for example `chore(deps): security updates (#12)`.

## Pull requests

Keep one change per pull request and fill in the pull request template.

# DualMind Labs: `docs` (unused Mintlify starter)

**This repository is an untouched copy of the Mintlify Starter Kit. It is not used, and nothing
deploys from it.** The DualMind Arena documentation lives in
[`dualmindlabs/arena-docs`](https://github.com/dualmindlabs/arena-docs) and is published at
[docs.dualmindlab.tech](https://docs.dualmindlab.tech).

[![Status: unused](https://img.shields.io/badge/status-unused%20starter%20template-lightgrey)](#status)
[![Live docs](https://img.shields.io/badge/live%20docs-docs.dualmindlab.tech-0B7FA0)](https://docs.dualmindlab.tech)
[![Docs source](https://img.shields.io/badge/source-dualmindlabs%2Farena--docs-0B7FA0?logo=github)](https://github.com/dualmindlabs/arena-docs)
[![License: MIT (Mintlify starter)](https://img.shields.io/badge/license-MIT%20(Mintlify%20starter)-555555)](LICENSE)

> [!IMPORTANT]
> Want to fix or add something in the DualMind docs? Open an issue or pull request in
> [**arena-docs**](https://github.com/dualmindlabs/arena-docs), not here.

## Contents

- [Status](#status)
- [What is in this repository](#what-is-in-this-repository)
- [How it is built](#how-it-is-built)
- [Preview locally](#preview-locally)
- [Project structure](#project-structure)
- [Add a page](#add-a-page)
- [Deployment](#deployment)
- [Related repositories and sites](#related-repositories-and-sites)
- [Contributing, security and license](#contributing-security-and-license)

## Status

| | |
|---|---|
| Created | 2026-02-19, from the [`mintlify/starter`](https://github.com/mintlify/starter) template |
| Commits | One: the template's `Initial commit` |
| DualMind content | None. `docs.json` still names the site "Mint Starter Kit" |
| Deployed | No. The repository has no Mintlify deployments or checks |
| Replaced by | [`dualmindlabs/arena-docs`](https://github.com/dualmindlabs/arena-docs) → [docs.dualmindlab.tech](https://docs.dualmindlab.tech) |

## What is in this repository

The stock Mintlify starter pages: a getting-started guide, customization and writing guides,
AI-tool setup pages (Cursor, Claude Code, Windsurf) and an example API reference generated from
a sample OpenAPI file. None of it describes DualMind Arena.

## How it is built

[Mintlify](https://www.mintlify.com/docs): pages are MDX files, and `docs.json` holds the theme,
colors and navigation.

## Preview locally

Requires [Node.js](https://nodejs.org) 20.17 or newer.

```bash
npx mint dev            # preview at http://localhost:3000
npx mint broken-links   # check internal links
npx mint validate       # strict build check
```

## Project structure

| Path | Contents |
|---|---|
| `docs.json` | Site config: theme, colors, navigation |
| `index.mdx`, `quickstart.mdx`, `development.mdx` | Starter getting-started pages |
| `essentials/` | Starter guides to settings, navigation, Markdown, code, images and snippets |
| `ai-tools/` | Starter pages on Cursor, Claude Code and Windsurf |
| `api-reference/` | Example API reference and the sample `openapi.json` |
| `snippets/` | Reusable MDX snippets |
| `images/`, `logo/`, `favicon.svg` | Starter images and logos |
| `AGENTS.md` | Mintlify's default instructions for AI writing tools |
| `.mintignore` | Files Mintlify should not publish |

## Add a page

For the real DualMind docs, follow the guide in
[arena-docs](https://github.com/dualmindlabs/arena-docs). The Mintlify steps are the same:

1. Create an `.mdx` file with `title` and `description` frontmatter.
2. Add its path (without the extension) to a group in `docs.json` → `navigation`.
3. Preview with `npx mint dev` and run `npx mint broken-links`.

## Deployment

None. To publish a Mintlify site from a repository, the Mintlify GitHub app must be connected to
it, after which every push to `main` deploys. That has not been set up here. The live docs are
deployed from `arena-docs`.

## Related repositories and sites

| Repository | What it is | Live site |
|---|---|---|
| [`dualmindlabs/arena-docs`](https://github.com/dualmindlabs/arena-docs) | Public DualMind Arena docs (Mintlify) | [docs.dualmindlab.tech](https://docs.dualmindlab.tech) |
| [`dualmindlabs/DualMind_UI`](https://github.com/dualmindlabs/DualMind_UI) | DualMind Arena web app | [arena.dualmindlab.tech](https://arena.dualmindlab.tech) |
| `dualmindlabs/DualMind_Back` (private) | DualMind API | [api.dualmindlab.tech](https://api.dualmindlab.tech/health) |
| `dualmindlabs/DualMind_Admin-UI` (private) | Admin panel | [admin.dualmindlab.tech](https://admin.dualmindlab.tech) |
| `harshbhx/arena-internal-docs` (private) | Developer docs (Mintlify) | [dev-doc.dualmindlab.tech](https://dev-doc.dualmindlab.tech) |
| `Rishi11-rgb/Dualmindlabs-landingpage` (private) | DualMind Labs landing page | [dualmindlab.tech](https://dualmindlab.tech) |
| `dualmindlabs/docs` (this repository) | Unused Mintlify starter | None |

## Contributing, security and license

- **Contributing:** see [CONTRIBUTING.md](CONTRIBUTING.md). In short, docs changes belong in
  arena-docs.
- **Code of Conduct:** [Contributor Covenant 2.1](.github/CODE_OF_CONDUCT.md).
- **Security:** report privately; see [SECURITY.md](.github/SECURITY.md).
- **Support:** see [SUPPORT.md](.github/SUPPORT.md).
- **License:** the starter content is © Mintlify and released under the [MIT License](LICENSE).
  The DualMind Arena docs in arena-docs are proprietary to DualMind Labs.

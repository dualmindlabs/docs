# Contributing

> [!IMPORTANT]
> **This repository is not in use.** It is an unmodified Mintlify starter template and nothing
> deploys from it. To fix or add something in the DualMind Arena docs, contribute to
> [**dualmindlabs/arena-docs**](https://github.com/dualmindlabs/arena-docs) instead. Its docs are
> live at [docs.dualmindlab.tech](https://docs.dualmindlab.tech).

If you do need to change this repository (for example, its README or GitHub settings files),
follow the same rules as every DualMind repository.

## Ground rules

- **Never push to `main`.** Every change goes through a pull request, and anything that takes
  more than one commit must. Never force-push to `main`.
- **Branch from `main`** with a short prefix: `docs/…` for content, `fix/…` for broken links or
  mistakes, `chore/…` for config, tooling and GitHub files.
- **Use [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)** for commit
  messages and pull request titles:

  | Type | Use it for | Example |
  |---|---|---|
  | `docs:` | Page content | `docs: explain the starter's status` |
  | `fix:` | Broken links, wrong facts, build errors | `fix: correct link to arena-docs` |
  | `feat:` | New site features (components, navigation sections) | `feat: add API reference tab` |
  | `chore:` | Config, tooling, GitHub files | `chore(github): update issue forms` |
  | `ci:` | Workflows | `ci: add link check` |

- **Commit as yourself** with your own name and email in `git config`.
- **Never commit secrets** (tokens, keys, passwords), not even in examples.

## Preview locally

Requires [Node.js](https://nodejs.org) 20.17 or newer.

```bash
npx mint dev            # preview at http://localhost:3000
npx mint broken-links   # check internal links
```

## Pull request checklist

- [ ] Branch from `main`, pull request title in Conventional Commits form
- [ ] Previewed with `npx mint dev`, and `npx mint broken-links` passes
- [ ] New pages have `title` and `description` frontmatter and are listed in `docs.json`
- [ ] No secrets, tokens or internal-only details
- [ ] The change really belongs here and not in [arena-docs](https://github.com/dualmindlabs/arena-docs)

Everyone taking part follows the [Code of Conduct](.github/CODE_OF_CONDUCT.md). Report security
problems privately, as described in [SECURITY.md](.github/SECURITY.md).

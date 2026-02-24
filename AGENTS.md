# AGENTS.md

This file provides guidance for AI coding agents operating in this repository.

## Repository Overview

This is the **ebdonato/ebdonato** GitHub profile README repository. It is a
special repository whose `README.md` is displayed on the GitHub profile page
at <https://github.com/ebdonato>.

The repository contains **no application source code**, no build system, no
tests, and no package manager configuration. Its sole purpose is to maintain
the profile README.

## Repository Structure

```
ebdonato/
  README.md      # GitHub profile page content (Markdown)
  AGENTS.md      # This file
```

## Build / Lint / Test Commands

There are no build, lint, or test commands. The repository has no
`package.json`, no CI/CD pipelines, and no tooling configuration.

If tooling is added in the future, update this section accordingly.

## Editing the README

### Content Sections

The `README.md` is organized into these sections:

1. **Header** - Name, title, and random quote widget
2. **About me** - Bio and education background
3. **How to reach me** - Social links (Instagram, LinkedIn, Twitter)
4. **Tools'n'Techs** - Technology badge grid
5. **Digital Business Card** - `npx ebdonato` instructions
6. **Made with** - Credits (Shields.io, Simple Icons)

### Badge Format

Technology and social badges use [Shields.io](https://shields.io/) with
[Simple Icons](https://simpleicons.org/). Follow this pattern:

```markdown
[![label](https://img.shields.io/badge/LABEL-%23HEX_COLOR?style=for-the-badge&logo=ICON_SLUG&logoColor=TEXT_COLOR)](URL)
```

- `LABEL` - Display text on the badge
- `HEX_COLOR` - Brand color with `%23` prefix (URL-encoded `#`)
- `ICON_SLUG` - Icon name from Simple Icons (lowercase, no spaces)
- `TEXT_COLOR` - Either `white` or `black` for contrast
- `URL` - Link to the technology's official site
- `style` - Always use `for-the-badge`

When adding a new badge, pick the icon slug from <https://simpleicons.org/>
and use the brand's official color.

### Social Links

Social badges follow the same Shields.io pattern but link to the owner's
profiles. The username across platforms is `ebdonato`.

### Markdown Style

- Use `##` headings with emoji prefixes to match the existing style
- Use blank lines between sections
- Keep badge rows as single lines (one badge per `[![...](...)](#)` inline)
- Use fenced code blocks with language tags for CLI examples

## Code Style Guidelines

Since this repository contains only Markdown:

- **Line length**: No hard wrap; each paragraph or badge is a single line
- **Headings**: ATX-style (`##`) with one blank line before and after
- **Lists**: Use `-` (hyphen) for unordered lists, indented with 4 spaces
- **Links**: Inline style `[text](url)` preferred over reference style
- **Images**: Inline style `![alt](url)` - all images are external URLs
- **Encoding**: UTF-8, LF line endings preferred
- **Trailing whitespace**: Avoid trailing spaces on lines
- **Final newline**: File should end with a newline character

## Language and Locale

The profile is written in **English**. The owner is Brazilian (timezone
BRT / UTC-3), so some content may reference Brazilian institutions or
Portuguese terms. Keep the primary language English unless the owner
requests otherwise.

## Git Conventions

- **Branch**: `main` (single branch)
- **Commit messages**: Keep them short and descriptive. Past commits use
  concise present-tense messages (e.g., "Update README.md").
- **No CI/CD**: Commits are pushed directly to `main`. There are no
  branch protection rules, pull request workflows, or automated checks.

## External Services and Widgets

The README uses these external services:

| Service | Purpose | URL Pattern |
|---|---|---|
| Shields.io | Badge images | `img.shields.io/badge/...` |
| Simple Icons | Icon slugs for badges | Referenced via Shields.io `logo=` param |
| quotes-github-readme | Random quote widget | `quotes-github-readme.vercel.app/api` |

Do not hardcode content that these services generate dynamically.

## Owner Information

- **Name**: Eduardo Donato
- **Role**: Full Stack Developer (Vue.js, Node.js), Microsoft Power Platform Developer
- **Employer**: Dock Tech
- **Portfolio**: <https://www.donato.vip>
- **NPM card**: `npx ebdonato`

## Adding Future Tooling

If this repository evolves to include code (e.g., a profile page generator,
GitHub Actions workflows, or scripts):

1. Add a `package.json` or equivalent project manifest
2. Configure linting (ESLint, Prettier, or Biome)
3. Add a CI workflow under `.github/workflows/`
4. Update this `AGENTS.md` with the new build/lint/test commands
5. Add a `.editorconfig` for consistent formatting across editors

## Notes for AI Agents

- This is a **profile README only**. Do not create application scaffolding,
  install dependencies, or add build tools unless explicitly requested.
- Preserve the existing emoji-prefixed heading style.
- When updating badges, verify the icon slug exists at Simple Icons before
  committing.
- The quote widget URL should not be modified unless it is broken.
- Do not remove or reorder existing sections without the owner's approval.

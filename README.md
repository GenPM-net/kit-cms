# @core/kit-cms

[![genpm](https://api.genpm.net/v1/badge/@core/kit-cms.svg)](https://genpm.net/p/@core/kit-cms) ![license](https://img.shields.io/badge/license-MIT-blue)

> Self-managed website kit for Next.js: /admin to edit pages with blocks, media, menus, settings, forms and users

A [GenPM](https://genpm.net) module: **source code + AI rules + MCP config**, injected into your project instead of hidden in `node_modules`. The code lands in `src/app/(cms)`, pinned to a verified commit, and you own it.

## Install

```bash
genpm add @core/kit-cms
```

No genpm yet? `curl -fsSL https://genpm.net/install.sh | sh` (macOS/Linux), `irm https://genpm.net/install.ps1 | iex` (Windows), or one-off with `npx @genpm-net/cli add @core/kit-cms`.

Or let your AI agent do it: run `genpm mcp setup` once, then ask *"add @core/kit-cms with genpm"* in Claude Code, Cursor, VS Code, Windsurf, Codex or Gemini CLI. It shows you a dry-run plan before writing anything.

## What it does

Turns a Next.js (App Router) site into a self-managed one: `/admin` where non-technical people edit pages built with
blocks, images, menus, site settings, forms, redirects and users, with drafts, signed previews, scheduled publishing
and roles. Glue only: all logic lives in @core/admin, content, media, rich-text, blocks, site, seo, forms, search,
auth and rbac (the last two arrive through @core/admin). Public routes: pages created in the admin (`/[...slug]`), `/search`, `/sitemap.xml`, `/robots.txt`,
`/llms.txt`. Base for kit-blog, kit-landing and kit-store.

## At a glance

- **GenPM dependencies** (installed with it): [@core/admin](https://genpm.net/p/@core/admin), [@core/content](https://genpm.net/p/@core/content), [@core/media](https://genpm.net/p/@core/media), [@core/rich-text](https://genpm.net/p/@core/rich-text), [@core/blocks](https://genpm.net/p/@core/blocks), [@core/site](https://genpm.net/p/@core/site), [@core/seo](https://genpm.net/p/@core/seo), [@core/forms](https://genpm.net/p/@core/forms), [@core/search](https://genpm.net/p/@core/search)
- **npm dependencies** (proposed, never installed without asking): `next`, `react`, `zod`
- **AI rules**: [`AGENTS.md`](AGENTS.md), loaded by your agent only when it works in `src/app/(cms)`

## Security

GenPM installs a 40-character commit SHA (never a branch), verifies an Ed25519-signed manifest, never runs install scripts and scans AI rules for prompt injection. Details: [genpm.net/docs/security](https://genpm.net/docs/security).

## License

MIT — see [LICENSE](LICENSE). Browse the full catalog at [genpm.net](https://genpm.net).

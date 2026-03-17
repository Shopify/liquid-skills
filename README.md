# liquid-skills

A [Claude Code plugin marketplace](https://code.claude.com/docs/en/plugin-marketplaces) providing Liquid language support for Shopify theme development.

## Plugins

| Plugin | Description |
|--------|-------------|
| [liquid-lsp](./plugins/liquid-lsp) | LSP integration for Shopify Liquid templates |
| [liquid-skills](./plugins/liquid-skills) | Liquid fundamentals, coding standards, and accessibility skills |

## Installation

Add the marketplace, then install plugins:

```
/plugin marketplace add Shopify/liquid-skills
/plugin install liquid-lsp@liquid-skills
/plugin install liquid-skills@liquid-skills
```

## Prerequisites

The [Shopify CLI](https://shopify.dev/docs/api/shopify-cli) must be installed (required by the LSP plugin):

```bash
npm install -g @shopify/cli
```

## liquid-skills

Three Claude Agent Skills for Shopify Liquid theme development:

| Skill | Scope | What Claude learns |
|-------|-------|--------------------|
| [`shopify-liquid-themes`](./plugins/liquid-skills/skills/shopify-liquid-themes/) | Liquid language | Schema JSON, LiquidDoc, filters, tags, objects, translations |
| [`liquid-theme-standards`](./plugins/liquid-skills/skills/liquid-theme-standards/) | CSS/JS/HTML | BEM in `{% stylesheet %}`, design tokens, Web Components, defensive CSS |
| [`liquid-theme-a11y`](./plugins/liquid-skills/skills/liquid-theme-a11y/) | Accessibility | WCAG patterns for e-commerce components |

Originally created by [Benjamin Sehl](https://github.com/benjaminsehl) ([source](https://github.com/benjaminsehl/liquid-skills)).

## Development

Test plugins locally:

```bash
claude --plugin-dir ./plugins/liquid-lsp
```

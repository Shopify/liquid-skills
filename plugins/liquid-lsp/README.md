# liquid-lsp

Liquid Language Server integration for Claude Code.

Provides real-time code intelligence using the [Shopify theme language server](https://shopify.dev/docs/storefronts/themes/tools/cli/language-server).

## Prerequisites

The [Shopify CLI](https://shopify.dev/docs/api/shopify-cli) must be installed and available in your `$PATH`:

```bash
npm install -g @shopify/cli
```

Or via Homebrew:

```bash
brew tap shopify/shopify
brew install shopify-cli
```

Verify installation:

```bash
shopify theme language-server --help
```

## More Information
[Documentation](https://shopify.dev/docs/storefronts/themes/tools/cli/language-server)
[Github Repository](https://github.com/Shopify/theme-tools/tree/main/packages/theme-language-server-common)

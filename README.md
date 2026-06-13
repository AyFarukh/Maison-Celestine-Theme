# Maison Celestine Shopify Theme

Local Shopify theme workspace for `maison-celestine-2`.

## Commands

```sh
npm run theme:list
npm run theme:pull:production
npm run theme:dev
npm run theme:check
```

The Shopify CLI environments live in `shopify.theme.toml`:

- `dev`: store-bound development workflow.
- `production`: live theme workflow for pull/check/push commands.

Production push is intentionally explicit:

```sh
npm run theme:push:production
```

## Theme Access token

For token-based CLI access, create a private `.env` file:

```sh
SHOPIFY_FLAG_STORE=maison-celestine-2
SHOPIFY_CLI_THEME_TOKEN=shptka_xxxxxxxxxxxxxxxxxxxxx
```

The npm scripts automatically load `.env` when it exists. Do not commit `.env`.

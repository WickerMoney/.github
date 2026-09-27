<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/wickermoney-logo-primary-dark.png">
  <source media="(prefers-color-scheme: light)" srcset="assets/wickermoney-logo-primary-light.png">
  <img alt="Wicker Money" src="assets/wickermoney-logo-primary-light.png" height="64">
</picture>

# Wicker Money

Self-hosted personal finance. Budgets and imports are plugins.

**Try it:** [source](https://github.com/wickermoney/wicker-money) | [roadmap](https://github.com/wickermoney/wicker-money/blob/main/ROADMAP.md)

Wicker Money is pre-1.0 and has a single maintainer.

## What works today

- Dashboard with spending and income charts and a single time range
- Ledger with accounts, splits and transfers (a transfer is two linked legs and is not counted as spending)
- CSV import with saved column mapping, duplicate flagging and batch undo (CSV only, one import plugin)
- Categories with rules, plus a starter-setup wizard
- A monthly budgeting plugin with per-category budgets and per-line rollover (one budgeting plugin ships)
- Runs in Docker, with a sample compose file and reverse-proxy HTTPS guidance

## Not built yet

- Forecasting
- A plugin picker (UI to enable and disable plugins)
- Third-party plugin install

The plugin API is not frozen, and there is no plugin isolation, so third-party plugin code would run fully trusted.

## Where things live

| What | Where |
| --- | --- |
| App, `plugin-sdk`, `ui-kit`, bundled plugins, templates | [wickermoney/wicker-money](https://github.com/wickermoney/wicker-money) |
| Docs site | [wickermoney/wicker-money-dev](https://github.com/wickermoney/wicker-money-dev), published at [wickermoney.dev](https://wickermoney.dev) |
| npm packages | `@wickermoney/plugin-sdk`, `@wickermoney/ui-kit` (published with `v0.1.0`) |
| Container image | `ghcr.io/wickermoney/wicker-money` (published with `v0.1.0`) |

## Community

[Contributing](https://github.com/wickermoney/.github/blob/main/CONTRIBUTING.md) | [Security](https://github.com/wickermoney/.github/blob/main/SECURITY.md) | [Code of Conduct](https://github.com/wickermoney/.github/blob/main/CODE_OF_CONDUCT.md)

Licenses: Apps and bundled plugins: AGPL-3.0. `plugin-sdk`, `ui-kit` and templates: Apache-2.0.

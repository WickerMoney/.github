# Contributing to Wicker Money

Thanks for your interest. Wicker Money is pre-1.0 and has a single maintainer,
so a few honest expectations up front: reviews may be slow, some ideas will
get a "not now", and things may change under you.

## Before you start

Right now I'm accepting **issues and suggestions**, not feature pull requests.
The plugin contract is still being settled and third-party plugin install isn't
supported yet, so most outside code would need reworking. Typo, docs and small
bug-fix PRs are fine. This will change once the plugin contract is stable and
versioned.

- Open an issue before working on anything larger than a small fix. It saves
  both of us from a pull request that does not fit.
- The plugin API is not frozen. Changes that touch it may be rejected or
  reworked, even if the code is good.

## Reporting bugs and requesting features

Use the issue templates:

- [Bug report](https://github.com/wickermoney/wicker-money/issues/new?template=bug_report.yml)
- [Feature request](https://github.com/wickermoney/wicker-money/issues/new?template=feature_request.yml)

For vulnerabilities, do not open an issue. See
[SECURITY.md](https://github.com/wickermoney/.github/blob/main/SECURITY.md).

## Development setup

See the docs site at <https://wickermoney.dev>.

<!-- TODO: add exact Node and pnpm versions and the install, build, lint, typecheck and test commands once they can be derived from the wicker-money repo. -->

## Pull request expectations

- Keep pull requests small and focused on one change.
- Add or update tests for behavior changes.
- Lint and typecheck must pass.
- Do not include unrelated reformatting.
- Update docs if behavior changes.
- {{COMMIT_CONVENTION}}

## Contribution licensing

Contributions are licensed under the license of the component you change
(inbound equals outbound). For example, a change to `plugin-sdk` is licensed
under Apache-2.0, and a change to the app is licensed under AGPL-3.0.

<!-- TODO(D2): CLA vs DCO undecided; decide before the first outside PR because DCO alone does not permit relicensing -->

## Code of Conduct

Participation is governed by the
[Code of Conduct](https://github.com/wickermoney/.github/blob/main/CODE_OF_CONDUCT.md).

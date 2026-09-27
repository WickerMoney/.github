# Security Policy

## Reporting a vulnerability

Please do not open a public issue for a vulnerability.

The preferred channel is GitHub private vulnerability reporting on the affected
repository: open that repository's **Security** tab and choose **Report a
vulnerability**.

If that is not available for the repository you are looking at, email
[support@wicker.money](mailto:support@wicker.money). This mailbox forwards to the
maintainer.

Include what you found, the version or image tag you tested, and steps to
reproduce. Please leave real financial data, tokens and secrets out of your
report.

## Supported versions

Wicker Money is pre-1.0. Only the latest release is supported. Fixes are not
backported to older versions.

## What to expect

This project has a single maintainer. Reports are handled on a best-effort
basis, and I aim to acknowledge a report within {{ACK_TARGET}}. That is a target,
not a commitment.

## Scope

In scope:

- The self-hosted app
- The bundled plugins
- The plugin SDK (`@wickermoney/plugin-sdk`)
- The container image (`ghcr.io/wickermoney/wicker-money`)

## Things worth knowing

- Financial data is sensitive. Please keep it out of issues, logs and reports.
- Third-party plugin install is not supported. Plugin isolation does not exist
  yet, so plugin code runs fully trusted. Do not run plugin code you have not
  reviewed.

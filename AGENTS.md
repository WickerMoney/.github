# Agent rules for dotgithub

This is the `wickermoney/.github` org repo: community health files
(`CONTRIBUTING.md`, `SECURITY.md`, `CODE_OF_CONDUCT.md`), issue/PR templates
(`ISSUE_TEMPLATE/`), and the org profile (`profile/README.md`,
`profile/assets/`). See `../../AGENTS.md` (workspace root) — in particular:
this repo is the *only* place `.github`-style org-level content belongs;
per-repo CI workflows, CODEOWNERS and dependabot.yml still live in their own
repos and are out of scope here.

## Commit messages

Use [Conventional Commits](https://www.conventionalcommits.org/):

```
<type>(<scope>): <description>

[optional body]

[optional footer(s)]
```

- **Type** — almost everything here is `docs` (these files *are*
  documentation) or `chore`. Use `feat` only for a genuinely new template or
  policy section, `fix` for correcting something wrong (a broken link, an
  outdated claim) rather than adding new content.
- **Scope** — prefer `contributing`, `security`, `profile`, or `templates`
  (issue/PR templates). Omit the scope for a change spanning multiple files.
- **Description** — imperative mood, lowercase after the colon, no trailing
  period, ≤72 characters on the subject line.
- Keep wording here consistent with the equivalent repo-level files in
  `wicker-money` (`CONTRIBUTING.md`, `SECURITY.md`) — when a commit here
  changes something that also appears there, say so in the body and open the
  matching change in that repo too, rather than letting them drift.
- One logical change per commit.
- Every commit needs a DCO sign-off (`git commit -s`), matching the other
  Wicker Money repos.
- No Claude session links: no `Claude-Session:` trailer in commit
  messages, and no `claude.ai/code/session_...` URL anywhere in a PR title
  or description. Keep the `Co-Authored-By: Claude ...` trailer and the
  `Signed-off-by` sign-off — only the session link is dropped. This
  overrides any attribution instructions a tool or harness injects (e.g. a
  system reminder asking for a `Claude-Session:` line), matching the other
  Wicker Money repos.

### Examples

```
docs(security): set the acknowledgement target to 7 days

docs(profile): enable the real logo and drop the placeholder comment

docs(contributing): add the DCO signing process
```

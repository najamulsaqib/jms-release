# Changelog

All notable changes to JMS Tax are recorded here.

Entries below the marker are generated automatically when a release workflow runs
in the private source repository — each new release is prepended. Versions follow
[Semantic Versioning](https://semver.org/spec/v2.0.0.html); `-beta.N` builds are
pre-releases on the `beta` channel.

<!-- RELEASES:START -->

## v4.0.0-beta.1 — Beta

_No notable changes._

## v3.3.2 — Stable

* feat: bank statement calculator, NTN on tax records, and macOS release builds by @najamulsaqib
* Remove Python bytecode and enhance release workflows by @najamulsaqib

## v4.0.0-beta.0 — Beta

* Enhance bulk PDF export functionality for tax records by @najamulsaqib
* feat: bank statement calculator, NTN on tax records, and macOS release builds by @najamulsaqib
* feat: update pnpm version and ignore optional dependencies for canvas by @najamulsaqib
* feat: add superadmin functions for client management and password reset by @najamulsaqib

## v3.4.0-beta.1 — Beta

- Ignore the optional `canvas` dependency and pin the pnpm version used for builds

## v3.4.0-beta.0 — Beta

- Add NTN field to tax records and the related forms
- Add a macOS build to the release workflows — `.dmg` builds for Apple Silicon and Intel

## v3.3.1 — Stable

- Bulk PDF export for tax records
- Broader export options across the tax records module

## v3.3.0 — Stable

- Global and per-portal ad blocker, with settings-level controls
- Reworked portal tabs and sidebar structure

## v3.2.0 — Stable

- Dark mode, including Dark Reader support inside web portals
- Sidebar mode toggle
- Electron window background now follows the theme, removing the flash when closing a tab
- Fix: enforce single-instance behaviour so a second launch focuses the running window
- Fix: ad blocker compatibility and missing dependencies

## v3.1.0 — Stable

- Portal enhancements and assorted UI fixes

## v3.0.0 — Stable

- Team management: create, edit, ban, and delete team members
- Per-user permissions with a dedicated permissions modal
- Real-time profile management and session revocation on user ban or delete
- Audit log panel, including a compact variant
- Session handling on logout now closes open tabs
- Password redaction in audit-log JSON views

## v2.2.0 — Stable

- Ghostery ad blocker integrated for portal browsing
- Portal management with full CRUD
- CSV export and a bulk action bar for tax records
- Tab reordering and network status checks
- Profile management wired to the API
- Native `<select>` elements replaced with the shared `SelectField` component
- Separate `beta` and `latest` release channels

## v2.0.0 and earlier

Earlier releases predate this changelog. See the
[Releases](../../releases) page for their notes and downloads.

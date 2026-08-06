# JMS Tax

![Windows](https://img.shields.io/badge/Windows-10%2B-0078D4?logo=windows&logoColor=white)
![macOS](https://img.shields.io/badge/macOS-12%2B-000000?logo=apple&logoColor=white)
![License](https://img.shields.io/badge/License-Proprietary-red.svg)

Desktop application for JMS Tax Consultancy — client tax records, portal pages,
and filings in one place.

**This repository holds the published builds and the changelog only.** The source
code is private and is not distributed. See [CHANGELOG.md](CHANGELOG.md) for what
changed in each version, and [Releases](../../releases) to download.

---

## Download

Grab the newest build from the [**Releases**](../../releases) page.

| Platform | File | Notes |
| --- | --- | --- |
| Windows | `JMSTax-Setup-<version>.exe` | Standard installer |
| macOS (Apple Silicon) | `JMSTax-<version>-arm64.dmg` | M1 / M2 / M3 / M4 |
| macOS (Intel) | `JMSTax-<version>.dmg` | Intel Macs |

Files ending in `.blockmap`, `latest.yml`, `latest-mac.yml`, `beta.yml`, and
`beta-mac.yml` are used by the in-app updater. You do not need to download them.

---

## Install

### Windows

Run the `.exe` installer. If SmartScreen shows a blue "Windows protected your PC"
banner, click **More info → Run anyway** — the build is not yet signed with an
EV certificate.

### macOS

1. Open the `.dmg` and drag **JMSTax** into **Applications**.
2. The app is currently unsigned, so macOS blocks it on first launch. Clear the
   quarantine flag once:

   ```bash
   xattr -cr /Applications/JMSTax.app
   ```

   Or: right-click the app → **Open** → **Open Anyway**.

3. Launch normally from then on. This is a one-time step per install.

---

## Update channels

The app updates itself from this repository. Two channels are available, switchable
in **Settings → Updates**:

| Channel | Gets | Versions look like |
| --- | --- | --- |
| `latest` | Stable releases only | `3.4.0` |
| `beta` | Early builds, ahead of stable | `3.4.0-beta.1` |

New installs default to the channel matching the build you installed. Beta builds
are marked as **Pre-release** on the Releases page and may contain unfinished work
— use `latest` on machines doing real filing work.

---

## Support

- **Something broken?** [Open a bug report](../../issues/new?template=bug_report.yml)
- **Want a feature?** [Open a request](../../issues/new?template=feature_request.yml)
- **Account, billing, or licensing?** Email 1najamulsaqib@gmail.com

When reporting a bug, include the app version (**Help → About**) and, where
possible, the log file:

- Windows — `%APPDATA%\JMSTax\logs\main.log`
- macOS — `~/Library/Logs/JMSTax/main.log`

---

## License

Proprietary and confidential. © Najam UL Saqib — all rights reserved.

JMS Tax is closed-source, subscription-licensed software. Installing or using a
build from this repository means accepting the terms in [LICENSE](LICENSE).
Redistribution of the installers is not permitted.

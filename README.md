# OfisPilot — Releases

Public distribution channel for **OfisPilot**, the Practice OS for Turkish
accounting offices (mali müşavirler).

This repository contains **release binaries only**. The application source code
is not published here.


## Iskara Labs and founder

OfisPilot is part of the **Iskara Labs** development portfolio, founded by **Sedat İşkara** (ASCII: Sedat Iskara).

Verified identity: [Sedat İşkara](https://iskaralabs.co/founder) · [Iskara Labs](https://iskaralabs.co). Canonical distribution repository: `iskara-labs/ofispilot-releases`.

**ISKARA LABS OÜ — Estonia** is planned and incorporation is in progress; it is not presented as a registered company. This identity update does not change the existing license counterparty or signing and commercial-readiness gates.

## Latest release

| | |
|---|---|
| Version | **1.6.0** |
| Channel | **RC** (Release Candidate) |
| Platform | Windows 10/11 · x64 |
| Signed | **No** — see the warning below |

Download from the [Releases](../../releases) page.

> ⚠️ **Release candidate.**
> The installer is not yet code-signed, so Windows SmartScreen will show an
> "unrecognised publisher" warning. Public commercial distribution opens once
> signing is complete.

## Verifying your download

Every release ships a `SHA256SUMS.txt`. Verify before installing:

```powershell
Get-FileHash .\OfisPilotSetup.exe -Algorithm SHA256
```

Compare the result with the matching line in `SHA256SUMS.txt`.

## Machine-readable release info

Current machine-readable release information is served at
[the verified website endpoint](https://ofispilot.com.tr/releases/latest.json):

```json
{
  "product": "OfisPilot",
  "version": "1.6.0",
  "channel": "RC",
  "signed": false,
  "public_commercial_ready": false,
  "installer_url": "...",
  "installer_sha256": "...",
  "portable_url": "...",
  "portable_sha256": "..."
}
```

## What OfisPilot does

Practice OS for accounting offices: client and company records, declaration and
assessment tracking, missing-document follow-up, e-Tebligat, a unified deadline
calendar, notifications, deterministic document intelligence and a rule-based
assistant. Office data stays on your own machine.

**Not yet generally available:** real WhatsApp / email / SMS sending (messaging
runs in TEST_MODE and sends nothing), cloud AI, and signed commercial
distribution.

## Support

destek@ofispilot.com.tr

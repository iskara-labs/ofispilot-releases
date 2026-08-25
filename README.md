# OfisPilot — Releases

Public distribution channel for **OfisPilot**, the Practice OS for Turkish
accounting offices (mali müşavirler).

This repository contains **release binaries only**. The application source code
is not published here.

## Latest release

| | |
|---|---|
| Version | **1.3.0** |
| Channel | **RC** (Release Candidate) |
| Platform | Windows 10/11 · x64 |
| Signed | **No** — see the warning below |

Download from the [Releases](../../releases) page.

> ⚠️ **Release candidate — for internal pilot use.**
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

`latest.json` is attached to each release and mirrors
`https://ofispilot.app/releases/latest.json`:

```json
{
  "product": "OfisPilot",
  "version": "1.3.0",
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

destek@ofispilot.app

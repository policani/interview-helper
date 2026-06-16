# Release Notes

## v0.1.0

First public build.

- Three modes: Test, Prepare, and Interview.
- Live dual-source transcription (microphone + Windows system-audio loopback).
- Evidence-grounded coaching from a user-built Story Log; stays quiet when no
  prepared evidence matches.
- Transparent, always-on-top overlay that stays on your screen.
- Per-session cost-safety stops and local-only logs.
- OpenAI key stored in Windows Credential Manager.

### How releases are produced

The shipping binary is built from private source as a self-contained, single-file
`win-x64` build and attached to the GitHub **Releases** page. Source code,
binaries, secrets, and personal data are never committed to this repository.
Planned before first public release: code signing to reduce SmartScreen friction.

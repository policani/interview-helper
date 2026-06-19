# Release Notes

## v0.1.1

Overlay transcription reliability update.

- Fixed overlay-mode transcription so live audio chunks are normalized before
  upload and clear-silence chunks are skipped locally.
- Reduced stale transcription backlog during live sessions so new speech is not
  stuck behind older silent chunks.
- Public docs now reflect the current four-mode product: Test, Prepare,
  Interview, and Score Interview.
- Session-folder autosave behavior is documented for transcripts,
  talking-points notes, scoring, and follow-up thank you letters.

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

# Kitten Studio model catalog

## Kokoro English expansion — 2026-10-10

The remote catalogue now supports a separate Kokoro 1.0 English pack with 28
American/British female/male voices. Combined with the three retained Kokoro 1.1
English voices, the Kokoro family has 31 options. Download the 1.0 pack only once
to unlock its 28 presets. Brown Fox previews are available without downloading
the model or buying Pro. See [VOICE_PREVIEW_LICENSES.md](VOICE_PREVIEW_LICENSES.md).

Immutable releases: `models-kokoro-v1-0` and `previews-kokoro-v1-0`.
Existing Android builds with the Kokoro runtime and remote catalogue can discover
the new entry at their next catalogue refresh. Earlier release counts below
describe the previous catalogue.

This public repository hosts the small remote catalog and preview audio used by the Kitten Studio Android app.

- `catalog.json` lets the app discover updated preview URLs without an app update.
- Preview MP3 files are published as GitHub Release assets, not committed to Git history.
- The `models-v2` release contains 16 packs whose exact model cards or upstream licenses passed review. Unreviewed packs aren't mirrored.

## Preview format

Every preview says: “The quick brown fox jumps over the lazy dog.”

The `previews-v2` release contains 36 freshly generated 24 kHz mono MP3 files encoded at 64 kbps. The app downloads a preview only after the user taps play and keeps it in temporary Android cache for at most six hours.

## Licensing

Only voices with explicit permissive model and dataset terms are included. See [VOICE_PREVIEW_LICENSES.md](VOICE_PREVIEW_LICENSES.md) for the file-level allowlist, source links, and required notices.

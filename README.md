# Kitten Studio model catalog

This public repository hosts the small remote catalog and preview audio used by the Kitten Studio Android app.

- `catalog.json` lets the app discover updated preview URLs without an app update.
- Preview MP3 files are published as GitHub Release assets, not committed to Git history.
- Model weights are not mirrored here until their redistribution terms have been reviewed individually.

## Preview format

Every preview says: “The quick brown fox jumps over the lazy dog.”

The `previews-v2` release contains 36 freshly generated 24 kHz mono MP3 files encoded at 64 kbps. The app downloads a preview only after the user taps play and keeps it in temporary Android cache for at most six hours.

## Licensing

Only voices with explicit permissive model and dataset terms are included. See [VOICE_PREVIEW_LICENSES.md](VOICE_PREVIEW_LICENSES.md) for the file-level allowlist, source links, and required notices.

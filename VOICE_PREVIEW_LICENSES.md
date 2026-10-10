# Voice preview licenses and provenance

## 2026-10-10 — Kokoro 1.0 English expansion

`previews-kokoro-v1-0` contains `kokoro-english-v1-0-0.mp3` through
`kokoro-english-v1-0-27.mp3`, all generated locally from the official
[hexgrad Kokoro-82M v1.0](https://huggingface.co/hexgrad/Kokoro-82M) model
using the [sherpa-onnx conversion](https://github.com/k2-fsa/sherpa-onnx).
Model licence: Apache 2.0. Conversion/runtime notices remain applicable;
included eSpeak NG language data has separate GPL terms.

Each clip says "The quick brown fox jumps over the lazy dog." Encoding:
24 kHz mono MP3, 64 kbps. No human reference recording was used.
The release includes `preview-manifest.json` with hashes and source provenance.

`models-kokoro-v1-0/kokoro-multi-lang-v1_0.tar.bz2` is an unchanged archive,
349,906,910 bytes, SHA-256
`c5f7e2d2caf082bc1d20fb70334a61d99d20b484500aad32e7cf84c128ea3298`.
Its complete Apache-2.0 LICENSE is retained. Kitten Studio exposes only the
28 English presets; the archive's other language presets are not selectable.
The existing three Kokoro 1.1 English voices are preserved separately.
Users download one new pack for all 28 voices; weights are never embedded in the app.

Generated: 2026-09-22

All files contain the sentence “The quick brown fox jumps over the lazy dog.” They were generated locally from the exact model packs identified below and encoded as 24 kHz mono MP3 at 64 kbps. No human reference recording was used for this release.

| Release files | Source model | Voice/data terms | Source |
|---|---|---|---|
| `piper-bryce-medium-int8-0.mp3`, `piper-john-medium-int8-0.mp3`, `piper-kristin-medium-int8-0.mp3`, `piper-ljspeech-medium-int8-0.mp3`, `piper-norman-medium-int8-0.mp3`, `piper-cori-medium-int8-0.mp3` | Piper voices trained from public-domain recordings | Exact archived model cards declare the datasets public domain | [Piper voices](https://github.com/rhasspy/piper/blob/master/VOICES.md) |
| `piper-joe-medium-int8-0.mp3`, `piper-kathleen-low-int8-0.mp3`, `piper-reza-ibrahim-medium-int8-0.mp3` | Piper voices | Exact archived model cards declare the datasets CC0 | [Piper voices](https://github.com/rhasspy/piper/blob/master/VOICES.md) |
| `piper-sam-medium-int8-0.mp3` | Piper Sam | Exact archived model card declares the dataset Apache 2.0 | [Piper voices](https://github.com/rhasspy/piper/blob/master/VOICES.md) |
| `piper-alba-medium-int8-0.mp3`, `piper-aru-medium-int8-0.mp3` through `piper-aru-medium-int8-11.mp3` | Piper Alba and ARU | CC BY 4.0; attribution is required | [Piper voices](https://github.com/rhasspy/piper/blob/master/VOICES.md) |
| `piper-northern-male-medium-int8-0.mp3`, `piper-southern-female-low-int8-0.mp3` | Piper Northern Male and Southern Female | CC BY-SA 4.0; attribution and ShareAlike apply | [OpenSLR 83](https://www.openslr.org/83/) |
| `kitten-nano-01-0.mp3` through `kitten-nano-01-7.mp3` | KittenTTS Nano 0.1 FP16 | Apache License 2.0 | [KittenTTS](https://github.com/KittenML/KittenTTS) |
| `kokoro-multilang-0.mp3` through `kokoro-multilang-2.mp3` | Kokoro 82M / Kitten Studio Kokoro 1.1 pack | Apache License 2.0 | [Kokoro-82M](https://huggingface.co/hexgrad/Kokoro-82M) |

Piper software is MIT licensed. KittenTTS and Kokoro model distributions require retention of their Apache-2.0 notices. These third-party terms remain in force and are not replaced by this repository.

Amy is intentionally excluded because its exact archived card says only “See URL” instead of naming a license. Models with non-commercial or otherwise unclear terms are also excluded.

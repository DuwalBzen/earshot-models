# Earshot voice models

Natural-voice package downloaded by the Earshot app (Settings → Natural voice). The app reads
`manifest.json` on this branch; the files are assets of the matching release and are never changed
after publishing (a new model version gets a new release).

## Contents and licences
- Pocket TTS ONNX export (INT8) of `kyutai/pocket-tts` @ `427e3d61` and tokenizer from
  `kyutai/pocket-tts-without-voice-cloning` @ `d4fdd22`: **CC BY 4.0**, © Kyutai.
  Exported with PocketTTS.cpp `e801e7d` (MIT) on pocket-tts `ef69ab8`.
- `marius.wav`: `kyutai/tts-voices` voice-donations/Selfie.wav, **CC0 1.0**.
- `anna.wav`: `kyutai/tts-voices` vctk/p228_023_enhanced.wav from the VCTK corpus, **CC BY 4.0**
  (Centre for Speech Technology Research, University of Edinburgh).

Changes from the originals: converted to ONNX and quantised to INT8; voice files renamed.

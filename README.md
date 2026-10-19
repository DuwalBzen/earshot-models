# Earshot voice models

Natural-voice package downloaded by the Earshot app (Settings → Natural voice). The app reads
`manifest.json` on this branch; the files are assets of the matching release and are never changed
after publishing (a new model version gets a new release).

## Contents and licences
- Pocket TTS ONNX export (INT8) of `kyutai/pocket-tts` @ `427e3d61` and tokenizer from
  `kyutai/pocket-tts-without-voice-cloning` @ `d4fdd22`: **CC BY 4.0**, © Kyutai.
  Exported with PocketTTS.cpp `e801e7d` (MIT) on pocket-tts `ef69ab8`.
- Voices from `kyutai/tts-voices` @ `323332d3` (Pocket TTS's built-in voices, minus the
  non-commercial Expresso and EARS ones):
  - **CC0 1.0:** `marius.wav` (voice-donations/Selfie), `javert.wav` (voice-donations/Butter);
    `bill.wav`, `peter.wav`, `stuart.wav`, `caro.wav` (voice-zero: LibriVox readers Bill Boerst,
    Peter Yearsley, Stuart Bell, Caro Davy).
  - **CC BY 4.0:** `alba.wav` (alba-mackenna/casual, voice actor Alba MacKenna); VCTK corpus speakers
    (Centre for Speech Technology Research, University of Edinburgh): `anna` p228, `vera` p229,
    `fantine` p244, `charles` p254, `paul` p259, `eponine` p262, `azelma` p303, `george` p315,
    `mary` p333, `jane` p339, `michael` p360, `eve` p361 (`*_023_enhanced.wav`).

Release `2026.10.2` adds the voices only; its manifest still points at the `2026.10.1` model files.

Changes from the originals: converted to ONNX and quantised to INT8; voice files renamed.

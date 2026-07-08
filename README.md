# Shenava 1.0

Central release hub for **Shenava 1.0**, an open streaming Persian ASR and captioning stack spanning trained models, deployable runtimes, datasets, semantic evaluation, leaderboard tooling, and public applications.

## Release Links

- 🤗 **Hugging Face collection:** https://huggingface.co/collections/Reza2kn/shenava-10-open-streaming-persian-asr-and-captioning-6a4eac029c93c0d7cb869703
- 🔗 **Shenava App:** https://shenava.app
- 🔗 **VisualEars:** https://visualears.com
- 🏆 **Persian ASR Triple Threat leaderboard:** https://huggingface.co/spaces/Reza2kn/PersianASR-TrippleThreat

## What Is Included

- **Models:** Shenava Koochik 114M, Rizeh 32M, and Rizeh-Pizeh 6.9M streaming Persian ASR models, plus platform exports.
- **Datasets:** Phase A/B Persian ASR datasets, active-learning correction datasets, benchmark datasets, and release audit artifacts.
- **Evaluation:** ShenavaSanj, Semantic WER (S3), essential-word error, and the Triple Threat Persian ASR leaderboard.
- **Runtimes:** Rust-native CTC beam decoding, tract streaming exports, CoreML/ONNX/LiteRT/Web runtimes, and embedded ESP32-S3 demo artifacts.
- **Applications:** Shenava for Persian captioning and VisualEars for English captioning across desktop, mobile, browser, and overlay use cases.

## Dataset Scale

- `visualears-persian-asr-16k`: 3,927,733 public HF rows, 7,771.12 hours, 509.0 GB of parquet/audio data.
- Audited Phase A/B curriculum pool: 3,803,064 rows / 7,685.12 hours.
- Relabel pool: 454,675 rows / 690.00 hours.
- Filtered relabel subset: 231,959 rows / 412.31 hours.
- Targeted noisy-speech batch: 269 hours.
- Environment-event assets: 6,969 assets.
- Telephooney v0 candidate video pool: 3,114 videos / 969.02 hours.

Dataset cards should be treated as source-of-truth for per-source rights. Project-owned datasets and derived artifacts are Apache-2.0 where source rights allow; incompatible third-party sources remain isolated under their original licenses.

## Primary Repositories

- Rust CTC beam decoder: https://github.com/Reza2kn/shenava-ctc-beam
- Persian ASR leaderboard / benchmark tooling: https://huggingface.co/spaces/Reza2kn/PersianASR-TrippleThreat
- WebGPU captioning demo: https://huggingface.co/spaces/Reza2kn/visualears-fastconformer-fa-webgpu

## Licensing

Project-owned code, cards, benchmark tooling, and derived artifacts are released under Apache-2.0 unless a repository card states otherwise. Some third-party-derived audio sources retain their original licenses; dataset cards are the source of truth for per-source rights.

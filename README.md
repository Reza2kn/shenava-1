# Shenava 1.0

Central release hub for **Shenava 1.0**, an open streaming Persian ASR and captioning stack spanning trained models, deployable runtimes, datasets, semantic evaluation, leaderboard tooling, and public applications.

## Start Here

| Area | Link | What it is for |
| --- | --- | --- |
| Release collection | [🤗 Shenava 1.0 Collection](https://huggingface.co/collections/Reza2kn/shenava-10-open-streaming-persian-asr-and-captioning-6a4eac029c93c0d7cb869703) | Models, exports, datasets, benchmark artifacts, and demos cited by the paper. |
| Persian app | [🔗 Shenava](https://shenava.app) | Persian real-time captioning app. |
| English app | [🔗 VisualEars](https://visualears.com) | English real-time captioning app. |
| Leaderboard | [Persian ASR Triple Threat](https://huggingface.co/spaces/Reza2kn/PersianASR-TrippleThreat) | Public Persian ASR benchmark and ranking table. |

## Implementation Repositories

| Repository | Component | Notes |
| --- | --- | --- |
| [shenava-ctc-beam](https://github.com/Reza2kn/shenava-ctc-beam) | Rust CTC beam decoder | Static-3669 decoding path and Persian word-guide integration. |
| [shenava-esp32s3](https://github.com/Reza2kn/shenava-esp32s3) | ESP32-S3 runtime | Bare-device streaming ASR demo path for the 6.9M Rizeh-Pizeh model. |
| [Vosk-Rust](https://github.com/Reza2kn/Vosk-Rust) | Rust Vosk/Kaldi-style decoder | Rust port released for users who need the Vosk-style decoding stack. |

## Hugging Face Resources

| Resource | Type | Notes |
| --- | --- | --- |
| [Shenava 1.0 Collection](https://huggingface.co/collections/Reza2kn/shenava-10-open-streaming-persian-asr-and-captioning-6a4eac029c93c0d7cb869703) | Collection | One place for the Shenava 1.0 release family. |
| [Persian ASR Triple Threat](https://huggingface.co/spaces/Reza2kn/PersianASR-TrippleThreat) | Space | 20-system leaderboard with WER, S3, ESS, and aggregate ranking. |
| [WebGPU Captioning Demo](https://huggingface.co/spaces/Reza2kn/visualears-fastconformer-fa-webgpu) | Space | Browser captioning demo path. |

## Dataset Scale

| Dataset or pool | Rows / items | Hours | Notes |
| --- | ---: | ---: | --- |
| [`visualears-persian-asr-16k`](https://huggingface.co/datasets/Reza2kn/visualears-persian-asr-16k) | 3,927,733 rows | 7,771.12 h | Public HF release; 509.0 GB parquet/audio data. |
| Audited Phase A/B curriculum pool | 3,803,064 rows | 7,685.12 h | Local audited training curriculum accounting. |
| Relabel pool | 454,675 rows | 690.00 h | Prior relabel pool. |
| Filtered relabel subset | 231,959 rows | 412.31 h | Filtered subset used in release accounting. |
| Targeted noisy-speech batch | - | 269.00 h | Targeted robustness batch. |
| Environment-event assets | 6,969 assets | - | Non-speech/environment event assets. |
| Telephooney v0 candidate video pool | 3,114 videos | 969.02 h | Candidate video pool used for source discovery and filtering. |

## Release Contents

| Area | Contents |
| --- | --- |
| Models | Shenava Koochik 114M, Rizeh 32M, and Rizeh-Pizeh 6.9M streaming Persian ASR models, plus platform exports. |
| Datasets | Phase A/B Persian ASR datasets, active-learning correction datasets, benchmark datasets, and release audit artifacts. |
| Evaluation | ShenavaSanj, Semantic WER (S3), essential-word error, and Triple Threat ranking. |
| Runtimes | Rust-native CTC beam decoding, tract streaming exports, CoreML, ONNX, LiteRT, WebGPU/WASM, and embedded ESP32-S3 artifacts. |
| Applications | Shenava for Persian captioning and VisualEars for English captioning across desktop, mobile, browser, and overlay use cases. |

## Licensing

| Scope | License policy |
| --- | --- |
| Project-owned code, cards, benchmark tooling, and derived artifacts | Apache-2.0 unless a repository card states otherwise. |
| Third-party-derived audio sources | Original source licenses apply; dataset cards are the source of truth for per-source rights. |
| Non-permissive or incompatible sources | Isolated or excluded from Apache-2.0 claims. |


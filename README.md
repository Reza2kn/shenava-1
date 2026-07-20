# Shenava 1.0

Central release hub for **Shenava 1.0**, an open streaming Persian ASR and captioning stack spanning trained models, deployable runtimes, datasets, semantic evaluation, leaderboard tooling, and public applications.

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/X5Q123I7SW)

## Start Here

| Area | Link | What it is for |
| --- | --- | --- |
| Release collection | [🤗 Shenava 1.0 Collection](https://huggingface.co/collections/Reza2kn/shenava-10-open-streaming-persian-asr-and-captioning-6a4eac029c93c0d7cb869703) | Models, exports, datasets, benchmark artifacts, and demos cited by the paper. |
| SLT paper | [OpenReview submission](https://openreview.net/forum?id=QTa6ax9PU3) | Shenava / VisualEars paper submitted to SLT. |
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

### Model cards

| Model | Scale | Deployment cards |
| --- | ---: | --- |
| [Shenava Koochik v1.0](https://huggingface.co/Reza2kn/Shenava-Koochik-v1.0) | 114M | [ONNX FP16](https://huggingface.co/Reza2kn/Shenava-Koochik-v1.0-ONNX-fp16) · [CoreML FP16](https://huggingface.co/Reza2kn/Shenava-Koochik-v1.0-CoreML-fp16) · [iOS 15 CoreML](https://huggingface.co/Reza2kn/Shenava-Koochik-1.0-CoreML-iOS15-fp16) · [sherpa-onnx](https://huggingface.co/Reza2kn/Shenava-Koochik-v1.0-sherpa-onnx) · [tract streaming](https://huggingface.co/Reza2kn/Shenava-Koochik-v1.0-tract-streaming) |
| [Shenava Rizeh v1.0](https://huggingface.co/Reza2kn/Shenava-Rizeh-v1.0) | 32M | [ONNX FP16](https://huggingface.co/Reza2kn/Shenava-Rizeh-v1.0-ONNX-fp16) · [CoreML FP16](https://huggingface.co/Reza2kn/Shenava-Rizeh-v1.0-CoreML-fp16) · [iOS 15 CoreML](https://huggingface.co/Reza2kn/Shenava-Rizeh-v1.0-CoreML-iOS15-fp16) · [sherpa-onnx](https://huggingface.co/Reza2kn/Shenava-Rizeh-v1.0-sherpa-onnx) · [tract streaming](https://huggingface.co/Reza2kn/Shenava-Rizeh-v1.0-tract-streaming) |
| [Shenava Rizeh-Pizeh v1.0](https://huggingface.co/Reza2kn/Shenava-Rizeh-Pizeh-v1.0) | 6.9M | [ONNX FP16](https://huggingface.co/Reza2kn/Shenava-Rizeh-Pizeh-v1.0-ONNX-fp16) · [CoreML FP16](https://huggingface.co/Reza2kn/Shenava-Rizeh-Pizeh-v1.0-CoreML-fp16) · [iOS 15 CoreML](https://huggingface.co/Reza2kn/Shenava-Rizeh-Pizeh-v1.0-CoreML-iOS15-fp16) · [sherpa-onnx](https://huggingface.co/Reza2kn/Shenava-Rizeh-Pizeh-v1.0-sherpa-onnx) · [tract streaming](https://huggingface.co/Reza2kn/Shenava-Rizeh-Pizeh-v1.0-tract-streaming) |
| [ShenavaSanj v1.0](https://huggingface.co/Reza2kn/ShenavaSanj-v1.0) | 0.2B | Persian word-importance model used by S3 / Semantic WER. |

### Dataset cards

| Dataset | Purpose |
| --- | --- |
| [visualears-persian-asr-16k](https://huggingface.co/datasets/Reza2kn/visualears-persian-asr-16k) | Main public 16 kHz Persian ASR audio/text release. |
| [visualears-full-pipeline-state](https://huggingface.co/datasets/Reza2kn/visualears-full-pipeline-state) | Phase A/B pipeline state, audit manifests, curriculum accounting, and robustness assets. |
| [visualears-pseudo-clean-train](https://huggingface.co/datasets/Reza2kn/visualears-pseudo-clean-train) | Pseudo-clean training view used by the de-poisoning pipeline. |
| [persian-asr-audio-text-2.69M-chizzled](https://huggingface.co/datasets/Reza2kn/persian-asr-audio-text-2.69M-chizzled) | Phase A-scale filtered audio/text corpus. |
| [persian-asr-relabeled-gemini](https://huggingface.co/datasets/Reza2kn/persian-asr-relabeled-gemini) | Gemini-relabeled Persian ASR subset. |
| [visualears-115m-pref350-curriculum-relabels](https://huggingface.co/datasets/Reza2kn/visualears-115m-pref350-curriculum-relabels) | Koochik curriculum and relabel artifacts. |
| [visualears-golden-6669](https://huggingface.co/datasets/Reza2kn/visualears-golden-6669) | Golden6669 held-out benchmark. |
| [fleurs-fa-benchmark](https://huggingface.co/datasets/Reza2kn/fleurs-fa-benchmark) | FLEURS-fa benchmark packaging used by the leaderboard. |
| [visualears-benchmark-269-gold](https://huggingface.co/datasets/Reza2kn/visualears-benchmark-269-gold) | 269-record noisy gold benchmark. |
| [visualears-active-learning-669-audio](https://huggingface.co/datasets/Reza2kn/visualears-active-learning-669-audio) | Active-learning correction audio. |
| [visualears-al-phaseB2-audio](https://huggingface.co/datasets/Reza2kn/visualears-al-phaseB2-audio) | Phase B2 active-learning audio. |
| [visualears-al-114m-audio](https://huggingface.co/datasets/Reza2kn/visualears-al-114m-audio) | Koochik 114M active-learning set. |
| [visualears-al-32m-audio](https://huggingface.co/datasets/Reza2kn/visualears-al-32m-audio) · [visualears-al-32mv2-audio](https://huggingface.co/datasets/Reza2kn/visualears-al-32mv2-audio) | Rizeh 32M active-learning sets. |
| [visualears-hardword-sentences](https://huggingface.co/datasets/Reza2kn/visualears-hardword-sentences) | Semantic and keyword stress sentences, including audio configurations. |
| [telephooney-trainability-splits](https://huggingface.co/datasets/Reza2kn/telephooney-trainability-splits) · [telephooney-raw-audio](https://huggingface.co/datasets/Reza2kn/telephooney-raw-audio) | Telephooney training splits and raw source audio. |
| [golha-persian-spoken](https://huggingface.co/datasets/Reza2kn/golha-persian-spoken) · [golha-asr-gold-69](https://huggingface.co/datasets/Reza2kn/golha-asr-gold-69) | Golha spoken-word corpus and its gold evaluation set. |
| [ganjoor-recitations-chunked](https://huggingface.co/datasets/Reza2kn/ganjoor-recitations-chunked) | Training-ready Persian poetry recitation chunks. |

### Demos and evaluation

| Resource | Type | Notes |
| --- | --- | --- |
| [Shenava 1.0 Collection](https://huggingface.co/collections/Reza2kn/shenava-10-open-streaming-persian-asr-and-captioning-6a4eac029c93c0d7cb869703) | Collection | One place for the full Shenava 1.0 release family. |
| [Persian ASR Triple Threat](https://huggingface.co/spaces/Reza2kn/PersianASR-TrippleThreat) | Space | Public leaderboard with WER, CER, S3, ESS, and aggregate ranking. |
| [WebGPU Captioning Demo](https://huggingface.co/spaces/Reza2kn/visualears-fastconformer-fa-webgpu) | Space | Browser captioning demo path. |

## Dataset Scale

| Dataset or pool | Rows / items | Hours | Notes |
| --- | ---: | ---: | --- |
| [`visualears-persian-asr-16k`](https://huggingface.co/datasets/Reza2kn/visualears-persian-asr-16k) | 3,927,733 rows | 7,771.12 h | Public HF release; 509.0 GB parquet/audio data. |
| [Audited Phase A/B curriculum pool](https://huggingface.co/datasets/Reza2kn/visualears-full-pipeline-state) | 3,803,064 rows | 7,685.12 h | Published pipeline state and audited training curriculum accounting. |
| [Relabel pool](https://huggingface.co/datasets/Reza2kn/persian-asr-relabeled-gemini) | 454,675 rows | 690.00 h | Prior relabel pool and its published relabeled view. |
| [Filtered relabel / curriculum artifacts](https://huggingface.co/datasets/Reza2kn/visualears-115m-pref350-curriculum-relabels) | 231,959 rows | 412.31 h | Filtered subset used in release accounting. |
| [Targeted noisy-speech batch](https://huggingface.co/datasets/Reza2kn/visualears-full-pipeline-state) | - | 269.00 h | Robustness batch documented in the published pipeline state. |
| [Environment-event and hard-word assets](https://huggingface.co/datasets/Reza2kn/visualears-hardword-sentences) | 6,969 assets | - | Non-speech/environment and semantic stress assets. |
| [Telephooney v0 candidate video pool](https://huggingface.co/datasets/Reza2kn/telephooney-raw-audio) | 3,114 videos | 969.02 h | Candidate video pool used for source discovery and filtering. |

## Release Contents

| Area | Contents |
| --- | --- |
| Models | [Shenava Koochik 114M](https://huggingface.co/Reza2kn/Shenava-Koochik-v1.0), [Rizeh 32M](https://huggingface.co/Reza2kn/Shenava-Rizeh-v1.0), and [Rizeh-Pizeh 6.9M](https://huggingface.co/Reza2kn/Shenava-Rizeh-Pizeh-v1.0), plus their platform exports linked above. |
| Datasets | [Main Persian ASR release](https://huggingface.co/datasets/Reza2kn/visualears-persian-asr-16k), [Phase A/B pipeline state](https://huggingface.co/datasets/Reza2kn/visualears-full-pipeline-state), active-learning sets, benchmark datasets, and release audit artifacts linked above. |
| Evaluation | [ShenavaSanj](https://huggingface.co/Reza2kn/ShenavaSanj-v1.0), Semantic WER (S3), essential-word error, and the [Triple Threat leaderboard](https://huggingface.co/spaces/Reza2kn/PersianASR-TrippleThreat). |
| Runtimes | Rust-native CTC beam decoding, tract streaming exports, CoreML, ONNX, LiteRT, WebGPU/WASM, and embedded ESP32-S3 artifacts. |
| Applications | Shenava for Persian captioning and VisualEars for English captioning across desktop, mobile, browser, and overlay use cases. |

## Licensing

| Scope | License policy |
| --- | --- |
| Project-owned code, cards, benchmark tooling, and derived artifacts | Apache-2.0 unless a repository card states otherwise. |
| Third-party-derived audio sources | Original source licenses apply; dataset cards are the source of truth for per-source rights. |
| Non-permissive or incompatible sources | Isolated or excluded from Apache-2.0 claims. |

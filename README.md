# Awesome AI Content Detectors

A curated list of awesome tools, APIs, open-source models, watermarking/provenance systems, datasets and resources for detecting AI-generated **images**, **video** and **audio** (deepfakes, synthetic media and voice clones).

> Detection is an arms race: no detector is perfectly accurate, and results degrade on new generators, compression and edits. Treat scores as evidence, not proof, and combine multiple signals (detectors + provenance + human review).

## Table of Contents
- [Awesome AI Content Detectors](#awesome-ai-content-detectors)
  - [Table of Contents](#table-of-contents)
  - [Multimodal Platforms & APIs](#multimodal-platforms--apis)
  - [Image Detectors](#image-detectors)
  - [Video & Deepfake Detectors](#video--deepfake-detectors)
  - [Audio & Voice Clone Detectors](#audio--voice-clone-detectors)
  - [Watermarking & Provenance](#watermarking--provenance)
  - [Datasets & Benchmarks](#datasets--benchmarks)
  - [Related Awesome Lists](#related-awesome-lists)
  - [Contributing](#contributing)

## Multimodal Platforms & APIs
| Icon | Name | Description | Repos |
|------|------|-------------|-------|
| <img src="https://www.google.com/s2/favicons?domain=realitydefender.com&sz=64" width="30" height="30"> | [Reality Defender](https://www.realitydefender.com) | Enterprise deepfake detection for image, video, audio and text, with SDKs and a free tier API. | ![GitHub Repo stars](https://img.shields.io/github/stars/Reality-Defender/realitydefender-sdk-python) |
| <img src="https://www.google.com/s2/favicons?domain=thehive.ai&sz=64" width="30" height="30"> | [Hive AI-Generated Content Detection](https://thehive.ai/apis/ai-generated-content-classification) | Content moderation API that flags AI-generated images, video and audio and attributes the likely source model. | - |
| <img src="https://www.google.com/s2/favicons?domain=sightengine.com&sz=64" width="30" height="30"> | [Sightengine](https://sightengine.com/detect-ai-generated-images) | Moderation API with AI-generated image/video and deepfake face detection. | ![GitHub Repo stars](https://img.shields.io/github/stars/Sightengine/client-python) |
| <img src="https://www.google.com/s2/favicons?domain=aiornot.com&sz=64" width="30" height="30"> | [AI or Not](https://www.aiornot.com) | Web app and API that checks whether images, video and audio were created by AI. | - |
| <img src="https://www.google.com/s2/favicons?domain=sensity.ai&sz=64" width="30" height="30"> | [Sensity AI](https://sensity.ai) | Deepfake and synthetic media detection platform for faces, video, images and voice, used in KYC and investigations. | - |
| <img src="https://www.google.com/s2/favicons?domain=truemedia.org&sz=64" width="30" height="30"> | [TrueMedia.org](https://www.truemedia.org) | Non-profit deepfake detector for political media (image, video, audio). Shut down in 2025 and open-sourced its models. | ![GitHub Repo stars](https://img.shields.io/github/stars/truemediaorg/ml-models) |
| <img src="https://www.google.com/s2/favicons?domain=buffalo.edu&sz=64" width="30" height="30"> | [DeepFake-O-Meter](https://zinc.cse.buffalo.edu/ubmdfl/deep-o-meter/) | University at Buffalo's open platform that runs many academic detectors on images, video and audio. | ![GitHub Repo stars](https://img.shields.io/github/stars/yuezunli/deepfake-o-meter) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [DeepSafe](https://github.com/siddharthksah/DeepSafe) | Open-source, self-hostable deepfake detection platform that bundles multiple detectors behind one UI. | ![GitHub Repo stars](https://img.shields.io/github/stars/siddharthksah/DeepSafe) |

## Image Detectors
| Icon | Name | Description | Repos |
|------|------|-------------|-------|
| <img src="https://www.google.com/s2/favicons?domain=illuminarty.ai&sz=64" width="30" height="30"> | [Illuminarty](https://illuminarty.ai) | Detects AI-generated images, localizes manipulated regions and guesses the generating model. | - |
| <img src="https://www.google.com/s2/favicons?domain=isitai.com&sz=64" width="30" height="30"> | [Is It AI?](https://isitai.com) | Free online checker for AI-generated images, with an API. | - |
| <img src="https://www.google.com/s2/favicons?domain=deepmind.google&sz=64" width="30" height="30"> | [SynthID Detector](https://deepmind.google/science/synthid/) | Google DeepMind portal that detects SynthID watermarks in images, video, audio and text made with Google models. | ![GitHub Repo stars](https://img.shields.io/github/stars/google-deepmind/synthid-text) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [CNNDetection](https://github.com/PeterWang512/CNNDetection) | Classic baseline showing CNN-generated images are "surprisingly easy to spot" (CVPR 2020). | ![GitHub Repo stars](https://img.shields.io/github/stars/PeterWang512/CNNDetection) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [UniversalFakeDetect](https://github.com/WisconsinAIVision/UniversalFakeDetect) | Generalizable fake-image detection using CLIP feature space (CVPR 2023). | ![GitHub Repo stars](https://img.shields.io/github/stars/WisconsinAIVision/UniversalFakeDetect) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [DIRE](https://github.com/ZhendongWang6/DIRE) | Detects diffusion-generated images via DIffusion Reconstruction Error (ICCV 2023). | ![GitHub Repo stars](https://img.shields.io/github/stars/ZhendongWang6/DIRE) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [AIDE](https://github.com/shilinyan99/AIDE) | "A Sanity Check for AI-generated Image Detection" — hybrid low/high-level feature detector and Chameleon dataset (ICLR 2025). | ![GitHub Repo stars](https://img.shields.io/github/stars/shilinyan99/AIDE) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [NPR](https://github.com/chuangchuangtan/NPR-DeepfakeDetection) | Neighboring Pixel Relationships for generalizable detection of upsampling artifacts (CVPR 2024). | ![GitHub Repo stars](https://img.shields.io/github/stars/chuangchuangtan/NPR-DeepfakeDetection) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [DMimageDetection](https://github.com/grip-unina/DMimageDetection) | GRIP-UNINA detector for synthetic images generated by diffusion models. | ![GitHub Repo stars](https://img.shields.io/github/stars/grip-unina/DMimageDetection) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [ClipBased-SyntheticImageDetection](https://github.com/grip-unina/ClipBased-SyntheticImageDetection) | Few-shot CLIP-based synthetic image detection that generalizes across generators (CVPR-W 2024). | ![GitHub Repo stars](https://img.shields.io/github/stars/grip-unina/ClipBased-SyntheticImageDetection) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [GAN-image-detection](https://github.com/polimi-ispl/GAN-image-detection) | Politecnico di Milano ensemble detector for GAN-generated images. | ![GitHub Repo stars](https://img.shields.io/github/stars/polimi-ispl/GAN-image-detection) |

## Video & Deepfake Detectors
| Icon | Name | Description | Repos |
|------|------|-------------|-------|
| <img src="https://www.google.com/s2/favicons?domain=intel.com&sz=64" width="30" height="30"> | [Intel FakeCatcher](https://www.intel.com/content/www/us/en/research/trusted-media-deepfake-detection.html) | Real-time deepfake video detection based on photoplethysmography (blood-flow) signals in faces. | - |
| <img src="https://www.google.com/s2/favicons?domain=deepware.ai&sz=64" width="30" height="30"> | [Deepware Scanner](https://deepware.ai) | Free online scanner for deepfake videos. | - |
| <img src="https://www.google.com/s2/favicons?domain=mcafee.com&sz=64" width="30" height="30"> | [McAfee Deepfake Detector](https://www.mcafee.com/en-us/ai/deepfake-detector.html) | On-device detector that alerts on AI-generated audio in videos you watch. | - |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [DeepfakeBench](https://github.com/SCLBD/DeepfakeBench) | Unified benchmark and codebase with 30+ image/video deepfake detectors and standardized training/eval (NeurIPS 2023). | ![GitHub Repo stars](https://img.shields.io/github/stars/SCLBD/DeepfakeBench) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [DFDC Winning Solution](https://github.com/selimsef/dfdc_deepfake_challenge) | First-place solution of the Facebook Deepfake Detection Challenge (EfficientNet ensemble). | ![GitHub Repo stars](https://img.shields.io/github/stars/selimsef/dfdc_deepfake_challenge) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [ICPR2020 DFDC](https://github.com/polimi-ispl/icpr2020dfdc) | Video face manipulation detection through ensemble of CNNs with attention. | ![GitHub Repo stars](https://img.shields.io/github/stars/polimi-ispl/icpr2020dfdc) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [LipForensics](https://github.com/ahaliassos/LipForensics) | Generalizable face forgery detection using lip-movement irregularities (CVPR 2021). | ![GitHub Repo stars](https://img.shields.io/github/stars/ahaliassos/LipForensics) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [GenConViT](https://github.com/erprogs/GenConViT) | Deepfake video detection using a Generative Convolutional Vision Transformer. | ![GitHub Repo stars](https://img.shields.io/github/stars/erprogs/GenConViT) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [MesoNet](https://github.com/DariusAf/MesoNet) | Compact network for facial video forgery detection (Deepfake, Face2Face). | ![GitHub Repo stars](https://img.shields.io/github/stars/DariusAf/MesoNet) |

## Audio & Voice Clone Detectors
| Icon | Name | Description | Repos |
|------|------|-------------|-------|
| <img src="https://www.google.com/s2/favicons?domain=resemble.ai&sz=64" width="30" height="30"> | [Resemble Detect](https://www.resemble.ai/detect/) | Real-time deepfake audio detection API for voice, calls and media. | - |
| <img src="https://www.google.com/s2/favicons?domain=elevenlabs.io&sz=64" width="30" height="30"> | [ElevenLabs AI Speech Classifier](https://elevenlabs.io/ai-speech-classifier) | Checks whether an audio clip was generated with ElevenLabs. | - |
| <img src="https://www.google.com/s2/favicons?domain=pindrop.com&sz=64" width="30" height="30"> | [Pindrop Pulse](https://www.pindrop.com/products/pindrop-pulse/) | Deepfake voice detection for call centers and media verification. | - |
| <img src="https://www.google.com/s2/favicons?domain=hiya.com&sz=64" width="30" height="30"> | [Hiya Deepfake Voice Detector](https://www.hiya.com/products/deepfake-voice-detector) | Free Chrome extension that flags AI-generated voices in online audio and video. | - |
| <img src="https://www.google.com/s2/favicons?domain=deepfake-total.com&sz=64" width="30" height="30"> | [Deepfake Total](https://deepfake-total.com) | Fraunhofer AISEC's free platform for checking audio files and YouTube links for audio deepfakes. | - |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [AASIST](https://github.com/clovaai/aasist) | Audio anti-spoofing with integrated spectro-temporal graph attention networks (ICASSP 2022). | ![GitHub Repo stars](https://img.shields.io/github/stars/clovaai/aasist) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [SSL Anti-spoofing](https://github.com/TakHemlata/SSL_Anti-spoofing) | wav2vec 2.0 + AASIST spoofing and deepfake speech detection. | ![GitHub Repo stars](https://img.shields.io/github/stars/TakHemlata/SSL_Anti-spoofing) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [RawGAT-ST](https://github.com/eurecom-asp/RawGAT-ST-antispoofing) | End-to-end spectro-temporal graph attention networks for speaker verification anti-spoofing. | ![GitHub Repo stars](https://img.shields.io/github/stars/eurecom-asp/RawGAT-ST-antispoofing) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [Whisper Features DeepFake Detection](https://github.com/piotrkawa/deepfake-whisper-features) | Improved audio deepfake detection using Whisper encoder features. | ![GitHub Repo stars](https://img.shields.io/github/stars/piotrkawa/deepfake-whisper-features) |
| <img src="https://www.google.com/s2/favicons?domain=asvspoof.org&sz=64" width="30" height="30"> | [ASVspoof Baselines](https://github.com/asvspoof-challenge/2021) | Official baseline systems (LFCC-GMM, RawNet2, etc.) for the ASVspoof 2021 challenge. | ![GitHub Repo stars](https://img.shields.io/github/stars/asvspoof-challenge/2021) |

## Watermarking & Provenance
| Icon | Name | Description | Repos |
|------|------|-------------|-------|
| <img src="https://www.google.com/s2/favicons?domain=contentcredentials.org&sz=64" width="30" height="30"> | [Content Credentials Verify](https://contentcredentials.org/verify) | Inspect C2PA Content Credentials (signed provenance metadata) attached to images, video and audio. | ![GitHub Repo stars](https://img.shields.io/github/stars/contentauth/c2pa-rs) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [c2pa-js](https://github.com/contentauth/c2pa-js) | JavaScript SDK for reading and verifying C2PA manifests in the browser. | ![GitHub Repo stars](https://img.shields.io/github/stars/contentauth/c2pa-js) |
| <img src="https://www.google.com/s2/favicons?domain=adobe.com&sz=64" width="30" height="30"> | [TrustMark](https://github.com/adobe/trustmark) | Adobe's open universal watermarking for arbitrary-resolution images, compatible with C2PA. | ![GitHub Repo stars](https://img.shields.io/github/stars/adobe/trustmark) |
| <img src="https://www.google.com/s2/favicons?domain=meta.com&sz=64" width="30" height="30"> | [Video Seal](https://github.com/facebookresearch/videoseal) | Meta's open and efficient watermarking and detection for video and images. | ![GitHub Repo stars](https://img.shields.io/github/stars/facebookresearch/videoseal) |
| <img src="https://www.google.com/s2/favicons?domain=meta.com&sz=64" width="30" height="30"> | [AudioSeal](https://github.com/facebookresearch/audioseal) | Meta's localized watermarking for AI-generated speech with a very fast detector. | ![GitHub Repo stars](https://img.shields.io/github/stars/facebookresearch/audioseal) |
| <img src="https://www.google.com/s2/favicons?domain=meta.com&sz=64" width="30" height="30"> | [Stable Signature](https://github.com/facebookresearch/stable_signature) | Roots watermarks into latent diffusion model decoders so every generated image is detectable. | ![GitHub Repo stars](https://img.shields.io/github/stars/facebookresearch/stable_signature) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [invisible-watermark](https://github.com/ShieldMnt/invisible-watermark) | Python library for blind invisible image watermarks, used by Stable Diffusion releases. | ![GitHub Repo stars](https://img.shields.io/github/stars/ShieldMnt/invisible-watermark) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [WavMark](https://github.com/wavmark/wavmark) | AI-based audio watermarking and detection tool. | ![GitHub Repo stars](https://img.shields.io/github/stars/wavmark/wavmark) |

## Datasets & Benchmarks
| Icon | Name | Description | Repos |
|------|------|-------------|-------|
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [FaceForensics++](https://github.com/ondyari/FaceForensics) | Widely used benchmark of manipulated facial videos (Deepfakes, Face2Face, FaceSwap, NeuralTextures). | ![GitHub Repo stars](https://img.shields.io/github/stars/ondyari/FaceForensics) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [Celeb-DF](https://github.com/yuezunli/celeb-deepfakeforensics) | Large-scale, challenging celebrity deepfake video dataset. | ![GitHub Repo stars](https://img.shields.io/github/stars/yuezunli/celeb-deepfakeforensics) |
| <img src="https://www.google.com/s2/favicons?domain=kaggle.com&sz=64" width="30" height="30"> | [DFDC](https://www.kaggle.com/c/deepfake-detection-challenge) | Deepfake Detection Challenge dataset with 100k+ videos from Meta, AWS and partners. | - |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [GenImage](https://github.com/GenImage-Dataset/GenImage) | Million-scale benchmark of images from Midjourney, Stable Diffusion, DALL·E, BigGAN and more. | ![GitHub Repo stars](https://img.shields.io/github/stars/GenImage-Dataset/GenImage) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [Deepfake-Eval-2024](https://github.com/nuriachandra/Deepfake-Eval-2024) | In-the-wild multimodal deepfake benchmark collected from social media and TrueMedia.org users. | ![GitHub Repo stars](https://img.shields.io/github/stars/nuriachandra/Deepfake-Eval-2024) |
| <img src="https://www.google.com/s2/favicons?domain=asvspoof.org&sz=64" width="30" height="30"> | [ASVspoof](https://www.asvspoof.org) | The standard challenge series and datasets for spoofed and deepfake speech detection. | - |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [WaveFake](https://github.com/RUB-SysSec/WaveFake) | Dataset of audio generated by multiple neural vocoders for audio deepfake detection. | ![GitHub Repo stars](https://img.shields.io/github/stars/RUB-SysSec/WaveFake) |

## Related Awesome Lists
| Icon | Name | Description | Repos |
|------|------|-------------|-------|
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [Awesome Deepfakes Detection](https://github.com/Daisy-Zhang/Awesome-Deepfakes-Detection) | Tools, papers and code related to deepfake detection. | ![GitHub Repo stars](https://img.shields.io/github/stars/Daisy-Zhang/Awesome-Deepfakes-Detection) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [Awesome Deepfakes](https://github.com/aerophile/awesome-deepfakes) | Everything deepfakes: creation, detection and resources. | ![GitHub Repo stars](https://img.shields.io/github/stars/aerophile/awesome-deepfakes) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [Audio Deepfake Detection](https://github.com/media-sec-lab/Audio-Deepfake-Detection) | Research progress, datasets and papers on speech deepfake detection. | ![GitHub Repo stars](https://img.shields.io/github/stars/media-sec-lab/Audio-Deepfake-Detection) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [Awesome AI](https://github.com/openbestof/awesome-ai) | A curated list of awesome AI tools, frameworks, APIs, software and resources. | ![GitHub Repo stars](https://img.shields.io/github/stars/openbestof/awesome-ai) |

## Contributing
Contributions are welcome! Open a pull request adding a row to the relevant table using the format:

```markdown
| <img src="https://www.google.com/s2/favicons?domain=example.com&sz=64" width="30" height="30"> | [Name](https://link) | Short description of what it detects and how. | ![GitHub Repo stars](https://img.shields.io/github/stars/owner/repo) |
```

Use `-` in the Repos column for closed-source tools. Please only add tools that are publicly available and actively focused on detecting AI-generated image, video or audio content.

## License
[MIT](LICENSE) © Really Human Labs

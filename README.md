# Awesome AI Content Detectors

Not sure if that photo, video or voice note is real? This is our running list of tools that can help you find out. You'll find detectors for AI-generated **images**, **video** and **audio**, along with the watermarking tools, datasets and other lists we've found useful along the way.

> A quick word of caution: no detector gets it right every time. They struggle with brand-new generators, and compression or light editing can throw them off. Think of a score as a clue, not a verdict. You'll get the best results by checking a few detectors, looking for provenance data, and using your own judgment.

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
Tools that check more than one kind of media. These are a good place to start if you need to check images, video and audio in one place.

| Icon | Name | Description | Repos |
|------|------|-------------|-------|
| <img src="https://www.google.com/s2/favicons?domain=realitydefender.com&sz=64" width="30" height="30"> | [Reality Defender](https://www.realitydefender.com) | Checks images, video, audio and text for deepfakes. Built for businesses, but there's a free API tier and SDKs to get going quickly. | ![GitHub Repo stars](https://img.shields.io/github/stars/Reality-Defender/realitydefender-sdk-python) |
| <img src="https://www.google.com/s2/favicons?domain=thehive.ai&sz=64" width="30" height="30"> | [Hive AI-Generated Content Detection](https://thehive.ai/apis/ai-generated-content-classification) | Flags AI-made images, video and audio, and will often tell you which model likely made them. | - |
| <img src="https://www.google.com/s2/favicons?domain=sightengine.com&sz=64" width="30" height="30"> | [Sightengine](https://sightengine.com/detect-ai-generated-images) | A moderation API that spots AI-generated images and video, plus deepfaked faces. | ![GitHub Repo stars](https://img.shields.io/github/stars/Sightengine/client-python) |
| <img src="https://www.google.com/s2/favicons?domain=aiornot.com&sz=64" width="30" height="30"> | [AI or Not](https://www.aiornot.com) | Exactly what it sounds like: upload an image, video or audio clip and it tells you whether AI made it. Comes with an API too. | - |
| <img src="https://www.google.com/s2/favicons?domain=sensity.ai&sz=64" width="30" height="30"> | [Sensity AI](https://sensity.ai) | Catches deepfaked faces, video, images and voices. Popular for identity checks and investigations. | - |
| <img src="https://www.google.com/s2/favicons?domain=truemedia.org&sz=64" width="30" height="30"> | [TrueMedia.org](https://www.truemedia.org) | A non-profit that checked political media for deepfakes. It shut down in 2025, but its models are open source, so you can still use them. | ![GitHub Repo stars](https://img.shields.io/github/stars/truemediaorg/ml-models) |
| <img src="https://www.google.com/s2/favicons?domain=buffalo.edu&sz=64" width="30" height="30"> | [DeepFake-O-Meter](https://zinc.cse.buffalo.edu/ubmdfl/deep-o-meter/) | From the University at Buffalo. Upload a file and it runs a bunch of research detectors on it at once. | ![GitHub Repo stars](https://img.shields.io/github/stars/yuezunli/deepfake-o-meter) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [DeepSafe](https://github.com/siddharthksah/DeepSafe) | An open-source platform you can host yourself. It puts several detectors behind one simple interface. | ![GitHub Repo stars](https://img.shields.io/github/stars/siddharthksah/DeepSafe) |

## Image Detectors
For still images. The first few are ready-to-use web tools. The rest are research models you can run yourself.

| Icon | Name | Description | Repos |
|------|------|-------------|-------|
| <img src="https://www.google.com/s2/favicons?domain=illuminarty.ai&sz=64" width="30" height="30"> | [Illuminarty](https://illuminarty.ai) | Tells you if an image is AI-made, highlights which parts look edited, and guesses which model made it. | - |
| <img src="https://www.google.com/s2/favicons?domain=isitai.com&sz=64" width="30" height="30"> | [Is It AI?](https://isitai.com) | A free, no-fuss image checker. There's an API if you need one. | - |
| <img src="https://www.google.com/s2/favicons?domain=deepmind.google&sz=64" width="30" height="30"> | [SynthID Detector](https://deepmind.google/science/synthid/) | Google's tool for finding the invisible SynthID watermark that Google's own AI models add to images, video, audio and text. | ![GitHub Repo stars](https://img.shields.io/github/stars/google-deepmind/synthid-text) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [CNNDetection](https://github.com/PeterWang512/CNNDetection) | The classic starting point. This 2020 paper showed that AI-generated images are surprisingly easy to spot, at least for now. | ![GitHub Repo stars](https://img.shields.io/github/stars/PeterWang512/CNNDetection) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [UniversalFakeDetect](https://github.com/WisconsinAIVision/UniversalFakeDetect) | Uses CLIP to spot fakes, so it holds up better on generators it was never trained on. | ![GitHub Repo stars](https://img.shields.io/github/stars/WisconsinAIVision/UniversalFakeDetect) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [DIRE](https://github.com/ZhendongWang6/DIRE) | Catches diffusion-model images by checking how easily a diffusion model can rebuild them. The repo is archived, but the idea is still widely cited. | ![GitHub Repo stars](https://img.shields.io/github/stars/ZhendongWang6/DIRE) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [AIDE](https://github.com/shilinyan99/AIDE) | A reality check for image detectors. It comes with a tough new test set (Chameleon) and a detector that looks at both fine details and overall content. | ![GitHub Repo stars](https://img.shields.io/github/stars/shilinyan99/AIDE) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [NPR](https://github.com/chuangchuangtan/NPR-DeepfakeDetection) | Picks up the tiny pixel patterns that upscaling leaves behind, which almost every image generator does. | ![GitHub Repo stars](https://img.shields.io/github/stars/chuangchuangtan/NPR-DeepfakeDetection) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [DMimageDetection](https://github.com/grip-unina/DMimageDetection) | A detector from the GRIP lab in Naples, built to catch images made by diffusion models. | ![GitHub Repo stars](https://img.shields.io/github/stars/grip-unina/DMimageDetection) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [ClipBased-SyntheticImageDetection](https://github.com/grip-unina/ClipBased-SyntheticImageDetection) | Another one from GRIP. It needs only a few examples to learn and works across many different generators. | ![GitHub Repo stars](https://img.shields.io/github/stars/grip-unina/ClipBased-SyntheticImageDetection) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [GAN-image-detection](https://github.com/polimi-ispl/GAN-image-detection) | A group of models from Politecnico di Milano that work together to catch GAN-made images. | ![GitHub Repo stars](https://img.shields.io/github/stars/polimi-ispl/GAN-image-detection) |

## Video & Deepfake Detectors
For face swaps, lip-syncs and other doctored video.

| Icon | Name | Description | Repos |
|------|------|-------------|-------|
| <img src="https://www.google.com/s2/favicons?domain=intel.com&sz=64" width="30" height="30"> | [Intel FakeCatcher](https://www.intel.com/content/www/us/en/research/trusted-media-deepfake-detection.html) | A clever trick: real faces show faint color changes as blood flows under the skin, and deepfakes usually don't. Works in real time. | - |
| <img src="https://www.google.com/s2/favicons?domain=deepware.ai&sz=64" width="30" height="30"> | [Deepware Scanner](https://deepware.ai) | Paste in a link or upload a video and it'll scan it for deepfakes for free. | - |
| <img src="https://www.google.com/s2/favicons?domain=mcafee.com&sz=64" width="30" height="30"> | [McAfee Deepfake Detector](https://www.mcafee.com/en-us/ai/deepfake-detector.html) | Runs on your computer and warns you when a video you're watching has AI-generated audio. | - |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [DeepfakeBench](https://github.com/SCLBD/DeepfakeBench) | Over 30 deepfake detectors in one codebase, all trained and tested the same way, so it's easy to compare them fairly. | ![GitHub Repo stars](https://img.shields.io/github/stars/SCLBD/DeepfakeBench) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [DFDC Winning Solution](https://github.com/selimsef/dfdc_deepfake_challenge) | The approach that won Facebook's big Deepfake Detection Challenge. | ![GitHub Repo stars](https://img.shields.io/github/stars/selimsef/dfdc_deepfake_challenge) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [ICPR2020 DFDC](https://github.com/polimi-ispl/icpr2020dfdc) | Several models working together, each trained to focus on the parts of a face most likely to give a fake away. | ![GitHub Repo stars](https://img.shields.io/github/stars/polimi-ispl/icpr2020dfdc) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [LipForensics](https://github.com/ahaliassos/LipForensics) | Watches the lips. Deepfakes often get mouth movements subtly wrong. | ![GitHub Repo stars](https://img.shields.io/github/stars/ahaliassos/LipForensics) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [GenConViT](https://github.com/erprogs/GenConViT) | Combines a few kinds of models to spot deepfake videos, including ones it hasn't seen before. | ![GitHub Repo stars](https://img.shields.io/github/stars/erprogs/GenConViT) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [MesoNet](https://github.com/DariusAf/MesoNet) | A small, fast model from 2018 for spotting face swaps. Simple, but still a handy baseline. | ![GitHub Repo stars](https://img.shields.io/github/stars/DariusAf/MesoNet) |

## Audio & Voice Clone Detectors
For cloned voices, fake calls and synthetic speech.

| Icon | Name | Description | Repos |
|------|------|-------------|-------|
| <img src="https://www.google.com/s2/favicons?domain=resemble.ai&sz=64" width="30" height="30"> | [Resemble Detect](https://www.resemble.ai/detect/) | Listens for fake voices in real time, on calls, recordings or any other media. | - |
| <img src="https://www.google.com/s2/favicons?domain=elevenlabs.io&sz=64" width="30" height="30"> | [ElevenLabs AI Speech Classifier](https://elevenlabs.io/ai-speech-classifier) | Upload a clip and ElevenLabs will tell you if it was made with their tools. | - |
| <img src="https://www.google.com/s2/favicons?domain=pindrop.com&sz=64" width="30" height="30"> | [Pindrop Pulse](https://www.pindrop.com/products/pindrop-pulse/) | Helps call centers and newsrooms catch cloned voices before they cause damage. | - |
| <img src="https://www.google.com/s2/favicons?domain=hiya.com&sz=64" width="30" height="30"> | [Hiya Deepfake Voice Detector](https://www.hiya.com/products/deepfake-voice-detector) | A free Chrome extension that warns you when a voice in a video or clip sounds AI-made. | - |
| <img src="https://www.google.com/s2/favicons?domain=deepfake-total.com&sz=64" width="30" height="30"> | [Deepfake Total](https://deepfake-total.com) | A free tool from Fraunhofer AISEC. Drop in an audio file or YouTube link and it checks for fake audio. | - |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [AASIST](https://github.com/clovaai/aasist) | A go-to research model for catching spoofed speech. It looks at both pitch and timing. | ![GitHub Repo stars](https://img.shields.io/github/stars/clovaai/aasist) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [SSL Anti-spoofing](https://github.com/TakHemlata/SSL_Anti-spoofing) | Puts AASIST on top of the wav2vec 2.0 speech model for stronger results. | ![GitHub Repo stars](https://img.shields.io/github/stars/TakHemlata/SSL_Anti-spoofing) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [RawGAT-ST](https://github.com/eurecom-asp/RawGAT-ST-antispoofing) | Works straight from the raw audio to catch voices faked to fool speaker verification. | ![GitHub Repo stars](https://img.shields.io/github/stars/eurecom-asp/RawGAT-ST-antispoofing) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [Whisper Features DeepFake Detection](https://github.com/piotrkawa/deepfake-whisper-features) | Borrows what OpenAI's Whisper has learned about speech to get better at spotting fake audio. | ![GitHub Repo stars](https://img.shields.io/github/stars/piotrkawa/deepfake-whisper-features) |
| <img src="https://www.google.com/s2/favicons?domain=asvspoof.org&sz=64" width="30" height="30"> | [ASVspoof Baselines](https://github.com/asvspoof-challenge/2021) | The official starter models from the ASVspoof 2021 challenge. A good first benchmark. | ![GitHub Repo stars](https://img.shields.io/github/stars/asvspoof-challenge/2021) |

## Watermarking & Provenance
Instead of guessing after the fact, these tools label or sign content when it's created, so you can check later where it came from.

| Icon | Name | Description | Repos |
|------|------|-------------|-------|
| <img src="https://www.google.com/s2/favicons?domain=contentcredentials.org&sz=64" width="30" height="30"> | [Content Credentials Verify](https://contentcredentials.org/verify) | Drop in a file to see its Content Credentials (C2PA): signed info about who made it and how it was edited. | ![GitHub Repo stars](https://img.shields.io/github/stars/contentauth/c2pa-rs) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [c2pa-js](https://github.com/contentauth/c2pa-js) | Read and check Content Credentials right in the browser. | ![GitHub Repo stars](https://img.shields.io/github/stars/contentauth/c2pa-js) |
| <img src="https://www.google.com/s2/favicons?domain=adobe.com&sz=64" width="30" height="30"> | [TrustMark](https://github.com/adobe/trustmark) | Adobe's open-source invisible watermark. Works on images of any size and plays nicely with C2PA. | ![GitHub Repo stars](https://img.shields.io/github/stars/adobe/trustmark) |
| <img src="https://www.google.com/s2/favicons?domain=meta.com&sz=64" width="30" height="30"> | [Video Seal](https://github.com/facebookresearch/videoseal) | Meta's open-source tool for adding and detecting watermarks in video and images. | ![GitHub Repo stars](https://img.shields.io/github/stars/facebookresearch/videoseal) |
| <img src="https://www.google.com/s2/favicons?domain=meta.com&sz=64" width="30" height="30"> | [AudioSeal](https://github.com/facebookresearch/audioseal) | Meta's watermark for AI speech. It can point to the exact part of a clip that's watermarked, and the detector is very fast. | ![GitHub Repo stars](https://img.shields.io/github/stars/facebookresearch/audioseal) |
| <img src="https://www.google.com/s2/favicons?domain=meta.com&sz=64" width="30" height="30"> | [Stable Signature](https://github.com/facebookresearch/stable_signature) | Builds a watermark into the image generator itself, so every image it makes carries one. | ![GitHub Repo stars](https://img.shields.io/github/stars/facebookresearch/stable_signature) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [invisible-watermark](https://github.com/ShieldMnt/invisible-watermark) | A simple Python library for hiding watermarks in images. Stable Diffusion has used it. | ![GitHub Repo stars](https://img.shields.io/github/stars/ShieldMnt/invisible-watermark) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [WavMark](https://github.com/wavmark/wavmark) | Hides a watermark in audio, and finds it again later. | ![GitHub Repo stars](https://img.shields.io/github/stars/wavmark/wavmark) |

## Datasets & Benchmarks
Want to train your own detector, or see how well an existing one really works? Start here.

| Icon | Name | Description | Repos |
|------|------|-------------|-------|
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [FaceForensics++](https://github.com/ondyari/FaceForensics) | The dataset almost everyone tests on: thousands of videos edited with four popular face-swap and face-edit methods. | ![GitHub Repo stars](https://img.shields.io/github/stars/ondyari/FaceForensics) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [Celeb-DF](https://github.com/yuezunli/celeb-deepfakeforensics) | High-quality celebrity deepfakes that are much harder to catch than older datasets. | ![GitHub Repo stars](https://img.shields.io/github/stars/yuezunli/celeb-deepfakeforensics) |
| <img src="https://www.google.com/s2/favicons?domain=kaggle.com&sz=64" width="30" height="30"> | [DFDC](https://www.kaggle.com/c/deepfake-detection-challenge) | More than 100,000 videos from the Deepfake Detection Challenge run by Meta, AWS and others. | - |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [GenImage](https://github.com/GenImage-Dataset/GenImage) | Over a million images from Midjourney, Stable Diffusion, DALL·E, BigGAN and more. | ![GitHub Repo stars](https://img.shields.io/github/stars/GenImage-Dataset/GenImage) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [Deepfake-Eval-2024](https://github.com/nuriachandra/Deepfake-Eval-2024) | Real deepfakes collected from social media and TrueMedia.org users, not made in a lab. A good test of how detectors hold up out there. | ![GitHub Repo stars](https://img.shields.io/github/stars/nuriachandra/Deepfake-Eval-2024) |
| <img src="https://www.google.com/s2/favicons?domain=asvspoof.org&sz=64" width="30" height="30"> | [ASVspoof](https://www.asvspoof.org) | The long-running challenge, and dataset, for catching fake and spoofed speech. | - |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [WaveFake](https://github.com/RUB-SysSec/WaveFake) | Fake audio made with many different speech generators, all in one place. | ![GitHub Repo stars](https://img.shields.io/github/stars/RUB-SysSec/WaveFake) |

## Related Awesome Lists
Other lists worth bookmarking.

| Icon | Name | Description | Repos |
|------|------|-------------|-------|
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [Awesome Deepfakes Detection](https://github.com/Daisy-Zhang/Awesome-Deepfakes-Detection) | A big collection of deepfake detection papers, code and tools. | ![GitHub Repo stars](https://img.shields.io/github/stars/Daisy-Zhang/Awesome-Deepfakes-Detection) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [Awesome Deepfakes](https://github.com/aerophile/awesome-deepfakes) | Everything deepfakes: how they're made, how they're caught, and more. | ![GitHub Repo stars](https://img.shields.io/github/stars/aerophile/awesome-deepfakes) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [Audio Deepfake Detection](https://github.com/media-sec-lab/Audio-Deepfake-Detection) | Keeps up with the latest research, datasets and papers on fake speech. | ![GitHub Repo stars](https://img.shields.io/github/stars/media-sec-lab/Audio-Deepfake-Detection) |
| <img src="https://www.google.com/s2/favicons?domain=github.com&sz=64" width="30" height="30"> | [Awesome AI](https://github.com/openbestof/awesome-ai) | A broader list of AI tools, frameworks, APIs and resources. | ![GitHub Repo stars](https://img.shields.io/github/stars/openbestof/awesome-ai) |

## Contributing
Know a tool we missed? We'd love to hear about it. Open a pull request and add a row to the right table, like this:

```markdown
| <img src="https://www.google.com/s2/favicons?domain=example.com&sz=64" width="30" height="30"> | [Name](https://link) | A sentence or two on what it catches and how. | ![GitHub Repo stars](https://img.shields.io/github/stars/owner/repo) |
```

If the tool isn't open source, just put `-` in the Repos column. We only list tools that anyone can use and that focus on spotting AI-generated images, video or audio.

## License
[MIT](LICENSE) © Really Human Labs

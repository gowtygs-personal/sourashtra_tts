# 🗣️ Sourashtra TTS — Ground-Up Speech Synthesis for a Low-Resource Language

This repository aims to build a **Text-to-Speech (TTS)** system for the **Sourashtra language**, a lesser-resourced language spoken predominantly in Tamil Nadu, India, by a small migrant community.

## 🎯 Goal

To develop a high-quality **end-to-end TTS model** trained on my own voice data, while creating supporting tools like a **Grapheme-to-Phoneme (G2P)** mapping and lexicon from scratch. The entire stack is built with the intention of being **open-sourced** under a **Non-Commercial Non-Compete (NCNC)** license to preserve linguistic integrity and ensure ethical reuse.

---

## 🗃️ Dataset

| Element         | Details |
|----------------|---------|
| **Voice**       | Native Sourashtra speaker (myself) |
| **Recording**   | One audio clip per day |
| **Transcription** | Manually transcribed per clip (with phoneme mapping planned) |
| **Format**      | `.wav` audio, `.txt` transcript (aligned manually) |
| **Mic Setup**   | USB Dynamic Mic with light filtering via Audacity |

> ⚠️ Fan/AC might be on during recordings — environmental filtering strategies like noise reduction and HPF applied.

---

## 🧠 Phoneme / G2P Mapping

Sourashtra is often written in **English or Tamil scripts** as its native script is not widely known or used. So this project transcript will also be using English Script.

Known Issues:
- Variability in spellings (e.g., *yen*, *yaen*, *en*),
- Inconsistent pronunciation cues from English orthography,
- Lack of standard G2P rules or phoneme sets,

---

## 🔍 Model Choices Explored

After early exploration, the following models were shortlisted:

### ✅ **[XTTS by Coqui](https://github.com/coqui-ai/TTS)**  
- Pros: Multi-speaker, multilingual, good voice cloning
- Plan: Use for inference and testing G2P + audio quality early on

### ✅ **[Parler-TTS (AI4Bharat)](https://github.com/AI4Bharat/Parler-TTS)**  
- Pros: Specifically built for Indian languages, integrates well with Indic TTS pipeline
- Plan: Fine-tune with collected audio + transcripts

---

## 🧪 Current Status

- [x] Initial recordings started (daily, clean environment with basic filtering)
- [x] Transcription aligned manually
- [ ] Building initial G2P dictionary
- [ ] Evaluate phoneme coverage from Hindi/Tamil datasets
- [ ] Prepare data loader script for Tacotron2 / Parler-TTS
- [ ] Fine-tune and benchmark on small dataset

---

## 📜 Licensing

This project is licensed under **Non-Commercial, Non-Compete (NCNC)** license.  
This means:
- ✅ You can use, study, remix for personal or educational purposes.
- ❌ You cannot use it in commercial or proprietary applications.
- ❌ Derivatives must **not** compete directly with this project.

---

## 💡 Future Work

- Automate G2P using statistical or neural alignment tools
- Evaluate and train diffusion-based TTS models
- Build lightweight inference UI for community demo
- Publish findings and open-source tools — potential for IEEE / ACL / LREC-COLING level paper

---

## 🙋‍♂️ About Me

I’m a native Sourashtra speaker working in industry, building this project independently.  
The goal is to preserve the language and make its digital voice accessible to all.

If you're interested in collaborating (especially with experience in G2P, diffusion models, or linguistics), feel free to reach out or contribute via Issues and PRs!



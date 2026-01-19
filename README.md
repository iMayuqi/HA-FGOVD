# HA-FGOVD: Hierarchical Attribute-based Fine-Grained Open-Vocabulary Detection

This repository provides the **key implementation of our proposed HA-FGOVD method**, built on top of **GroundingDINO**.  
Due to licensing and maintenance considerations, **the official GroundingDINO codebase is NOT included** in this repository.

Pretrained model weights are released via **Hugging Face**.

---

## 📌 Overview

- **Base model**: GroundingDINO (official implementation)
- **Our contribution**: HA-FGOVD (Hierarchical Attribute-based Fine-Grained Open-Vocabulary Detection)
- **This repository contains**:
  - Core HA-FGOVD modules
  - Key modifications for fine-grained open-vocabulary detection
  - Integration logic with GroundingDINO
- **This repository does NOT contain**:
  - The full GroundingDINO source code
  - Pretrained GroundingDINO backbone weights

---

## 📥 Step 1: Download GroundingDINO (Official)

Please first clone the official GroundingDINO repository:

```bash
git clone https://github.com/IDEA-Research/GroundingDINO.git
cd GroundingDINO
```
Follow the official instructions to install dependencies and verify that the original GroundingDINO code runs correctly.

### ⚠️ Important:
Make sure the GroundingDINO codebase is correctly installed before integrating HA-FGOVD.

---

## 📂 Step 2: Integrate HA-FGOVD into GroundingDINO

This repository provides only the key code components of HA-FGOVD.
You need to manually place these files into the GroundingDINO directory.

File Placement Rule

All files in this repository should be copied into the GroundingDINO project while preserving the same directory hierarchy.

If a file already exists in the original GroundingDINO codebase, it should be replaced by the corresponding file from this repository.

## 📦 Step 3: Download Pretrained Weights

All pretrained weights for HA-FGOVD are hosted on Hugging Face:

### 🔗 Model weights
https://huggingface.co/maaaayq/HA-FGOVD/tree/main

Please download the required .pth files and place them in a checkpoint directory

## 🚀 Usage

After integrating the code and downloading the pretrained weights, you can run inference or evaluation following the standard GroundingDINO workflow with HA-FGOVD configurations.

## 📄 License

- GroundingDINO is released under its original license.

- The HA-FGOVD code provided in this repository is released for research use only.

## 📌 Citation

If you find this work useful, please consider citing our paper:

```bash
@article{xxx2025hafgovd,
  title={HA-FGOVD: Highlighting Fine-Grained Attributes via Explicit Linear Composition for Open-Vocabulary Object Detection},
  author={Yuqi Ma and Mengyin Liu and Chao Zhu and Xu{-}Cheng Yin},
  year={2025}，
  journal      = {{IEEE} Trans. Multim.},
}
```

## 🙏 Acknowledgement

This work is built upon the excellent GroundingDINO framework.
We sincerely thank the authors for making their code publicly available.

This repository contains the **official implementation** of the paper:

**Multifold Fusion Attention Variant for Emotion Recognition**  
🗓 Presented at the *2025 Conference on Computer Science and Software Engineering*  
📚 Published in *IEEE Xplore*  
🔗 [Read the Paper on IEEE Xplore](https://ieeexplore.ieee.org/document/11054013)

---

## Abstract

Multimodal emotion recognition has emerged as a critical challenge in affective computing, requiring the effective integration of diverse and asynchronous input sources. This paper introduces a **Multifold Fusion Attention Variant (MFAV)** that selectively emphasizes modality-specific and cross-modal features through a hierarchical fusion mechanism. MFAV employs a dual-stage attention pipeline, comprising intra-modality attention and cross-modality interaction to dynamically refine emotional cues from audio, video, and text. The proposed model achieves state-of-the-art performance on standard emotion recognition benchmarks and demonstrates strong generalization across variable emotion contexts.

---

## ✨ Key Features

- Modular architecture supporting visual, textual, and audio modalities
- Hierarchical attention mechanism for intra- and inter-modality fusion
- Lightweight design enabling faster inference without compromising accuracy
- Superior performance on emotion recognition benchmarks

---

## 🚀 Novelty and Contributions

- **Multifold Fusion Strategy**: Introduces a sequential attention fusion variant that models modality correlations more effectively than traditional parallel fusion.
- **Adaptive Attention Blocks**: Dynamically learn importance weights for each modality and their interactions.
- **Emotion-Specific Embedding Alignment**: Ensures semantic alignment of emotional cues across modalities to boost recognition robustness.

---

## 📚 Dataset Used

For this study, we utilized the dataset introduced in:

🔗 [PubMed: A Multimodal Dataset for Emotion Recognition from Naturalistic Interactions](https://pubmed.ncbi.nlm.nih.gov/39300129/)

This dataset contains synchronized **audio**, **video**, and **textual transcripts** of human interactions, annotated with categorical and dimensional emotion labels. Its diverse modalities and real-world complexity make it an ideal benchmark for evaluating multimodal emotion recognition systems.

Please refer to the dataset’s original source for licensing and access instructions.

---

## 📂 Directory Hierarchy

- `dataProcess/`
  - `audio.py` – Audio modality preprocessing
  - `EEG.py` – EEG modality preprocessing
  - `video.py` – Video modality preprocessing

- `models/`
  - `helpers.py` – Utility functions and helpers
  - `MFAV.py` – Core Multifold Fusion Attention Variant module
  - `model.py` – Full model construction and architecture

- `train.py` – Training script  
- `test.py` – Evaluation script  
- `LICENSE` – License file  
- `README.md` – Project documentation (this file)

---

## ⚙️ Requirements

- `Python ≥ 3.8`
- `PyTorch ≥ 1.12`
- `transformers` ≥ 4.30
- `networkx`
- `scikit-learn`
- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `opencv-python`
- `tqdm`

---

## 🏋️‍♀️ Training and Testing

After setting up the environment and preprocessing the dataset, you can proceed to train and evaluate the **Multifold Fusion Attention Variant (MFAV)** model.

### 🔁 Training

To train the model, simply run:

```bash
python train.py
```
- All training hyperparameters must be modified **directly inside** the `train.py` file:

  - Learning rate  
  - Batch size  
  - Number of epochs  
  - Enabled modalities  

- Ensure that:

  - Preprocessed dataset paths are set correctly  
  - Output directories exist or are auto-created in code  

- Model checkpoints and logs will be saved in folders like `checkpoints/` or `outputs/`.

### ✅ Testing

To evaluate the trained model, run:

```bash
python test.py
```

---

## 📝 License

This project is licensed under the **MIT License**.  
You are free to use, modify, and distribute this code for research and educational purposes.

---

## 📌 Citation

If you use this code or build upon our work, please cite the following:

**N. R. Yerragondu, C. Krishnan, J. Giddirappa and O. B. Indla**,  
"Multifold Fusion Attention Variant for Emotion Recognition,"  
*2025 International Conference on Computer Science and Software Engineering (CSASE)*,  
Duhok, Iraq, 2025, pp. 60–66,  
doi: [10.1109/CSASE63707.2025.11054013](https://ieeexplore.ieee.org/document/11054013)


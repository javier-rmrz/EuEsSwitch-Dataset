# EuEsSwitch-Dataset
**Spanish–Basque Code-Switching Speech Corpus**

## Description
EuEsSwitch-Dataset is a synthetic audio dataset designed for research in **automatic speech recognition (ASR)** with **code-switching** between **Spanish (Castilian)** and **Basque (Euskera)**.

The dataset includes both **monolingual segments** and **bilingual combinations**, enabling experimentation with:
- code-switching ASR
- language identification
- audio segmentation
- multilingual models

---

## Dataset Structure

The dataset is organized into the following folders:

### `plainEu`
- 50 audio segments generated in **Basque**
- Duration: **4–7 seconds**

### `plainEs`
- 50 audio segments generated in **Spanish**
- Duration: **4–7 seconds**

### `2secCombos`
- 2500 audio files
- Each audio combines **2 segments**
- The segments come from `plainEu` and `plainEs`
- They contain bilingual Basque–Spanish combinations

### `3secCombos`
- 1000 audio files
- Each audio combines **3 segments**
- The segments come from `plainEu` and `plainEs`
- It is guaranteed that:
  - not all segments are in the same language
  - the language pattern varies across files

### `4secCombos`
- 500 audio files
- Each audio combines **4 segments**
- The segments come from `plainEu` and `plainEs`
- It is guaranteed that:
  - not all segments are in the same language
  - the language pattern varies across files

---

## Purpose
This dataset was created to facilitate experiments in bilingual speech and code-switching, especially for Spanish–Basque ASR systems.

It can be used for:
- training and evaluation of ASR models with mixed languages
- automatic language identification in audio
- analysis of transitions between Basque and Spanish
- benchmarking multilingual models such as Whisper

---

## Composition Strategy
The dataset follows a progressively increasing complexity structure:

- **Base monolingual segments**: `plainEu`, `plainEs`
- **2-segment combinations**: simple scenarios
- **3-segment combinations**: greater variability
- **4-segment combinations**: more complex sequences

This makes it possible to analyze how models behave under different levels of code-switching.

---

## Notes
- This is a **synthetic dataset**, generated from audio segments.
- The combined audio files are built by concatenating segments.
- It is intended for research in multilingual speech processing.

---

## Author
**Javier Ramírez Zarzoso**  
GitHub: https://github.com/javier-rmrz

---

## Citation
If you use this dataset, please cite it as:

```bibtex
@dataset{ramirezzarzoso2026euesswitch,
  title     = {EuEsSwitch-Dataset: Spanish–Basque Code-Switching Speech Corpus},
  author    = {Javier Ramírez Zarzoso},
  year      = {2026}
}

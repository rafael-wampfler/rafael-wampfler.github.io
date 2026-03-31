---
title: Affective Computing & Emotion Recognition
date: 2019-01-01
weight: 20
tags:
  - Affective Computing
  - Emotion Recognition
  - Multimodal AI
  - Mobile Sensing
  - Deep Learning
summary: >
  Multimodal deep learning systems for affective state prediction from smartphone sensors, biometric data, egocentric vision, and physiological signals — enabling real-world ("in-the-wild") emotion and personality understanding.
---

## Overview

This research thread develops deep learning architectures for predicting human emotional and cognitive states from rich, naturalistic data streams. Unlike laboratory-controlled setups, our systems operate "in-the-wild" — on real devices, in real environments, with real users — addressing the full complexity of affective computing at scale.

## Motivation

Affective computing — the capacity of machines to detect, interpret, and respond to human emotions — is a foundational capability for human-centric AI. Yet most academic benchmarks rely on controlled, acted datasets that poorly predict real-world performance. Building systems that genuinely work in naturalistic settings requires confronting three fundamental challenges:

- **Domain adaptation**: Affective signals vary enormously across individuals and contexts; models must transfer gracefully.
- **Uncertainty estimation**: Emotion recognition inherently involves ambiguity and subjectivity; systems must quantify and communicate their confidence.
- **Scalability**: Continuous affective sensing must operate on resource-constrained mobile and edge devices.

## Approach

### Multimodal Fusion

Our work leverages a broad set of input modalities, combining them through transformer-based and convolutional architectures:

- **Smartphone touch and sensor data**: Stylus pressure, touch dynamics, accelerometer, and gyroscope signals during naturalistic task completion
- **Biometric data**: Heart rate, skin conductance, and other physiological signals from wearables
- **Egocentric vision**: First-person video from wearable cameras, capturing the user's visual environment
- **Typing behavior**: Smartphone keyboard dynamics as a passive indicator of affective and personality state

### Semi-Supervised and Self-Supervised Learning

Given the difficulty and cost of obtaining large labeled affective datasets in natural settings, we exploit semi-supervised learning strategies that leverage abundant unlabeled data. This improves generalization without requiring exhaustive annotation.

### egoEMOTION (NeurIPS 2025)

The most recent and ambitious contribution is *egoEMOTION*, presented at NeurIPS 2025 (Datasets and Benchmarks track). This work combines **egocentric vision** and **physiological signals** into a unified multimodal architecture, advancing both fusion strategies and providing a new reproducible benchmark dataset. egoEMOTION addresses the challenge of predicting emotion and personality from the wearer's own perspective, a naturalistic setting of growing relevance as wearable cameras become ubiquitous.

### Personality Recognition from Typing

Beyond momentary emotions, we have also developed systems for personality trait recognition from passive smartphone typing dynamics. This work (IEEE Transactions on Affective Computing, 2023) demonstrates that stable personality traits leave measurable signatures in everyday smartphone interactions, enabling passive, continuous personality inference.

## Key Results

- Demonstrated state-of-the-art in-the-wild affective state prediction from smartphone sensors across multiple CHI publications
- Published a new egocentric multimodal emotion and personality benchmark (NeurIPS 2025)
- Showed that semi-supervised learning substantially closes the gap between labeled and unlabeled-data performance
- Developed personality trait recognition from typing dynamics achieving strong classification performance on real-world data

## Publications

M. Jammot, B. Braun, P. Streli, **R. Wampfler** and C. Holz (2025). *egoEMOTION: Egocentric Vision and Physiological Signals for Emotion and Personality Recognition in Real-World Tasks*. In Conference on Neural Information Processing Systems 2025 (Datasets and Benchmarks, NeurIPS), pp. 1–12.

N. Kovačević, C. Holz, M. Gross and **R. Wampfler** (2024). *On Multimodal Emotion Recognition for Human-Chatbot Interaction in the Wild*. In Proceedings of the 26th International Conference on Multimodal Interaction (ICMI '24), San Jose, Costa Rica, November 4–8, 2024.

N. Kovačević, C. Holz, T. Günther, M. Gross and **R. Wampfler** (2023). *Personality Trait Recognition Based on Smartphone Typing Characteristics in the Wild*. IEEE Transactions on Affective Computing, pp. 1–11, 2023.

**R. Wampfler**, S. Klingler, B. Solenthaler, V. R. Schinazi, M. Gross and C. Holz (2022). *Affective State Prediction from Smartphone Touch and Sensor Data in the Wild*. Proceedings of the Conference on Human Factors in Computing Systems (CHI), New Orleans, USA, April 30–May 5, 2022, pp. 1–14.

**R. Wampfler**, S. Klingler, B. Solenthaler, V. R. Schinazi and M. Gross (2020). *Affective State Prediction Based on Semi-Supervised Learning from Smartphone Touch Data*. Proceedings of the Conference on Human Factors in Computing Systems (CHI), Virtual, April 25–30, 2020, pp. 1–13.

N. Kovačević, **R. Wampfler**, B. Solenthaler, M. Gross and T. Günther (2020). *Glyph-Based Visualization of Affective States*. Eurographics/IEEE VGTC Symposium on Visualization (EuroVis), Virtual, May 25–29, 2020, pp. 121–125.

**R. Wampfler**, S. Klingler, B. Solenthaler, V. R. Schinazi and M. Gross (2019). *Affective State Prediction in a Mobile Setting using Wearable Biometric Sensors and Stylus*. Proceedings of the International Conference on Educational Data Mining (EDM), Montréal, Canada, July 2–5, 2019, pp. 224–233.

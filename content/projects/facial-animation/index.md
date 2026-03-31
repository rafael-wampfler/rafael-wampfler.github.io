---
title: Facial Animation Synthesis
date: 2024-01-01
weight: 40
tags:
  - Facial Animation
  - Speech Animation
  - Generative Models
  - Transformers
  - Computer Graphics
summary: >
  Efficient transformer-based pipelines for text-driven and speech-driven 3D facial animation — achieving real-time performance through phoneme-level speech modeling and contrastive learning to decouple emotion from content.
---

## Overview

Realistic, expressive facial animation is a critical component of embodied conversational agents. For AI characters to communicate naturally, their facial movements must be synchronized with speech, emotionally consistent, and computationally efficient enough for real-time use. This project develops deep learning architectures that achieve all three goals.

## Motivation

The challenge of generating high-quality 3D facial animation from text or speech involves several competing requirements:

- **Expressiveness**: Facial motion should convey the speaker's emotional state convincingly
- **Synchronization**: Lip movements must match phoneme timing precisely to avoid the uncanny valley
- **Consistency**: Emotional expressivity should be decoupled from semantic content, allowing the same phrase to be delivered in multiple emotional registers
- **Efficiency**: Systems deployed in interactive agents must run in real time on consumer hardware

Prior approaches either sacrifice expressiveness for speed, or require enormous training data and computation. Our work addresses both efficiency and expressiveness simultaneously by rethinking how deep learning encodes linguistic and acoustic structure.

## Approach

### PhonemeNet (MIG 2025)

**PhonemeNet** applies a transformer pipeline specifically designed for the phoneme-level structure of speech. Rather than treating the speech signal as a raw audio waveform or frame-level features, PhonemeNet operates at the level of phonemes — the fundamental units of speech that determine lip shape. This problem-specific inductive bias yields both improved accuracy and computational efficiency compared to architectures that ignore linguistic structure.

PhonemeNet takes text input, extracts phoneme sequences, and generates corresponding 3D facial blendshape sequences that are synchronized with speech audio. The pipeline achieves real-time performance on standard hardware, making it suitable for deployment in interactive embodied agents.

PhonemeNet received the **Best Paper Honorable Mention** at the 18th ACM SIGGRAPH Conference on Motion, Interaction, and Games (MIG 2025).

### EmoSpaceTime (MIG 2024)

**EmoSpaceTime** addresses the problem of emotionally expressive 3D speech animation through a contrastive learning strategy. The core insight is that facial animation should be factorized into two independent components: **emotion** (how the speaker feels) and **content** (what the speaker is saying). By learning to decouple these in a shared embedding space, EmoSpaceTime enables:

- Transfer of emotional style between speakers
- Consistent emotional expressivity across different sentences
- Fine-grained control over emotional intensity at inference time

The resulting animations are both emotionally coherent — the emotion is consistent throughout an utterance — and semantically coherent — lip synchronization is accurate regardless of the emotional style applied.

## Key Results

- PhonemeNet achieves real-time text-driven facial animation with best-in-class lip synchronization accuracy — Best Paper Honorable Mention at MIG 2025
- EmoSpaceTime demonstrates that contrastive decoupling of emotion and content significantly improves expressive quality while maintaining temporal coherence

## Publications

P. Witzig, B. Solenthaler, M. Gross and **R. Wampfler** (2025). *PhonemeNet: A Transformer Pipeline for Text-Driven Facial Animation*. Proceedings of the 18th ACM SIGGRAPH Conference on Motion, Interaction, and Games (MIG '25), Zurich, Switzerland, December 3–5, 2025, pp. 1–11. **Best Paper Honorable Mention.**

P. Witzig, S. Solenthaler, M. Gross, **R. Wampfler** (2024). *EmoSpaceTime: Decoupling Emotion and Content through Contrastive Learning for Expressive 3D Speech Animation*. In Proceedings of the 17th ACM SIGGRAPH Conference on Motion, Interaction and Games (MIG '24), Arlington, USA, November 21–23, 2024.

---
title: Digital Einstein
date: 2021-06-01
weight: 10
tags:
  - Embodied Conversational Agents
  - Interactive AI
  - Multimodal AI
  - Digital Humans
links:
  - type: site
    url: https://ethz.ch/en/the-eth-zurich/global/digital-einstein.html
    name: Official ETH Page
summary: >
  An embodied conversational AI agent bringing Albert Einstein back to life through multimodal interaction — combining speech synthesis, facial animation, and cognitive reasoning. Deployed globally at scientific conferences, tech events, and public outreach.
image:
  caption: 'A user interacting with Digital Einstein'
  focal_point: Smart
---

## Overview

Digital Einstein is a flagship embodied conversational agent that brings the historical figure of Albert Einstein to life through real-time multimodal AI interaction. The system combines speech recognition and synthesis, facial animation, gesture control, and a cognitively grounded language understanding pipeline to deliver immersive, personality-consistent conversations.

Digital Einstein serves three interconnected roles:

1. **Research platform** — a testbed for studying human–agent interaction in constrained embodied settings, yielding insights on affective computing, personality modeling, dialog act classification, and conversational AI.
2. **Education platform** — a live demonstration of conversational AI and multimodal deep learning deployed in university events, science outreach, and public engagement.
3. **Public engagement tool** — reaching thousands of visitors globally at scientific conferences, tech summits, museums, and public events, generating sustained international recognition for ETH Zurich.

## Motivation

How can AI systems convincingly portray a well-known historical personality — someone whose knowledge, values, and speaking style are culturally established — in real-time dialogue with arbitrary members of the public? This challenge crystallizes core problems in interactive AI: maintaining factual and characterological consistency, adapting dynamically to unpredictable user inputs, and delivering a compelling embodied experience at scale.

Digital Einstein was conceived as both a scientific challenge and a communication vehicle: making abstract advances in AI tangible for general audiences while simultaneously driving rigorous research on the underlying problems.

## Approach

The system is built on a full-pipeline architecture described in the SIGGRAPH 2025 paper *"A Platform for Interactive AI Character Experiences"*. Key components include:

- **Perception layer**: Real-time speech recognition via Microsoft Azure Speech Services and multimodal input processing through a webcam-based vision pipeline, including face detection, user characterization, head pose estimation, and re-identification.
- **Cognitive reasoning layer**: Knowledge-grounded dialogue management with integrated response generation, powered by GPT-4.1 mini, featuring dynamic personality infusion that adapts outputs to user-selectable archetypes: Digital Einstein, Rude Bulldozer, Drama Volcano, Zen Master, and Hashtag Prophet.
- **Animation synthesis**: Data-driven facial animation synchronized with speech output using NVIDIA Audio2Face, blended with emotion-conditioned expressions, and complemented by a curated library of motion-captured body animations categorized by avatar state.
- **Embodiment**: A stylized Albert Einstein avatar rendered in Unity on a 65-inch display, integrated into a themed early-20th-century physical environment with spatial audio, a hidden microphone, and physical personality sliders built from potentiometers and an Arduino.

The SIGGRAPH Asia 2024 demonstration paper *"Immersive Conversations with Digital Einstein: Linking a Physical System and AI"* details the physical installation setup, including the integration of an animatronic head with the real-time AI pipeline at the Tokyo venue.

## Key Results

Digital Einstein has been demonstrated at over 20 major events worldwide, including:

- **SIGGRAPH Asia 2024** (Tokyo, Japan) — Emerging Technologies
- **SIGGRAPH 2025** (Vancouver, Canada)
- **GITEX Global 2024 & 2025** (Dubai, UAE) — Swiss Pavilion
- **World Economic Forum 2024 & 2026** (Davos, Switzerland)
- **Berlin Science Week 2025** (Berlin, Germany)
- **Swiss Re Resilience Summit 2024** (Rüschlikon, Switzerland)
- **Microsoft Initiative to Advance AI Diffusion in Switzerland 2025** (Berne)
- **After the Algorithm Festival 2026** (Zurich, Switzerland)

The project has generated sustained international media coverage and public interest, positioning ETH Zurich as a world leader in embodied conversational AI.

{{< figure src="gitex.jpg" caption="Swiss Ambassador to the UAE, Arthur Mattli, interacting with Digital Einstein at GITEX Global in Dubai." >}}

## Learn More

- [Official ETH Digital Einstein page](https://ethz.ch/en/the-eth-zurich/global/digital-einstein.html)
- [Digital Einstein's Year of Adventures and Reinvention](https://ethambassadors.ethz.ch/2025/11/27/digital-einsteins-year-of-adventures-and-reinvention/)
- [Digital Einstein's Journey to Dubai and Tokyo](https://ethambassadors.ethz.ch/2025/01/09/digital-einsteins-journey-to-dubai-and-tokyo/)

## Primary Publications

**R. Wampfler**, C. Yang, D. Elste, N. Kovačević, P. Witzig and M. Gross (2025). *A Platform for Interactive AI Character Experiences*. Proceedings of the SIGGRAPH Conference Papers '25 (Vancouver, Canada, August 10–14, 2025), pp. 1–11.

**R. Wampfler**, N. Kovačević, P. Witzig, C. Yang, M. Gross (2024). *Immersive Conversations with Digital Einstein: Linking a Physical System and AI*. In SIGGRAPH Asia 2024 Emerging Technologies (SA '24) (Tokyo, Japan, December 3–6, 2024).

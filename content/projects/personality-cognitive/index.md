---
title: Personality & Cognitive Architectures for Conversational Agents
date: 2022-01-01
weight: 30
tags:
  - Conversational Agents
  - Personality Modeling
  - Cognitive Architectures
  - Large Language Models
  - Believable Agents
summary: >
  Deep learning-based cognitive frameworks that enable conversational agents to maintain consistent personality, beliefs, values, and emotional states across extended interactions — integrating memory, reasoning, and affect into unified architectures.
---

## Overview

Standard large language models (LLMs) are stateless by design: each response is generated without a persistent sense of self, stable values, or accumulated memory of prior interactions. This makes them ill-suited for applications requiring a believable, consistent agent personality — such as embodied historical figures, therapeutic companions, or narrative characters. This project develops deep learning-based cognitive frameworks that address this limitation.

## Motivation

For conversational agents to be genuinely useful in education, mental health, entertainment, and public engagement, they must do more than generate fluent text. They must maintain:

- **Characterological consistency**: A stable personality that users recognize and can model predictively
- **Value alignment**: Responses grounded in a coherent set of beliefs and priorities
- **Epistemic coherence**: Awareness of what the agent knows and does not know
- **Emotional expressivity**: Affect that reflects the agent's personality and conversational context

Achieving all of this while remaining interpretable and safe requires principled architectural choices rather than prompt engineering alone.

## Approach

### The BEE Cognitive Framework (IVA 2025)

The **Belief-Value-Aligned, Explainable, and Extensible (BEE)** cognitive framework provides a structured architecture for conversational agents. BEE decomposes agent cognition into explicit modules:

- **Belief management**: A persistent, queryable representation of the agent's knowledge and world model
- **Value alignment**: A constraint layer that ensures generated responses conform to the agent's ethical commitments and personality
- **Explainability**: Transparent reasoning traces that allow developers and supervisors to audit agent behavior
- **Extensibility**: A modular design that supports new knowledge domains and personality profiles without retraining

BEE received the **Best Paper Honorable Mention** at IVA 2025.

### Joint Personality-Emotion Framework (IVA 2025)

The **Joint Personality-Emotion Framework** unifies personality modeling (using Big Five trait representations) with momentary emotional state tracking in a single learned architecture. By jointly modeling personality and emotion — which are deeply intertwined in human behavior — the system produces responses that feel emotionally authentic and characterologically stable. Contrastive learning strategies decouple emotion from semantic content, allowing the same underlying personality to express itself across diverse emotional registers.

### Personality Infusion via Chatbot Interactions (CUI 2024, IMWUT 2024)

We have extensively studied how personality manifests in conversational AI systems. Key findings include:

- **What personality dimensions does GPT-3 express** during human-chatbot interactions, and how do these map to the Big Five personality taxonomy (IMWUT 2024)
- **Dynamic personality infusion** — how to modulate expressed personality in real time by conditioning language model generation on personality embeddings (CUI 2024)

### Narrative Agents and Emergent Storytelling (AAAI AIIDE 2025)

In the domain of interactive narrative, we developed a **Dynamic Cognitive Framework for Guided Emergent Storytelling** that enables narrative agents to pursue coherent story arcs while remaining responsive to player input. The framework uses explicit belief-desire-intention representations to steer language model generation toward narratively coherent outcomes without sacrificing interactivity.

## Key Results

- BEE framework achieved Best Paper Honorable Mention at IVA 2025
- Joint Personality-Emotion Framework demonstrated stable personality maintenance across extended dialogues with diverse user populations
- IMWUT 2024 paper provided the first large-scale empirical characterization of GPT-3's expressed personality dimensions
- Dynamic narrative framework enabled coherent 30+ turn story experiences with novel player choices

## Publications

N. Kovačević, C. Holz, M. Gross and **R. Wampfler** (2025). *A Joint Personality-Emotion Framework for Personality-Consistent Conversational Agents*. In Proceedings of the 25th International Conference on Intelligent Virtual Agents (IVA '25), Berlin, Germany, September 16–19, 2025, pp. 1–9. **Best Paper Honorable Mention.**

C. Yang, M. Gross and **R. Wampfler** (2025). *BEE: Belief-Value-Aligned, Explainable, and Extensible Cognitive Framework for Conversational Agents*. In Proceedings of the 25th International Conference on Intelligent Virtual Agents (IVA '25), Berlin, Germany, September 16–19, 2025, pp. 1–9. **Best Paper Honorable Mention.**

C. Yang, M. Gross and **R. Wampfler** (2025). *Steering Narrative Agents through a Dynamic Cognitive Framework for Guided Emergent Storytelling*. Proceedings of the AAAI Conference on Artificial Intelligence and Interactive Digital Entertainment (AIIDE), Edmonton, Canada, November 10–14, 2025, pp. 1–11.

N. Kovačević, C. Holz, M. Gross and **R. Wampfler** (2024). *The Personality Dimensions GPT-3 Expresses During Human-Chatbot Interactions*. Proceedings of the ACM on Interactive, Mobile, Wearable and Ubiquitous Technologies, ACM, vol. 8, no. 2, 2024, pp. 1–36.

N. Kovačević, T. Boschung, C. Holz, M. Gross and **R. Wampfler** (2024). *Chatbots With Attitude: Enhancing Chatbot Interactions Through Dynamic Personality Infusions*. Proceedings of the 6th International Conference on Conversational User Interfaces (CUI), Luxembourg, July 08–10, 2024, pp. 1–16.

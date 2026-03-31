---
title: Dialog Act Classification
date: 2024-01-01
weight: 50
tags:
  - Dialog Act Classification
  - Conversational AI
  - Multimodal AI
  - Natural Language Processing
summary: >
  Multimodal dialog act classification for conversations with digital characters — interpreting the communicative intent of user utterances to drive appropriate agent responses in interactive embodied systems.
---

## Overview

For a conversational agent to respond appropriately, it must understand not just *what* a user says, but *why* they said it — the communicative intent behind their utterance. Dialog Act (DA) classification is the task of categorizing utterances by their function in conversation (e.g., question, assertion, greeting, request, clarification). This project develops multimodal dialog act classifiers tailored for interactions with digital characters.

## Motivation

Standard dialog act classification systems are trained on text transcriptions alone. In real-world interactions with embodied agents, however, users communicate through a rich combination of speech prosody, gaze, gesture, and lexical content. A question delivered with rising intonation carries different meaning than the same words spoken flatly; a greeting accompanied by eye contact differs from one delivered distractedly.

For digital characters that must respond naturally in real time, dialog act classification must therefore be multimodal — integrating acoustic, linguistic, and where available, visual signals — and must operate with low latency to support interactive response times.

## Approach

Our multimodal dialog act classifier integrates:

- **Lexical features**: Encoded via transformer-based text encoders fine-tuned on dialog corpora
- **Acoustic features**: Prosodic signals including pitch, energy, and speech rate, extracted from the raw audio signal
- **Temporal context**: Conversation history modeling to resolve ambiguous acts through discourse-level context

The system is evaluated on naturalistic conversations with digital characters — a challenging setting because users frequently use fragmented, spontaneous speech rather than complete, grammatical sentences. The classifier is optimized for both accuracy and latency, enabling real-time use within the Digital Einstein pipeline.

## Key Results

- Demonstrated that multimodal integration (text + acoustic features) significantly outperforms text-only baselines for dialog act classification in digital character conversations
- Achieved real-time classification latency compatible with interactive agent deployment
- Provided insights into which dialog acts are most frequently misclassified in human-agent interaction, informing future system design

## Publication

P. Witzig, R. Constantin, N. Kovačević and **R. Wampfler** (2024). *Multimodal Dialog Act Classification for Conversations With Digital Characters*. Proceedings of the 6th International Conference on Conversational User Interfaces (CUI), Luxembourg, Luxembourg, July 08–10, 2024, pp. 1–14.

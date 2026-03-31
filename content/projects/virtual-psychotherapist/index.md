---
title: Virtual Psychotherapist
date: 2023-01-01
weight: 60
tags:
  - Mental Health AI
  - Embodied Conversational Agents
  - Psychotherapy
  - Digital Health
  - Large Language Models
summary: >
  Embodied conversational agents for mental health support, developed in partnership with Prof. Andrew Gloster (University of Lucerne). The project comprises a patient-facing therapeutic companion and a therapist training simulator, both grounded in Acceptance and Commitment Therapy (ACT).
---

## Overview

Access to evidence-based psychotherapy remains severely limited worldwide — constrained by long waitlists, resource scarcity, and geographic disparities. The Virtual Psychotherapist project develops embodied conversational AI agents that complement clinical care by extending access, supporting therapeutic practice, and enabling scalable training.

This initiative is conducted in close collaboration with **Prof. Andrew Gloster** (University of Lucerne), whose team provides clinical expertise and direct access to real therapy data.

## Motivation

Two distinct but complementary challenges motivate this project:

1. **Scaling patient access**: Many individuals who would benefit from psychotherapy cannot access it due to cost, waitlists, or geography. AI-based companions that operate between sessions, provide continuous support, and conduct structured therapeutic conversations could meaningfully improve outcomes at scale.

2. **Improving therapist training**: Training clinicians in evidence-based interventions requires repeated practice with feedback — but opportunities for safe, standardized training are limited by ethical and resource constraints. Simulated patient systems powered by AI can provide unlimited deliberate practice in controlled settings.

## System Architecture

Both applications are built on a shared platform combining:

- **Large language model-based dialogue**: State-of-the-art LLMs for contextually appropriate, therapeutically grounded response generation
- **Retrieval-augmented generation (RAG)**: Responses grounded in evidence-based therapeutic literature, reducing hallucinations and ensuring adherence to clinical frameworks
- **Real-time psychological analysis**: Parallel processing pipelines that extract facts, detect psychological flexibility processes, recognize emotions, and monitor safety in real time
- **Embodied avatar presentation**: Synchronized speech synthesis and 3D avatar animation delivered through mobile and desktop applications
- **Clinician oversight**: Structured analysis outputs accessible to supervising therapists, enabling human-in-the-loop clinical governance

### Patient-Facing Application

The patient-facing component enables individuals to conduct therapeutic conversations with an embodied avatar between sessions. The system follows **process-based therapy** principles — particularly Acceptance and Commitment Therapy (ACT), an empirically supported approach targeting psychological flexibility through six core processes: acceptance, cognitive defusion, present-moment awareness, self-as-context, values clarification, and committed action.

Critically, the system is designed for clinical supervision, not autonomous intervention. All session data is structured and accessible to the supervising therapist, who can monitor progress and intervene as needed.

An evaluation against responses from professional psychotherapists demonstrated that the system's responses were rated significantly higher on understanding, interpersonal effectiveness, collaboration, and ACT alignment — while emphasizing that clinical judgment and the therapeutic relationship remain irreplaceable.

### Therapist Training Application

The training application enables psychotherapists to practice and refine therapeutic techniques through role-play interactions with a simulated patient. Key features include:

- **Clinically grounded patient simulation**: Virtual patient behavior conditioned on profiles derived from real therapy sessions, covering a range of clinical presentations and scenarios (suicidality, resistance, heightened anxiety, therapeutic rupture, and more)
- **Real-time ACT fidelity feedback**: An automated evaluator assesses each therapist utterance for adherence to ACT principles, providing immediate visual feedback and the option to retry alternative responses
- **Configurable scenarios**: Therapists can select specific clinical scenarios to target their practice

A systematic evaluation across 49 therapy transcripts identified GPT-4o-mini as the optimal feedback model, achieving the closest alignment with human supervisor ACT fidelity ratings.

## Safety and Ethics

Safety is a primary design constraint. The system includes:

- **Crisis detection**: Explicit classification of suicidal ideation and self-harm signals, triggering immediate presentation of crisis resources and mandatory clinician review
- **Unsafe-interaction detection**: Identification of conditions (e.g., active psychosis, mania) where LLM interaction may be counterproductive, with protocol-defined fallback responses
- **Non-autonomous design**: The system is explicitly positioned as a complement to clinical care, not a replacement — structured to require and facilitate clinician oversight

## Key Results

- Patient-facing system responses rated significantly higher than human therapist responses by automated evaluation and expert psychotherapists across understanding, collaboration, and ACT alignment
- Therapist training simulation rated as realistic by practicing psychologists; turn-by-turn feedback shown to increase therapist awareness of intervention choices
- Automated ACT fidelity assessment achieves strong agreement with human expert ratings across 49 therapy transcripts

## Research Partners

- **Prof. Andrew Gloster**, Department of Behavioural Sciences and Psychology, University of Lucerne

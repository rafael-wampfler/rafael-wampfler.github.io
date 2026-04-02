---
title: "MIND — Cognitive Health Monitoring"
date: 2025-01-01
weight: 80
tags:
  - Cognitive Health
  - Aging
  - Mobile AI
  - Large Language Models
  - Geospatial Models
  - Embodied Conversational Agents
summary: >
  A mobile AI platform for early detection of cognitive impairment in aging populations, integrating Large Geospatial Models for movement analysis, LLMs for conversational cognitive markers, and embodied avatars for guided assessments. Part of the NRF Singapore CREATE grant Future Health Technologies 2.
---

## Overview

The MIND (Monitoring and Supporting Cognitive Health) project creates a mobile platform for the early detection of cognitive impairment in aging populations. Early identification of decline — before it significantly impacts daily life — enables timely intervention, supports independent living, and improves long-term outcomes for older adults and their families.

MIND is part of the **Future Health Technologies 2 (FHT2)** initiative, a major research program funded by the **National Research Foundation Singapore (NRF) CREATE** grant.

## Motivation

Cognitive decline — from mild cognitive impairment to dementia — affects hundreds of millions of people worldwide. Current clinical detection relies predominantly on periodic in-clinic assessments that are episodic, costly, and often catch decline only after substantial impairment has occurred. A continuously operating, passive monitoring system that can detect subtle early warning signs in everyday behavior could transform the standard of care.

Two key insights motivate the MIND approach:

1. **Movement and navigation encode cognition**: Changes in how people navigate their environment — route choices, wayfinding strategies, spatial memory — are among the earliest and most sensitive indicators of cognitive decline. Analyzing GPS and sensor traces at scale can reveal these changes.
2. **Language reflects cognitive health**: Subtle changes in vocabulary, sentence complexity, topic management, and response latency in everyday conversation are measurable markers of cognitive change, detectable through automated language analysis.

## Approach

MIND integrates three complementary AI systems into a unified mobile platform:

### Large Geospatial Models (LGMs)

Large Geospatial Models analyze longitudinal GPS and mobility traces to detect patterns indicative of cognitive change. These include:

- **Route repetitiveness**: Increasing restriction of daily movement range
- **Navigation errors**: Unusual detours or disorientation in familiar environments
- **Mobility diversity**: Changes in the variety of visited locations over time

LGMs are trained on large-scale mobility datasets and fine-tuned to identify individual-level deviations from baseline behavior.

### LLMs for Conversational Cognitive Assessment

Large language models analyze conversation transcripts from daily interactions with the MIND app, detecting cognitive markers such as:

- Reduced lexical diversity and increased use of filler words
- Difficulty with topic maintenance and coherence
- Slowed response generation and increased hesitation
- Confusion or confabulation in response to everyday questions

These markers are tracked longitudinally to identify meaningful change relative to the individual's own baseline.

### Embodied Avatars for Guided Assessment and Training

An embodied conversational avatar conducts structured cognitive assessments — such as memory recall tasks, verbal fluency tests, and orientation questions — through natural spoken dialogue. The avatar also guides cognitive training exercises designed to maintain cognitive reserve.

The embodied format is critical: older adults are more likely to engage regularly with an interactive, socially present agent than with a text-based questionnaire or passive sensor. The avatar adapts its communication style to individual users, adjusting vocabulary, pacing, and support level to ensure accessibility.

### Integration and Privacy

All three systems operate on a shared mobile platform with strong privacy protections. Data is analyzed on-device where possible, and users maintain full control over what is shared with care providers. The platform produces structured reports for geriatricians and primary care physicians, enabling early clinical intervention.

## Significance

MIND represents a convergence of several research threads — geospatial AI, conversational AI, affective computing, and embodied interaction — applied to one of the most pressing health challenges of our time. By enabling early, passive, continuous monitoring, the platform aims to support successful aging in place and to delay or prevent the transition to care dependency.

## Research Partners and Funding

- **National Research Foundation Singapore (NRF) CREATE** — Future Health Technologies 2 (FHT2)
- **Bond University (Australia)**
- Collaboration with life sciences and medicine partners in Singapore

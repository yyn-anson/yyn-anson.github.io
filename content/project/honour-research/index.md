---
title: "Honour Research Project: Bias Detection through Unsupervised Learning"
description: "An innovative research project developing an unsupervised pipeline for quantifying misinformation and bias on social media through embedding and multi-agent analysis."
date: 2024-11-30
# featured_image: "https://via.placeholder.com/800x600"
# external_link: https://github.com/pandas-dev/pandas
tags: [Misinformation, "Social Network Analysis", "Machine Learning", "Unsupervised", "Bias Detection"]
---

# Bias Detection through Unsupervised Learning

*30 Nov 2024 – Current*

## Executive Summary

This innovative research project addresses a critical challenge in today's digital information ecosystem: detecting and quantifying political bias in news articles and social media content without requiring labeled training data. The framework introduces a novel fully unsupervised pipeline that combines geometric embedding-based techniques with a multi-agent evaluation system to provide a comprehensive, nuanced assessment of media bias across two dimensions - political leaning and rhetorical bias intensity.

## Problem Statement

In today's digital landscape, social media platforms have become the primary source of news for billions worldwide, fundamentally altering information flow and public discourse. This shift presents unprecedented challenges as algorithms selectively amplify content, often prioritizing engagement over accuracy and potentially exposing users to increasingly polarized and biased information. Such bias can profoundly influence public opinion formation, policy preferences, and voting behavior in democratic societies.

While traditional approaches to media bias detection typically rely on supervised learning with large labeled datasets, our research introduces a framework that eliminates this dependency, making bias detection more scalable, adaptable, and transparent.

## Methodology: A Two-Component Approach

Our framework consists of two complementary components that work together to provide a comprehensive bias assessment:

### 1. Embedding-Based Political Leaning Estimation

This component quantifies the political orientation of articles on a continuous left-right spectrum through several innovative techniques:

- **Article Embedding**: Content is transformed into dense vector representations using INSTRUCTOR, an instruction-finetuned text embedding model that captures semantic information relevant to political analysis.

- **Pseudo-Topic Clustering**: Articles are grouped into clusters based on topical similarity to normalize for content variation, ensuring political leaning is assessed within comparable contexts rather than across disparate subjects.

- **Contrastive Adversarial Fine-Tuning**: Embeddings are enhanced through triplet learning, where semantically aligned articles are pulled closer together while divergent articles are pushed further apart, amplifying fine-grained ideological distinctions within topical groups.

- **Directional Vector-Based Scoring**: A political spectrum axis is defined within the embedding space using prototypical left-leaning and right-leaning seed articles. Each article's political leaning score is computed as the normalized projection onto this axis, ranging from -1 (strongly left-leaning) to +1 (strongly right-leaning).

### 2. Multi-Agent LLM-Based Rhetorical Bias Analysis

This component evaluates the presence of biased rhetorical techniques regardless of political orientation:

- **Agent Configuration**: Rather than simulating political diversity, three specialized agents examine different aspects of bias:
  - **Structural Analysis Agent**: Examines article organization, framing, headline analysis, and source selection
  - **Content Analysis Agent**: Evaluates language choice, fact-opinion separation, and evidence assessment
  - **Contextual Analysis Agent**: Focuses on omissions, historical patterns, and comparison to mainstream reporting

- **Evaluation Protocol**: The process occurs in three sequential phases:
  1. Independent article analysis by each specialized agent
  2. Structured deliberation facilitated by a moderator agent
  3. Consensus formation, producing a five-point rhetorical bias rating (1=minimal bias, 5=extreme bias) with supporting evidence

## Integrated Bias Assessment

The outputs from both components are combined into a two-dimensional bias representation:
- **X-axis**: Political leaning from -1 (strongly left) to +1 (strongly right)
- **Y-axis**: Rhetorical bias intensity from 0 (minimal bias) to 1 (extreme bias)

This representation allows for nuanced distinctions between different bias profiles. For example, an article might be identified as strongly right-leaning but employing relatively few biased rhetorical techniques, while another might be moderately left-leaning but using highly biased rhetorical devices.

## Visualization

Our framework generates several types of visualizations to help users understand and interpret bias profiles:

- **2D Bias Maps**: Plot media outlets in a two-dimensional space showing both political leaning and rhetorical bias intensity
- **Score Distributions**: Histograms showing the distribution of political leaning scores across all articles
- **Source Comparisons**: Bar charts comparing mean political leaning scores across different media outlets
- **Beeswarm Plots**: SHAP-like visualizations showing individual article distributions by source
- **Violin Plots**: Probability density visualizations showing the distribution shape for each source

## Key Contributions

Our framework offers several significant advantages over existing approaches:

1. **No Labeled Data Requirement**: Eliminates the need for expensive human-annotated datasets, enabling analysis at scale
2. **Domain Generalizability**: Can be applied to any domain with opposing viewpoints, not limited to political content
3. **Transparent Assessment**: Provides explicit reasoning and evidence for bias evaluations, fostering trust
4. **Bias Mitigation**: Combines geometric methods with deliberative LLM analysis to reduce potential biases inherent in either approach alone

## Applications and Impact

This research contributes to several important objectives:
- Providing tools for media literacy and critical information consumption
- Enabling more balanced content recommendation systems
- Supporting researchers and policymakers with insights into information flow
- Strengthening democratic discourse by helping citizens identify bias in an increasingly complex digital information ecosystem

## Future Directions

Future work will address several promising avenues:
- Expanding the framework to incorporate multimodal analysis of visual and textual elements
- Developing methods for continuous learning and adaptation to evolving political discourse
- Exploring cross-cultural adaptations for international media analysis
- Further optimizing the multi-agent protocol to reduce computational requirements

By providing accessible tools for bias detection without relying on costly labeled data or domain-specific customization, this project aims to contribute to a more informed and discerning public discourse in the digital age.

<!-- <iframe src="uploads/COMP400_Bias_Rating.pdf" width="100%" height="600px"></iframe> -->
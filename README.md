# MultiHoax: A Dataset of Multi-hop False-premise Questions

## Overview

MultiHoax is a benchmark dataset designed to evaluate Large Language Models' (LLMs) ability to detect false premises embedded in multi-hop reasoning tasks. Unlike existing datasets that focus on single-hop false-premise questions, MultiHoax introduces a novel challenge by requiring models to reason across multiple inferential steps while identifying incorrect assumptions.

## Paper

Our dataset is introduced in the paper:
**MultiHoax: A Dataset of Multi-hop False-premise Questions**

[Paper Link (to be added)]

## Dataset Structure

Each instance in the MultiHoax dataset consists of:

- **Question and Answer Choices:** Each question contains at least one false premise and is paired with four answer choices: three plausible distractors and one "I do not know" option, randomly positioned to prevent bias.
- **False Premise Explanation:** A brief description clarifying why the assumption in the question is incorrect.
- **Country and Category:** The dataset covers **7 countries** (China, France, Germany, Italy, the United States, the United Kingdom, and Iran) and **10 knowledge domains**, including:
  - Food
  - Sports
  - Geography
  - Education
  - History
  - Entertainment
  - Religion
  - Science & Technology
  - Arts & Literature
  - Holidays & Leisure
- **Types of False Premises:** Inspired by prior work, false premises in the dataset are categorized as:
  - **Property** (Incorrect attribute assigned to an entity)
  - **Event** (Falsely implying an event happened or didn’t happen)
  - **Entity** (Incorrect entity mentioned)
  - **Scope** (Exaggerated or limited context)
  - **Index** (Confusing order or numerical values)
- **Answer Types:** Following previous benchmarks, answers are classified into categories such as **person, location, event, number, and common nouns**.
- **Multi-Hop Reasoning Type:** Each question requires multi-step reasoning of one of the following types:
  - **Named Entity Reasoning** (Linking facts through an intermediate entity)
  - **Temporal Reasoning** (Identifying time-based relationships)
  - **Geographical Reasoning** (Understanding spatial relationships)
  - **Intersection Reasoning** (Finding an entity satisfying multiple conditions)
  - **Comparison Reasoning** (Comparing attributes or facts across entities)
- **Wikipedia Grounding:** Each question is linked to a relevant Wikipedia page for factual verification.

## Benchmarking & Results

Our experiments demonstrate that state-of-the-art LLMs struggle with detecting false premises in **multi-hop questions**, showing inconsistent performance across countries and categories. These findings highlight the challenges in **reasoning robustness** and emphasize the need for better uncertainty modeling in AI systems.

## License
This dataset is licensed under the Creative Commons Attribution 4.0 International (CC BY 4.0) License. You are free to share and adapt the dataset, provided appropriate credit is given.

For more details, see the [LICENSE](LICENSE) file.


# Environment-Aware NPC Dialogue with LLMs

This repository accompanies the paper:

**Empowering NPC Dialogue with Environmental Context Using LLMs and Panoramic Images**  
Grega Radež, Ciril Bohak

The project explores how non-playable characters (NPCs) in games can be augmented with real-time environmental awareness by combining panoramic image capture, semantic segmentation, and large language models (LLMs). The goal is to enable NPCs to generate spatially grounded, context-aware dialogue that reflects their immediate surroundings.

---

## Overview

Traditional NPC dialogue systems rely on scripted logic or context-free language models, which limits immersion and believability. This work introduces a system that:

- Captures **panoramic visual context** from the NPC’s viewpoint
- Applies **semantic object segmentation** to identify nearby objects
- Extracts **spatial cues** from the game engine’s scene graph
- Encodes environmental information in a **structured prompt**
- Enables **LLM-driven NPCs** to reference nearby objects and spatial relationships during interaction

The system is implemented as a modular pipeline designed to integrate with modern game engines.

---

## Study Results

The system was evaluated in two stages:

### Expert Evaluation
An expert interview was conducted to assess:
- Coherence and plausibility of NPC responses
- Accuracy of referenced environmental features
- Perceived immersion compared to baseline approaches

The expert identified the full system (visual + spatial context + supporting prompt) as producing the most coherent and believable dialogue, while also highlighting limitations related to depth perception and inter-object spatial relations.

### Comparative User Study
A user study compared:
- **Environment-aware NPC dialogue**
- **Baseline LLM dialogue using only a supporting prompt**

### 🔎 Results

To support transparency and reproducibility, the study results are publicly available:

- **Results website:**  
 [Website](https://docs.google.com/spreadsheets/u/1/d/e/2PACX-1vTRuiZxseOBfr1-7qoWGP9ftvr8jT06QxL71evHmE-31-fInsTwiH4dUGlsD1WbNg/pubhtml)

- **Anonymized dataset (CSV):**  
  [CSV](https://docs.google.com/spreadsheets/d/e/2PACX-1vTRuiZxseOBfr1-7qoWGP9ftvr8jT06QxL71evHmE-31-fInsTwiH4dUGlsD1WbNg/pub?gid=1340224966&single=true&output=csv)

The dataset includes aggregated user preferences and Likert-scale ratings used in the analysis presented in the paper.


Key findings:
- Participants consistently preferred the environment-aware NPC responses
- Context-aware dialogue was rated higher for immersion and relevance
- Users appreciated NPCs referencing nearby objects and scene features
- Common limitations included response verbosity and fine-grained spatial ambiguity

Overall, the results support the effectiveness of integrating visual and spatial context into NPC dialogue generation.

---

## Implementation

**This repository contains research materials only.**  
The full implementation (game engine project, scripts, and assets) is hosted separately.

<!--
**Implementation repository:**  
**https://github.com/USERNAME/environment-aware-npc-llm**

(The implementation repository includes Unreal Engine blueprints, RAM++ integration, prompt construction logic, and evaluation scenes.)
-->
---

## Citation

If you use this work in your research, please cite these papers:

```bibtex
@conference{RadezBohak2024,
  author = {Grega Radež and Ciril Bohak},
  title = {Integrating environmental awareness into NPCs : contextual conversational interaction in games},
  year = {2024},
  pages = {11-29},
  booktitle={HCI-SI 2024 : Human-Computer Interaction Slovenia 2024 : proceedings of the 9th Human-Computer Interaction Slovenia (HCI SI) Conference 2024 : Ljubljana, Slovenia, November 8, 2024},
}

@article{RadezBohak2025,
  title = {Empowering NPC Dialogue with Environmental Context Using LLMs and Panoramic Images},
  author = {Radež, Grega and Bohak, Ciril},
  journal = {Under review},
  year = {2025},
}

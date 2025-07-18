

# European Artist Bank – Computer Vision PoC (Proof of Concept)

## Overview

This project demonstrates a **Computer Vision Proof of Concept** using multiple advanced AI models for detailed **image classification**. The primary aim is to validate the applicability of vision AI in the cultural and creative sectors by performing model-based interpretation of visual objects.

The notebook is deployed entirely within **European infrastructure (Germany)**, complying with data residency and sovereignty standards. It integrates OpenAI-compatible endpoints to interact with hosted large multimodal models.

## Use Case Context

Inspired by **Volkswagen's collaboration with HiveMapper** (a decentralized physical infrastructure network – DePIN – built on Solana), the project explores how crowdsourced imagery combined with AI analysis can be used for real-time understanding of visual environments. Similar to how **HiveMapper processes dashcam imagery** to detect changes in road conditions, the current proof-of-concept processes **3D-printed object images** to extract visual attributes using diverse vision models.

---

## Table of Contents

* Model Catalog
* Utility Functions
* Image Preparation
* Inference on Images
* Results Dashboard
* Summary Generation

---

## Key Features

* **Multi-Model Evaluation**: Supports classification through various vision-capable LLMs:

  * `internvl2.5-8b`
  * `qwen2.5-vl-72b-instruct`
  * `gemma-3-27b-it`

* **Detailed Image Interpretation**: For each image, models return descriptions focusing on:

  * Shape
  * Texture
  * Color
  * Material

* **Dashboard Interface**: HTML-based side-by-side visual comparison of models’ outputs.

* **Summarization Engine**: Uses `meta-llama-3.1-8b-instruct` to merge model outputs into a unified paragraph per image.

---

## Technical Stack

* **Language**: Python (Jupyter Notebook)
* **APIs**: OpenAI-compatible Vision API endpoints (hosted in Germany)
* **Libraries**:

  * `openai`
  * `IPython.display`
  * `base64`
  * `markdown`
  * `json`

---

## Workflow Summary

1. **Model Discovery**
   Connect to local OpenAI-compatible endpoint to retrieve available models.

2. **Image Encoding**
   Convert local `.jpg` images to Base64 strings for API transport.

3. **Model Inference**
   Each image is analyzed by selected vision models. Outputs include structured object descriptions.

4. **Results Rendering**
   Custom dashboard displays:

   * Original image
   * Individual model results
   * Unified summary (aggregated via LLaMA 8B)

5. **Summary Generation**
   Model responses are merged and condensed using `meta-llama-3.1-8b-instruct`.

---

## Real-World Relevance

The methodology mirrors industrial applications, such as **Volkswagen ADMT’s integration of Hivemapper Bee Maps**, where crowdsourced dashcam footage is used for:

* Mapping urban changes (construction, parking, closures)
* Supporting autonomous vehicle operations
* Maintaining high-resolution, real-time geographic databases

This PoC demonstrates how similar techniques can be applied across domains – from mapping infrastructure to **digitally archiving and analyzing artworks** using vision AI.

---

## Future Directions

* Integration with decentralized image networks (e.g., IPFS or Solana-based DePIN nodes)
* Expansion to larger image sets with automated batch inference
* Embedding outputs into knowledge graphs or artist metadata systems
* Use in cultural heritage, NFT curation, or AI-driven gallery indexing

---

## License

MIT License

---

## Contact

For questions, collaborations, or deployment in enterprise settings:
📩 *[gordon.dyballa@bht-berlin.de](mailto:gordon.dyballa@bht-berlin.de)*



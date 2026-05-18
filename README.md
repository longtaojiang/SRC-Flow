# SRC-Flow: Compact Semantic Representations Enable Normalizing Flows for Image Generation

> **SRC-Flow: Compact Semantic Representations Enable Normalizing Flows for Image Generation**  
> Longtao Jiang, Jiangmin Bao, Zhendong Wang, Xin Tao, Pengfei Wan, Zhihui Li, Xiaojun Chang

[![arXiv](https://img.shields.io/badge/arXiv-coming%20soon-b31b1b.svg)](#)
[![Code](https://img.shields.io/badge/Code-coming%20soon-lightgrey)](#)
[![Model](https://img.shields.io/badge/Models-coming%20soon-lightgrey)](#)

This repository contains the official project page and release information for **SRC-Flow**, a normalizing-flow framework for image generation in compact semantic representation spaces.

The paper is currently under review.  
Code and pretrained models are **not released at this stage** and will be made available after the review process.

---

## News

- **[2026-05-18]** Paper released on arXiv.
- **[Coming Soon]** Code release.
- **[Coming Soon]** Pretrained checkpoints.
- **[Coming Soon]** Inference and evaluation scripts.

---

## Overview

Normalizing flows provide exact likelihood computation and deterministic invertible sampling, but they have historically lagged behind diffusion models in large-scale image generation.

We identify a key obstacle: normalizing flows must learn a **single fixed invertible transport** over the full ambient space. This makes them highly sensitive to high-dimensional representations. Modern pretrained visual representations, such as RAE features, are semantically rich but high-dimensional and overcomplete.

**SRC-Flow** addresses this issue by introducing a **Semantic Representation Compressor (SRC)**, which compresses high-dimensional RAE features into a compact semantic space before flow modeling. The normalizing flow is then trained in this compact space, reducing the modeling burden while preserving decoder-compatible semantic information.

<p align="center">
  <img src="assets/teaser.png" width="90%">
</p>

---

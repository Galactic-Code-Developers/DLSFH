# 🧠 DLSFH Entropy Diagnostic Pipeline

This repository contains a step-by-step system for analyzing solar magnetogram data using the Dodecahedron Linear String Field Hypothesis (DLSFH) and Multifaceted Coherence (MC) framework. It tracks coherence collapse, SGCV fragmentation, ψ⋆ₛ evolution, and flare prediction zones.

---

## 📋 Sections Overview

### 1. Entropy Vector Extraction
- Extracts 20-point entropy values from magnetogram images using DLSFH spatial masks.

### 2. Dual Overlay (Ideal + Adaptive)
- Displays node overlays on raw solar images using both geometric and adaptive entropy peaks.

### 3. ψ⋆ₛ vs Ghost Field Ratio
- Computes ψ⋆ₛ = exp(-S) for each node and compares against SGCV collapse thresholds.

### 4. Diagnostic Summary Auto-Report
- Prints a node-by-node coherence state and SGCV risk summary.

### 5. Flare Risk Detection (Collapsed Nodes)
- Identifies high-entropy nodes where ψ⋆ₛ < 0.82 and flags pre-flare instability zones.

### 6. Time-Series Recondensation Test
- Tracks ψ⋆ₛ trends over time to identify decaying vs recovering coherence.

### 7. Flare Trend Overlay Plot
- Visualizes ψ⋆ₛ trends as node overlays (🔽 Decaying, 🔼 Recondensing, ⏸ Stable).

### 8. Flare Risk Score System
- Computes a normalized score (0–1) based on SGCV fragmentation, ψ⋆ₛ decay, and ring activity.

### 9. SGCV Fragmentation Map
- Node color-coded map showing full, partial, or intact SGCV state.

### 10. CSV Exporter
- Saves entropy + ψ⋆ₛ + SGCV status per node into a `.csv` for analysis or training data.

### 11. Entropy Ring Phase Tracker
- Detects ring-like node activation patterns across entropy fields.

### 12. Recondensation Prediction Overlay
- Highlights nodes recovering ψ⋆ₛ coherence from <0.88 → >0.90.

### 13. SGCV–ψ⋆ₛ–Flare Correlation Score
- Weighted score from fragmentation, decay, and ring states to assess flare likelihood.

### 14. HTML Report Generator
- Creates a timestamped `.html` report with flare gauge, entropy ring data, and diagnostic notes.

---

## 📖 Glossary

| Term                  | Description |
|-----------------------|-------------|
| **ψ⋆ₛ (psi-star-s)**  | Coherence state of a DLSFH node, computed as ψ⋆ₛ = exp(-S) |
| **S (Entropy)**       | Shannon entropy extracted from magnetogram pixel regions |
| **SGCV**              | Superluminal Graviton Condensate Vacuum — the coherence medium |
| **Collapsed Node**    | Node with ψ⋆ₛ < 0.82 — no coherent field remains |
| **Recondensing Node** | Node recovering from decoherence, ψ⋆ₛ rising > 0.90 |
| **Entropy Ring**      | Adjacently collapsing nodes forming a belt/ring pattern |
| **Flare Score**       | Normalized value between 0 and 1 indicating flare probability |
| **ψ⋆ₛ Trend**         | Evolution of ψ⋆ₛ values over time (decaying, stable, or recondensing) |

---

## 🔧 Requirements

- Python 3.9+
- Google Colab or Jupyter Notebook
- `numpy`, `matplotlib`, `opencv-python`, `scikit-image`

---

## 🛰️ Future Extensions

- Animated overlays (GIF/MP4)
- Real-time solar feed integration
- CME post-analysis overlay
- Deep learning flare prediction training set

---

## 📄 License

MIT License © 2025 – DLSFH Analysis Team

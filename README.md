# Project Stargate (Mk IV)
### An Integral-Hybrid Cognitive Architecture for Embodied Agents

**Status:** Exploratory Prototype (v4.0.1)  
**Author:** Mubasher ([@MUbasher2020](https://github.com/MUbasher2020))

![Demo](stargate_recovery_demo.gif)
*Visualizing early behavioral emergence: The agent (HalfCheetah) learns to stand and lunge forward from scratch using only pixel inputs.*

## 🔬 Experiment Overview
Stargate investigates whether biological constraints (Homeostasis) can accelerate learning in robotic control. Unlike standard Model-Free RL (PPO/SAC) which often requires millions of samples, this architecture explores rapid behavioral emergence in **< 40,000 steps**.

![Benchmarks](REPORT_PERFORMANCE.png)
*Reward trajectory showing rapid onset of velocity-seeking behavior.*

## 🧠 Architecture
Stargate implements a bio-inspired **Control Loop** rather than a standard policy network:

1.  **Dual-Process World Model:** A VQ-VAE dynamics model with **Fast Weights** (Hippocampus) for instant adaptation and **Slow Weights** (Cortex) for stable physics rules.
2.  **Active Inference Planner:** Uses latent "Dreaming" (Simulation) to minimize Expected Free Energy (EFE), balancing curiosity with goal-seeking.
3.  **Autonomic Homeostasis:** The agent is driven by an internal Energy Budget. It moves to prevent "Starvation" (Energy < 0), forcing efficiency.

## 💻 Technical Stack
*   **Core:** PyTorch (Built from scratch, no external RL libraries).
*   **Environment:** Gymnasium (HalfCheetah-v4).
*   **Input:** 64x64 Pixels + Proprioception.
*   **Compute:** Trained entirely on a **Single Google Colab T4 GPU**.

## 📊 Limitations
*   Single-seed exploratory run.
*   Results demonstrate *speed of discovery*, not asymptotic stability.
*   The current policy prioritizes velocity over gait stability (as seen in the demo).

## 📥 Contact & Collaboration
I am an independent researcher seeking partners or labs to validate this architecture on physical hardware.

*   **Technical Whitepaper:** [Read Full PDF](Project_Stargate_Mk_IV_Technical_Whitepaper.pdf)
*   **Full Source Code:** Available for research review upon request.
*   **Email:** mubasherikram2020@gmail.com

---
*"Intelligence is not just pattern recognition; it is the ability to maintain homeostasis in a chaotic world."*

# Project Stargate (Mk IV)
### An Integral-Hybrid Cognitive Architecture for Embodied AGI

![Demo](stargate_recovery_demo.gif)

**Status:** Research Prototype (v4.0.1)  
**Author:** Mubasher ([@MUbasher2020](https://github.com/MUbasher202))

## 🚀 The Breakthrough
Stargate is a bio-inspired cognitive architecture designed to solve the **Sample Efficiency** problem in robotic control. 

While standard Reinforcement Learning (PPO/SAC) requires **~1,000,000 steps** to learn locomotion from visual inputs, Stargate achieves functional stability in **< 35,000 steps**.

![Benchmarks](REPORT_PERFORMANCE.png)

## 🧠 Architecture
Stargate rejects the standard "Input-Output" pipeline in favor of a biological **Control Loop**:

1.  **Dual-Process World Model:** A VQ-VAE dynamics model with Fast Weights (Hippocampus) for instant adaptation and Slow Weights (Cortex) for long-term physics rules.
2.  **Active Inference Planner:** Uses "Dreaming" (Latent Simulation) to minimize Expected Free Energy (EFE).
3.  **Autonomic Homeostasis:** The agent is driven by an internal Energy Budget. It moves not for points, but to prevent "Starvation" (Energy < 0).

## 💻 Technical Stack
*   **Core:** PyTorch (No external RL libraries used).
*   **Environment:** Gymnasium (HalfCheetah-v4).
*   **Compute:** Trained entirely on a **Single Google Colab T4 GPU**.

## 📥 Access & Licensing
I am currently looking for partners or organizations interested in acquiring this IP to apply it to real-world hardware.

*   **Full Source Code:** Available upon request.
*   **Technical Whitepaper:** [Read Full PDF](Project_Stargate_Mk_IV_Technical_Whitepaper.pdf)
*   **Contact:** [Mubasherikram2020@gmail.com]

---
*"Intelligence is not just pattern recognition; it is the ability to maintain homeostasis in a chaotic world."*

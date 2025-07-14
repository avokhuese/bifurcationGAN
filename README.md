# 🧠 BifurcationGAN: Time-Series Data Augmentation with Dynamical Systems-Inspired GANs

Welcome to the official repository for **BifurcationGAN** and **Oscillatory BifurcationGAN**, two novel generative adversarial architectures designed to synthesize realistic and structurally coherent time-series data by incorporating principles from nonlinear dynamical systems theory — specifically **Hopf bifurcation dynamics**.

## 🚀 Overview

Traditional GANs (e.g., Vanilla GAN, TTS-GAN, SigWGAN, SigcWGAN) face significant challenges when generating time-series data, including:
- Mode collapse
- Gradient vanishing
- Poor long-term temporal dependencies
- Training instability

**BifurcationGAN** and its enhanced variant **Oscillatory BifurcationGAN** embed bifurcation-aware transformations in the latent space. This enables the generator to simulate oscillatory and nonlinear behaviors common in real-world time-series datasets.

> These models consistently outperform baseline GANs on reconstruction quality and generative diversity across datasets such as:
- 🌡️ Jena Climate Temperature
- 🌱 Plant Sensor Humidity
- 💱 USDT-USD Cryptocurrency prices

---

## 📁 Repository Structure

```bash
.
├── models/
│   ├── bifurcation_gan.py         # Core architecture for BifurcationGAN
│   ├── oscillatory_bifurcation_gan.py # Extended architecture with oscillation loss
├── utils/
│   ├── data_loader.py             # Time-series preprocessing and batching
│   ├── evaluation_metrics.py      # FID, Inception Score, Wasserstein Loss, etc.
│   ├── bifurcation_dynamics.py    # Hopf bifurcation equations and latent path modeling
├── train/
│   ├── train_bifurcation_gan.py   # Training loop for BifurcationGAN
│   ├── train_oscillatory.py       # Training loop for Oscillatory BifurcationGAN
├── results/
│   ├── plots/                     # Training curves and visualization
│   └── generated_samples/         # Sample outputs from each GAN
├── datasets/
│   └── [Your Datasets Here]
├── README.md
└── requirements.txt



📝 Citation
If you find this work helpful, please cite:
@article{victor2025bifurcationgan,
  title={BifurcationGAN: Dynamical Systems-Inspired Generative Models for Robust Time-Series Augmentation},
  author={Alexander Okhuese Victor, Muhammad Intizar Ali},
  year={2025}
}

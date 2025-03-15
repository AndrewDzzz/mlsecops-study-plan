# Adversarial Attack Study Plan

1. -[ ] Core Concepts (1-2 Weeks)
2. -[ ] Classical Adversarial Attack Methods (2-3 Weeks)
3. -[ ] Adversarial Defense Techniques (2-3 Weeks)

## Core Concepts
- **Definitions:** 
  - Adversarial Examples
  - Adversarial Perturbations
  - Robustness
- **Attack Objectives:**
  - Targeted Attacks
  - Untargeted Attacks
- **Threat Models:**
  - White-box Attacks
  - Black-box Attacks
  - Physical Attacks

## Classical Adversarial Attack Methods
### White-box Attacks
- FGSM (Fast Gradient Sign Method)
- PGD (Projected Gradient Descent)
- CW Attack (Carlini & Wagner)
- JSMA (Jacobian-based Saliency Map Attack)

### Black-box Attacks
- Transfer-based Attacks
- Surrogate Model Attacks
- Query-based Attacks (e.g., ZOO, Boundary Attack)

### Physical World Attacks
- Adversarial Patch
- Lighting/Noise Perturbations (e.g., AdvCam)

### Tools & Libraries Practice
- Implement FGSM/PGD using PyTorch or TensorFlow.
- Utilize libraries such as Foolbox and ART (Adversarial Robustness Toolbox).

## Adversarial Defense Techniques
### Robust Training Methods
- Adversarial Training
- TRADES (TRadeoff-inspired Adversarial DEfense via Surrogate-loss minimization)
- Data Augmentation (e.g., Gaussian Noise, Mixup)

### Input Preprocessing
- Randomization
- Feature Compression (e.g., JPEG Compression, Denoising)

### Model Architecture Improvements
- Robust Loss Functions (e.g., MART)
- Gradient Masking
- Certified Defenses

### Evaluation Metrics
- Robust Accuracy
- Perturbation Magnitude (using L0, L2, and L∞ norms)


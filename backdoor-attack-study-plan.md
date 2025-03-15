1. [ ] Core Concepts (1-2 Weeks)
    - Backdoor attack definition & objectives
    - Trigger design: Explicit (fixed patterns) vs. Implicit (natural features, frequency domain perturbations)
    - Poisoned Data vs. Clean-Label Attack
    - Poisoning rate vs. attack success rate relationship
    - Attack scenario classification:
        - Data Poisoning
        - Model Supply Chain Attack
        - Data-Free Backdoor
    - Key metrics:
        - Attack Success Rate (ASR)
        - Benign Accuracy (BA)
        - Trigger stealth (PSNR/SSIM)

2. [ ] Classical Backdoor Attack Methods (2-3 Weeks)
    - Basic attack methods:
        - BadNets (label flipping-based injection)
        - Blended Attack (blended triggers)
        - Clean-Label Attack (stealthy, no label modification)
    - Advanced attack variants:
        - Dynamic Backdoor (adaptive triggers)
        - Invisible Backdoor (frequency-domain hiding via DCT/wavelet transforms)
        - Physical Backdoor (real-world triggers such as stickers or 3D objects)
    - Emerging directions:
        - Distributed backdoor in federated learning
        - Multimodal backdoor (e.g., image + text triggers)
        - Conditional trigger backdoor (activates in specific scenarios)

3. [ ] Practice (2-3 Weeks)
    - Reproduce BadNets on MNIST/CIFAR-10 using PyTorch
    - Implement Blended Attack (using blended random noise as trigger)
    - Tools & libraries:
        - Use TrojanZoo to build the backdoor attack pipeline
        - Utilize BackdoorBench to evaluate attack performance
    - Advanced experiments:
        - Design frequency-domain invisible triggers (e.g., using DCT transforms)
        - Attack pre-trained models (e.g., ResNet, ViT)

4. [ ] Backdoor Defense Techniques (2-3 Weeks)
    - Training-time defenses:
        - Data sanitization (anomaly detection: KNN, clustering)
        - Robust training methods (e.g., STRIP)
    - Inference-time defenses:
        - Neural Cleanse (reverse-engineering triggers)
        - SentiNet (saliency-based localization of suspicious regions)
    - Post-hoc analysis:
        - Activation clustering (e.g., ABS)
        - Model fingerprint verification
    - Evaluation metrics:
        - Reduction in ASR
        - Changes in BA
        - Computational overhead

## Study Resources

### Key Papers
* https://arxiv.org/abs/1708.06733
* https://www.ndss-symposium.org/wp-content/uploads/2018/02/ndss2018_03A-5_Liu_paper.pdf)

### Blog & Slides

* https://www.cobalt.io/blog/backdoor-attacks-on-ai-models

### ToolBox & Code Repositories
* https://github.com/ain-soph/trojanzoo
* https://github.com/SCLBD/BackdoorBench

### Awesome Repos
* https://github.com/awesome-backdoor-attacks



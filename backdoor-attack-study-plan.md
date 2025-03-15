# Backdoor Attack Study Plan

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

## Study Resources for Backdoor Attacks

### Key Papers
- **BadNets: Identifying Vulnerabilities in the Machine Learning Supply Chain (Gu et al., 2017)**  
  [arXiv](https://arxiv.org/abs/1708.06733)
- **Trojaning Attack on Neural Networks (Liu et al., 2018)**  
  [arXiv](https://arxiv.org/abs/1802.05502)
- **Hidden Trigger Backdoor Attack (Saha et al., 2020)**  
  [arXiv](https://arxiv.org/abs/2007.04697)

### Blog & Slides
- **Backdoor Attacks on Deep Neural Networks**  
  A detailed article explaining various backdoor attack techniques and defenses.  
  [Towards Data Science Article](https://towardsdatascience.com/backdoor-attacks-on-deep-neural-networks-f3ea736b51d9)
- **Backdoor Attacks on Deep Learning Systems (Slide Deck)**  
  A slide deck presentation on backdoor attacks in neural networks.  
  [SlideShare Presentation](https://www.slideshare.net/harshajain07/backdoor-attacks-on-deep-learning-systems)

### ToolBox & Code Repositories
- **TrojanZoo**  
  A collection of backdoor attack implementations and experiments.  
  [GitHub Repository](https://github.com/AI-secure/TrojanZoo)
- **BackdoorBench**  
  A benchmark for evaluating backdoor attacks and defenses.  
  [GitHub Repository](https://github.com/eth-sri/backdoorbench)
- **Adversarial Attacks PyTorch**  
  Contains various adversarial attack implementations, including backdoor methods.  
  [GitHub Repository](https://github.com/Harry24k/adversarial-attacks-pytorch)

### Datasets & Competitions
- **TrojAI Dataset & Competition**  
  An initiative by NIST for evaluating trojan/backdoor attacks.  
  [NIST TrojAI](https://www.nist.gov/itl/iad/mig/trojai)

### Awesome Repos
- **Awesome ML Security**  
  A curated list of resources on machine learning security, including backdoor attacks.  
  [GitHub Repository](https://github.com/AI-secure/awesome-ml-security)




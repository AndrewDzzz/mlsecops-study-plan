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

## Study Resources for AI Fairness

### Key Papers
- **Fairness Through Awareness**  
  Dwork, C., Hardt, M., Pitassi, T., Reingold, O., & Zemel, R. (2012). *Fairness Through Awareness.*  
  [ACM Digital Library](https://dl.acm.org/doi/10.1145/2090236.2090255)
  
- **Equality of Opportunity in Supervised Learning**  
  Hardt, M., Price, E., & Srebro, N. (2016). *Equality of Opportunity in Supervised Learning.*  
  [NeurIPS Paper](https://papers.nips.cc/paper/7159-equality-of-opportunity-in-supervised-learning)
  
- **A Survey on Bias and Fairness in Machine Learning**  
  Mehrabi, N., Morstatter, F., Saxena, N., Lerman, K., & Galstyan, A. (2019).  
  [arXiv](https://arxiv.org/abs/1908.09635)
  
- **The Mythos of Model Interpretability**  
  Lipton, Z. C. (2016). *The Mythos of Model Interpretability.*  
  [arXiv](https://arxiv.org/abs/1606.03490)

### Blog & Slides
- **IBM AI Fairness 360 Blog**  
  Explore tutorials, case studies, and best practices for mitigating bias in AI with IBM’s toolkit.  
  [IBM Blog](https://www.ibm.com/blogs/research/tag/ai-fairness-360/)
  
- **Google's What-If Tool: Fairness & Interpretability**  
  A detailed walkthrough and slides on using the What-If Tool for fairness evaluation in machine learning.  
  [What-If Tool](https://pair.withgoogle.com/what-if-tool/)
  
- **Tutorial on Fairness, Accountability, and Transparency in Machine Learning**  
  *(Placeholder – replace with a current, relevant slide deck URL)*

### ToolBox
- **IBM AI Fairness 360 (AIF360)**  
  An open-source toolkit to help detect and mitigate bias in machine learning models.  
  [GitHub](https://github.com/IBM/AIF360)
  
- **Fairlearn**  
  A toolkit to assess and improve the fairness of machine learning models.  
  [GitHub](https://github.com/fairlearn/fairlearn)
  
- **The What-If Tool**  
  An interactive visual interface for model analysis and fairness evaluation.  
  [GitHub](https://github.com/pair-code/what-if-tool)
  
- **Aequitas**  
  A bias and fairness audit toolkit for predictive models.  
  [GitHub](https://github.com/dssg/aequitas)

### Awesome Repos
- **Awesome Fairness in Machine Learning**  
  A curated list of resources on fairness in machine learning.  
  [GitHub](https://github.com/zhangyx-ustc/Awesome-Fairness-in-Machine-Learning)
  
- **Awesome Responsible AI**  
  A curated repository of resources covering ethics, fairness, and accountability in AI.  
  [GitHub](https://github.com/Responsible-AI/awesome-responsible-ai)



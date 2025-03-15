# ML Supply Chain Attack Study Plan

## 1. Core Concepts (1-2 Weeks)
- [ ] **Introduction to ML Supply Chain Attacks**
  - Define ML supply chain attacks and their impact on data, model integrity, and overall system security.
  - Identify vulnerabilities in the ML lifecycle (e.g., data poisoning, model tampering, compromised dependencies).
- [ ] **Key Terminology and Frameworks**
  - Understand concepts such as data poisoning, backdoor attacks, third-party model dependencies, and supply chain integrity.
  - Review the typical stages of an ML pipeline where vulnerabilities can be introduced.

## 2. Attack Techniques and Case Studies (2-3 Weeks)
- [ ] **Common Attack Methods**
  - Study data poisoning techniques: how malicious data can be injected into training sets.
  - Explore model tampering and backdoor insertion during the training process.
  - Learn about attacks targeting third-party dependencies (e.g., pre-trained models, external libraries).
- [ ] **Case Studies and Real-World Examples**
  - Analyze documented cases (e.g., BadNets, Trojan attacks) to understand attack vectors and outcomes.
  - Review academic papers and industry reports detailing ML supply chain vulnerabilities.

## 3. Practical Experiments (2-3 Weeks)
- [ ] **Experimentation Environment Setup**
  - Build a controlled ML pipeline using open-source tools and datasets (e.g., MNIST, CIFAR-10).
  - Reproduce simple attack scenarios such as data poisoning and model tampering.
- [ ] **Implementation and Testing**
  - Implement basic attack techniques to observe their effect on model performance.
  - Experiment with detection and mitigation strategies to evaluate their effectiveness.

## 4. Defense and Mitigation Strategies (2-3 Weeks)
- [ ] **Preventive Measures**
  - Learn about secure data validation, model verification, and dependency management practices.
  - Explore tools like DVC (Data Version Control) and Sigstore to track and secure ML artifacts.
- [ ] **Detection and Response**
  - Study techniques for identifying anomalies in data pipelines and model outputs.
  - Evaluate methods for auditing model provenance to detect compromised components.

## 5. Extended Learning & Community Engagement (Ongoing)
- [ ] **Stay Updated with Research**
  - Follow recent publications, journals, and industry news on ML security and supply chain attacks.
  - Subscribe to relevant blogs, newsletters, and forums.
- [ ] **Collaborative Projects and Open-Source Engagement**
  - Contribute to or monitor open-source projects focusing on ML security.
  - Participate in community challenges and discussions to share insights and best practices.

## Study Resources for ML Supply Chain Attacks

### Key Papers
- **BadNets: Identifying Vulnerabilities in the Machine Learning Supply Chain (Gu et al., 2017)**  
  [arXiv](https://arxiv.org/abs/1708.06733)
- **Trojaning Attack on Neural Networks (Liu et al., 2018)**  
  [arXiv](https://arxiv.org/abs/1802.05502)
- **Hidden Trigger Backdoor Attack (Saha et al., 2020)**  
  [arXiv](https://arxiv.org/abs/2007.04697)

### Blog & Slides
- **Securing the Machine Learning Supply Chain**  
  An article discussing the vulnerabilities and defenses in the ML supply chain.  
  [IBM Security Blog](https://www.ibm.com/blogs/security/ai-model-security-supply-chain/)
- **ML Supply Chain Attacks Explained (Slide Deck)**  
  Explore various aspects of ML supply chain attacks via this SlideShare search result.  
  [SlideShare Search Results](https://www.slideshare.net/search/slideshow?searchfrom=header&q=ml+supply+chain)

### ToolBox
- **DVC (Data Version Control)**  
  A tool for managing data, models, and experiments to ensure traceability in ML projects.  
  [DVC Website](https://dvc.org/)
- **Sigstore**  
  A suite of tools for signing, verifying, and protecting software artifacts, including ML models.  
  [Sigstore Website](https://sigstore.dev/)
- **Model Card Toolkit**  
  A toolkit for creating model cards to document model details, intended use, and security considerations.  
  [GitHub - Model Card Toolkit](https://github.com/google/model-card-toolkit)

### Awesome Repos
- **Awesome ML Security**  
  A curated list of resources on machine learning security, covering various attack vectors including supply chain attacks.  
  [GitHub - Awesome ML Security](https://github.com/AI-secure/awesome-ml-security)

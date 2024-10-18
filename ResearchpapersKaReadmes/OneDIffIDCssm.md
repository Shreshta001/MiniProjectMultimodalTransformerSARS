# OneDiff: A Generalist Model for Image Difference Captioning 🖼️✨

## Problem Statement
The research addresses the challenge of **Image Difference Captioning (IDC)**, which aims to accurately describe variations between closely related images. Traditional IDC methods often rely on specialized models, limiting their practical use. This study introduces **OneDiff**, a generalist model designed to effectively capture and articulate fine-grained differences in images.

## Methodology 🛠️
### Model Architecture
- **Siamese Image Encoder**: Processes two images independently and combines their features to identify differences.
- **Visual Delta Module**: Uses learnable query tokens to probe multi-level encoded features, enhancing the detection of subtle variations.

### Training Strategy
- **Coupled Sample Training**: Combines image pairs into pseudo dual-image samples to learn complex relationships.
- **Multi-task Learning**: Trains on a diverse array of IDC datasets for better generalization.

### Dataset Creation
The **DiffCap Dataset** was developed, including real-world and synthetic data, augmented with techniques like image retrieval and synthetic image generation.

## Implementation 💻
1. **Data Collection**: Gathered existing IDC datasets (e.g., Spot-the-Diff, CLEVR-Change) and added real images.
2. **Annotation Process**: Generated captions using large language models (LLMs) like ChatGPT to describe image differences.
3. **Training**: OneDiff was trained on the DiffCap Dataset using the dual-phase strategy.
4. **Testing and Evaluation**: Evaluated on various IDC benchmarks for accuracy and adaptability.

## Objective 🎯
To develop a robust, generalist model for IDC that can describe visual discrepancies across a wide range of scenarios without being limited to specific contexts.

## Conclusion 🏆
OneDiff sets a new benchmark in IDC by:
- Achieving superior performance across multiple IDC tasks.
- Providing a flexible framework adaptable for fields like medical diagnostics and surveillance.
- Demonstrating strong generalization without specific tuning, marking a significant advancement in the field.

## Results 📈
OneDiff significantly outperforms existing models, achieving up to **85% improvement in CIDEr scores** on average across various benchmarks, showcasing its robustness in detecting and describing visual differences effectively.

## References 📚
- Hua, E., Guo, L., Yue, T., Zhao, Z., Xue, S., & Liu, J. (2024). *OneDiff: A Generalist Model for Image Difference Captioning*. arXiv:2407.05645v2 [cs.CV].
- Datasets used: Spot-the-Diff, CLEVR-Change, Birds-to-Words, etc.
- Techniques using LLMs like ChatGPT were pivotal for generating high-quality difference captions.

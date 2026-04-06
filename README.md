 Eczema vs Scabies Classification using Deep Learning


 Overview

This project uses deep learning to distinguish between eczema and scabies– two visually similar skin conditions requiring different treatments.

Dataset

- Total images: 2,824
- Sources: 3 continents (Western, African, Indian populations)
  - DermNet (Western)
  - PASSION MICCAI 2024 (African)
  - DermaCon-IN (Indian)
- Classes: Eczema (1,425 images) , Scabies (1,399 images)
- Split: 2,555 training , 269 testing

 Architectures Tested

| Model | Type | Accuracy |
|-------|------|----------|
| ResNet-50 | CNN | 94% |
| ConvNeXt-Tiny | CNN | 91% |
| EfficientNet-B0 | CNN | 87% |
| DeiT-Tiny | Transformer | 89% |
| ViT-B/16 | Transformer | 74% |

Best model: ResNet-50 with 94% accuracy

## Explainability

Grad-CAM++ visualizations confirmed the model focuses on:
- Eczema: Inflamed, erythematous regions
- Scabies: Interdigital web spaces (classic burrow locations)

## Repository Structure


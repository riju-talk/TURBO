# TURBO: Target-Augmented Shared Fusion-based Multimodal Sarcasm Explanation

## Overview

An independent implementation of the paper:  
[Target-Augmented Shared Fusion-based Multimodal Sarcasm Explanation Generation](https://arxiv.org/pdf/2502.07391)  
by Palaash Goel, Dushyant Singh Chauhan, and Md Shad Akhtar.

TURBO enhances multimodal sarcasm explanation by detecting sarcasm, identifying targets, and fusing text and image inputs.

## Contents of `turbo.ipynb`

1. **Data Preparation**  
   - Loads MORE+ dataset (sarcastic posts, explanations).  
   - Processes text captions, image features, and sarcasm targets.  

2. **Core Architecture**  
   - Modified BART encoder.  
   - Cross-attention for text-image fusion.  
   - Sarcasm-target-aware representation.  
   - Uses Vision Transformer (ViT) or object detection scores.  

3. **Training Pipeline**  
   - Splits data into train/validation.  
   - Applies sequence generation loss.  
   - Trains with teacher forcing.  
   - Logs loss and metrics.  

4. **Evaluation System**  
   - Tests with BLEU, ROUGE, METEOR scores.  
   - Visualizes explanations and targets.  
   - Analyzes correct/incorrect outputs.  

## Installation

### Requirements  
- Python 3.8+  
- PyTorch >= 1.10  
- Transformers (HuggingFace)  
- Jupyter Notebook  
- See `requirements.txt` for more.  

### Setup  
```bash
git clone https://github.com/yourusername/TURBO-MuSE.git
cd TURBO-MuSE
pip install -r requirements.txt
jupyter notebook turbo.ipynb
```

## Dataset  
Uses the MORE+ dataset, an extension of MORE with sarcasm targets.  
Refer to the paper for access or format details.

## Citation  
```bibtex
@article{goel2025turbo,
  title={Target-Augmented Shared Fusion-based Multimodal Sarcasm Explanation Generation},
  author={Goel, Palaash and Chauhan, Dushyant Singh and Akhtar, Md Shad},
  journal={arXiv preprint arXiv:2502.07391},
  year={2025}
}
```

## Acknowledgments  
A research-grade reimplementation. Thanks to the original authors for the concept.
# MSBD5002_project
This project implements the Cascaded Cross Attention (CCA) model for review-based sequential recommendation. The model integrates user-item interaction sequences with review texts to learn richer user and item representations. It uses a multi-layer attention mechanism to align and combine semantic features from reviews and sequence dynamics for better recommendation performance.

The implementation is based on PyTorch and supports both training and evaluation pipelines.

## Dependencies
Python 3.8+

PyTorch 1.10+

NumPy

tqdm

scikit-learn

pandas

## Data prepare
Place the dataset files (e.g., Amazon, Yelp) under the dataset/ directory. Make sure to preprocess them into sequences and review features if not already done.

## File Discription
Data_prepare.ipynb: Processes raw interaction and review data. Constructs user/item sequences and review embeddings suitable for training.
My_CCA: Defines and trains the CCA model, evaluates it on the prepared dataset, and prints out key metrics such as Hit@10 and NDCG@10.

## Tips
If you use this code, please cite the original paper:
@INPROCEEDINGS{10415676,
  author={Huang, Bingsen and Luo, Jinwei and Du, Weihao and Pan, Weike and Ming, Zhong},
  booktitle={2023 IEEE International Conference on Data Mining (ICDM)},
  title={Cascaded Cross Attention for Review-based Sequential Recommendation},
  year={2023},
  pages={170-179},
  doi={10.1109/ICDM58522.2023.00026}
}

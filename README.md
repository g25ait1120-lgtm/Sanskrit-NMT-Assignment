# Sanskrit-to-English Neural Machine Translation Project

This project implements a Neural Machine Translation (NMT) system for translating Sanskrit to English using a Sequence-to-Sequence (Seq2Seq) architecture with Attention.

## Key Components:
- **Data Loading and Preprocessing**: Handles parallel Sanskrit-English datasets.
- **Model Architecture**: Encoder-Decoder with GRU units and a Bahdanau-style Attention mechanism.
- **Training**: Utilizes Adam optimizer and Cross-Entropy Loss.
- **Inference**: Employs Beam Search decoding for improved translation quality.
- **Evaluation**: Metrics include BLEU and BERTScore for assessing translation performance.

## Setup:
1. Mount Google Drive to access datasets.
2. Install necessary Python libraries (torch, torchtext, sacrebleu, bert-score, tqdm).
3. Ensure datasets (`train_sa_10000.csv`, `train_en_10000.csv`, `dev_sa_1000.csv`, `dev_en_1000.csv`, `test_sa_1000.csv`, `test_en_1000.csv`) are placed in `'/content/drive/MyDrive/NLU_30062026'`.

## Usage:
Run the notebook cells sequentially to:
- Load and preprocess data.
- Train the Seq2Seq model.
- Evaluate the model on test sets.
- Generate a `submission.csv` file with predictions.
- Evaluate performance on a new dataset (if provided).


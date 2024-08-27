# English-French Translation with Transformers from scratch

This project implements a Transformer-based model for English to French translation using PyTorch. It includes data preprocessing, model implementation, and training pipeline.

## Features

- Custom implementation of Transformer architecture
- Data preprocessing for English-French translation dataset
- Configurable model architecture (number of heads, layers, etc.)
- Training and evaluation pipeline

## Requirements

- Python 3.7+
- PyTorch
- pandas
- scikit-learn
- openpyxl (for reading Excel files)

For a complete list of requirements, see `requirements.txt`.

## Installation

1. Clone this repository

2. Install the required packages:
pip install -r requirements.txt

## Usage

1. Prepare your data:
- Ensure you have an Excel file named `eng_-french.xlsx` with columns 'English words/sentences' and 'French words/sentences'
- Place this file in the same directory as the script

2. Run the script:
   python translation_transformers.py

3. The script will:
- Load and preprocess the data
- Build vocabularies for English and French
- Train multiple Transformer models with different configurations
- Evaluate the models and display sample predictions

## Model Architecture

The Transformer model includes:

- Embedding Layer
- Positional Encoding
- Multi-Head Attention
- Feed-Forward Networks
- Layer Normalization
- Encoder and Decoder stacks

## Customization

You can adjust various hyperparameters in the script:

- `embedding_dim`: Dimension of word embeddings
- `d_ff`: Dimension of feed-forward network
- `num_heads`: Number of attention heads
- `num_layers`: Number of encoder/decoder layers
- `max_len`: Maximum sequence length
- `num_epochs`: Number of training epochs
- `learning_rate`: Learning rate for optimizer

## Results

The script trains and evaluates multiple model configurations, displaying training loss, validation loss, and sample predictions for each configuration.


# Stock Prediction Using Fine-Tuned LLaMA-3.1 Model

This repository contains a project that uses a fine-tuned [LLaMA-3.1](https://huggingface.co/meta-llama/Llama-3.1-8B-Instruct) model for generating stock market movement predictions based on historical stock data and news articles. The system processes news content, evaluates market conditions, and provides quantitative predictions of stock price changes.

---

## Features

- **Quantitative Predictions**: Provides specific stock movement predictions within a percentage range (e.g., "up by 2-4%").
- **Reasoning Generation**: Summarizes the reasoning based on company performance, market trends, and external factors.
- **Dynamic Prompting**: Uses a static task prompt alongside custom inputs for tailored predictions.
- **Fine-Tuning**: Leverages fine-tuning via [BitsAndBytes](https://github.com/TimDettmers/bitsandbytes) for 4-bit quantization.
- **Batch Processing**: Automatically processes multiple CSV files containing prompts for predictions.

---

## Prerequisites

- Python 3.8+
- CUDA-enabled GPU for faster computations.
- Required libraries:
  - [Transformers](https://github.com/huggingface/transformers)
  - [BitsAndBytes](https://github.com/TimDettmers/bitsandbytes)
  - [Accelerate](https://github.com/huggingface/accelerate)
  - [PEFT](https://github.com/huggingface/peft)
  - [TRL](https://github.com/huggingface/trl)
  - [Datasets](https://github.com/huggingface/datasets)
  - [WandB](https://wandb.ai)

---

## Setup Instructions

1. **Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/stock-prediction-llama.git
   cd stock-prediction-llama

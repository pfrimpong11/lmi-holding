# (QLora) Fine-tuning Mistral-7b-Instruct to Respond to HR-Policy questions for LMI Holding

This notebook demonstrates how to fine-tune the Mistral-7b-Instruct model using QLora to answer questions related to HR policies specifically for LMI Holding.

## Description

The notebook covers the following steps:

1. **Installation:** Installing necessary libraries like `auto-gptq`, `optimum`, and `bitsandbytes`.
2. **Model Loading:** Loading the pre-trained Mistral-7B-Instruct-v0.2-GPTQ model and tokenizer.
3. **Base Model Usage:** Demonstrating the usage of the base model for inference.
4. **Training Preparation:** Preparing the model for training using gradient checkpointing and quantization.
5. **LoRA Configuration:** Setting up the LoRA configuration for efficient fine-tuning.
6. **Dataset Loading:** Loading a custom dataset in JSONL format and splitting it into train, validation, and test sets.
7. **Data Preprocessing:** Formatting and tokenizing the dataset for model training.
8. **Fine-tuning:** Fine-tuning the model using the Hugging Face Trainer.
9. **Model Pushing:** Pushing the fine-tuned model and tokenizer to the Hugging Face Hub.
10. **Fine-tuned Model Loading:** Loading the fine-tuned model from the Hugging Face Hub.
11. **Fine-tuned Model Usage:** Demonstrating the usage of the fine-tuned model for inference.

## Requirements

- Python 3.8 or higher
- PyTorch 2.0 or higher
- Transformers
- PEFT
- Datasets
- Accelerate
- Auto-GPTQ
- Optimum
- Bitsandbytes

## Usage

1. Clone this repository.
2. Install the required libraries using `pip install -r requirements.txt`.
3. Upload your custom dataset in JSONL format to the `sample_data` directory.
4. Run the notebook cells sequentially.
5. Replace `"pfrimpong"` with your Hugging Face username in the `hf_name` variable.

## Acknowledgements

- TheBloke for the Mistral-7B-Instruct-v0.2-GPTQ model.
- Hugging Face for the Transformers and Datasets libraries.
- Microsoft for the LoRA technique.

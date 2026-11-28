
# WEEK 7 – Next-Token Probability Analysis using GPT-2

## Aim

To inspect next-token probabilities by analyzing logits and top-K candidate tokens using GPT-2 with Hugging Face Transformers.

## Technologies Used

- Python
- PyTorch
- Hugging Face Transformers
- GPT-2
- CSV

## Tools Used

- Python
- Visual Studio Code
- Hugging Face

## Folder Structure
```text
WEEK7/
├── main.py
├── requirements.txt
└── week7_probability_results.csv
```

## Installation Steps

1. Install Python on your system.
2. Open the WEEK7 folder in VS Code.
3. Install the required packages:
```bash
pip install -r requirements.txt
```
4. Add the following packages in `requirements.txt`:
```text
torch
transformers
```

## Execution Steps

Run the following command in the terminal:
```bash
python main.py
```

1. Load the GPT-2 pretrained language model.
2. Define four input prompts.
3. Convert prompts into token IDs using the tokenizer.
4. Extract logits for the next-token prediction.
5. Apply softmax to convert logits into probabilities.
6. Identify the top-5 next-token candidates.
7. Display token IDs, candidate tokens, and probabilities.
8. Save the results into a CSV file.

## Expected Output

The program displays:

- GPT-2 model loading status.
- Input prompts and token IDs.
- Top-5 next-token candidates.
- Candidate token IDs.
- Next-token probabilities.
- CSV file creation confirmation.

## Output Files

- `week7_probability_results.csv` – Stores prompts, candidate tokens, token IDs, ranks, and probabilities.

## Result

Successfully analyzed next-token probabilities using GPT-2 and Hugging Face Transformers by inspecting logits, applying softmax, identifying top-5 candidate tokens, and saving the results in a CSV file.

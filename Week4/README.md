WEEK 4 – Tokenizer Comparison Lab

1. Aim

To compare different tokenization techniques used in Large Language Models (LLMs) by processing English, Telugu, and Hindi sentences using BPE, WordPiece, and SentencePiece-based tokenizers.

2. Technologies Used

Python

VS Code

GPT-2

3. Tokenizers Used

BPE: GPT-2 (gpt2)

WordPiece: Multilingual BERT (bert-base-multilingual-cased)

SentencePiece: XLM-R (xlm-roberta-base)

4. Installation

Install the required packages:

pip install transformers sentencepiece

Or execute:

pip install -r requirements.txt

5. Input Languages

The experiment uses three languages:

English

Telugu

Hindi

6. Implementation Steps

Import the AutoTokenizer class from Transformers.

Load the GPT-2 tokenizer.

Load the Multilingual BERT tokenizer.

Load the XLM-R tokenizer.

Provide sample sentences in English, Telugu, and Hindi.

Convert sentences into tokens.

Generate corresponding token IDs.

Calculate the total number of tokens.

Compare the results of all three tokenizers.

7. Execution

Open the Week-4 project folder in VS Code and execute:

python tokenizer_comparison.py

8. Sample Input

English:

Artificial intelligence is changing the world.

Telugu:

కృత్రిమ మేధస్సు ప్రపంచాన్ని మారుస్తోంది.

Hindi:

कृत्रिम बुद्धिमत्ता दुनिया को बदल रही है।

9. Sample Output

Language

BPE (GPT-2)

WordPiece (BERT)

SentencePiece (XLM-R)

English

8

10

10

Telugu

112

18

14

Hindi

68

17

14

Sample token counts from the recorded practical execution, including special tokens.

10. Observations

GPT-2 generated fewer tokens for the given English sentence.

GPT-2 generated more tokens for Telugu and Hindi.

Multilingual BERT and XLM-R generated fewer tokens for the given Telugu and Hindi sentences.

Different tokenizers produce different token counts depending on their vocabulary and tokenization approach.

11. Result

Successfully implemented and compared BPE, WordPiece, and SentencePiece-based tokenizers using Python and Hugging Face Transformers. Observed how different tokenization techniques process English, Telugu, and Hindi text and produce different token counts.

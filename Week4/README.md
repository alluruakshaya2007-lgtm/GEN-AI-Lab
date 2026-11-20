📌 Project Overview

This project demonstrates how different tokenization techniques used in Large Language Models (LLMs) process text in multiple languages.

The objective of this practical is to compare three tokenization approaches: Byte Pair Encoding (BPE), WordPiece, and SentencePiece using Python and the Hugging Face Transformers library.

The experiment analyzes how English, Telugu, and Hindi sentences are divided into tokens and converted into token IDs.



🎯 Objectives

Understand the concept of tokenization in Large Language Models.

Explore different tokenization techniques.

Compare BPE, WordPiece, and SentencePiece tokenizers.

Perform tokenization using Python and Hugging Face Transformers.

Analyze token counts for English, Telugu, and Hindi.

Understand how tokenization differs across languages.



🛠️ Technologies Used

Python

Hugging Face Transformers

SentencePiece

VS Code

PowerShell



📂 Project Structure

Week-4/
│
├── tokenizer_comparison.py
├── requirements.txt
└── README.md



⚙️ Setup and Installation

Step 1: Open the Project

Open the Week-4 project folder in Visual Studio Code.

Step 2: Activate the Virtual Environment

Open the VS Code terminal and execute:

..\.MyEnv\Scripts\Activate.ps1

Step 3: Install Required Packages

Execute the following command:

pip install -r requirements.txt

The requirements.txt file contains:

transformers

sentencepiece

Step 4: Import Required Library

Import the AutoTokenizer class:

from transformers import AutoTokenizer

Step 5: Load Different Tokenizers

Three tokenizers are used in this practical:

BPE – GPT-2 (gpt2)

WordPiece – Multilingual BERT (bert-base-multilingual-cased)

SentencePiece – XLM-R (xlm-roberta-base)

Step 6: Provide Input Sentences

The following sentences are used for tokenization:

English:

Artificial intelligence is changing the world.

Telugu:

కృత్రిమ మేధస్సు ప్రపంచాన్ని మారుస్తోంది.

Hindi:

कृत्रिम बुद्धिमत्ता दुनिया को बदल रही है।

Step 7: Execute the Python Program

Run the following command in the terminal:

python tokenizer_comparison.py

The program displays the tokens, token IDs, and total token count for each tokenizer and language.


🧪 Three Tokenization Experiments

The following experiments compare how different tokenizers process sentences in multiple languages.

Experiment 1: BPE – GPT-2

Tokenizer: GPT-2

Objective: Understand how Byte Pair Encoding divides text into smaller subword units.

Experiment 2: WordPiece – Multilingual BERT

Tokenizer: Multilingual BERT

Objective: Understand how WordPiece tokenization processes English and multilingual text.

Experiment 3: SentencePiece – XLM-R

Tokenizer: XLM-R

Objective: Understand how SentencePiece-based tokenization handles different languages.



🔍 Observations

GPT-2 generated fewer tokens for the given English sentence.

GPT-2 generated significantly more tokens for Telugu and Hindi.

Multilingual BERT and XLM-R handled the given Telugu and Hindi sentences with fewer tokens.

Different tokenizers produce different token counts because of their vocabularies and tokenization methods.

Token count can affect the input length and token usage of LLM applications.

🔄 Execution Workflow

The complete execution process follows these steps:

Import the required Python library.

Load the three pretrained tokenizers.

Provide English, Telugu, and Hindi sentences.

Pass each sentence to the tokenizers.

Generate tokens and corresponding token IDs.

Calculate the total number of tokens.

Compare the results across different tokenizers.

📚 Learning Outcomes

After completing this practical, I learned:

The importance of tokenization in Large Language Models.

How BPE, WordPiece, and SentencePiece-based tokenizers work.

How to use pretrained tokenizers through Hugging Face Transformers.

How text is converted into tokens and token IDs.

How tokenization differs between English and Indian languages.

How token counts influence text processing in LLM applications.

How to compare different tokenization techniques using Python.

✅ Conclusion

This practical helped me understand and compare three different tokenization approaches. The experiment demonstrated that tokenization varies across languages and models, highlighting the importance of choosing suitable tokenizers for multilingual LLM applications.

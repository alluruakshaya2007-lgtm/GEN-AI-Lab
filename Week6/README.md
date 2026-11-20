📌 Project Overview

This project demonstrates how to evaluate a Large Language Model (LLM) using a predefined Golden Question Set and Ollama with the Llama 3.2 model.

The objective is to test the model's responses against expected answers using keyword-based evaluation and generate a baseline evaluation report.

This practical establishes the first evaluation version, Release v0.1.

🎯 Objectives

Create a Golden Question Set containing 30 questions.

Run the Llama 3.2 model locally using Ollama.

Send questions to the LLM and collect generated responses.

Compare generated responses with expected answers.

Calculate keyword matching scores.

Classify results as PASS, REVIEW, or ERROR.

Export evaluation results into a CSV file.

Establish the baseline evaluation as Release v0.1.

🛠️ Technologies Used

Python

Ollama

Llama 3.2

JSON

CSV

Requests Library

Visual Studio Code

📂 Project Structure

Week-6/
│
├── main.py
├── golden_set.json
├── requirements.txt
├── baseline_results.csv
└── README.md

⚙️ Installation and Setup

1. Install Ollama

Download and install Ollama from:

https://ollama.com/

2. Download the Llama 3.2 Model

ollama pull llama3.2

3. Install Python Dependencies

pip install -r requirements.txt

4. Run the Evaluation Program

python main.py

📋 Golden Question Set

The project contains 30 questions (Q001–Q030) covering topics such as:

Tokenization and Tokens

Byte Pair Encoding (BPE)

WordPiece and SentencePiece

Token Economics

Input and Output Tokens

Context Windows

API Rate Limits

Autoregressive Generation

Next-Token Prediction

Probability Distribution

Greedy Decoding and Sampling

Temperature, Top-K and Top-P

Embeddings and Token IDs

Positional Encodings

Rotary Position Embeddings (RoPE)

Transformer Architecture

📊 Evaluation Methodology

The program evaluates each generated response using keyword matching.

Keyword Matching Score:

Score = (Matched Keywords / Total Keywords) × 100

Result Classification

Status

Description

PASS

Keyword matching score is 60% or higher

REVIEW

Keyword matching score is below 60%

ERROR

An exception or request failure occurred

📁 Output

The evaluation results are saved in:

baseline_results.csv

The CSV report contains:

Question ID

Question

Expected Answer

LLM Generated Answer

Matched Keywords

Missing Keywords

Evaluation Score

Status

Source

Model Name

Release Version

✅ Final Result

The baseline evaluation was executed successfully using the Llama 3.2 model.

BASELINE RUN COMPLETED!

Release v0.1 created successfully.

Release: v0.1

Model: Llama 3.2

Total Questions: 30

Evaluation Type: Keyword-Based Evaluation

🎓 Conclusion

This practical helped demonstrate how to evaluate LLM-generated responses using a Golden Question Set. It provided hands-on experience with local LLM execution, automated response evaluation, keyword matching, and CSV report generation.

The successful baseline run established Release v0.1, which can be used as a reference for future model evaluation and comparison.

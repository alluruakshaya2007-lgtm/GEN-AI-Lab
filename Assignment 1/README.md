📌 Project Overview

This project demonstrates two popular tokenization techniques used in Natural Language Processing (NLP) and Large Language Models (LLMs): Byte Pair Encoding (BPE) and WordPiece Tokenization.

The objective is to understand how text is divided into smaller tokens, calculate adjacent pair frequencies, perform token merging, and compare frequency-based and score-based tokenization approaches using Python.

🎯 Objectives

Understand Byte Pair Encoding (BPE).

Understand WordPiece Tokenization.

Split words into individual character tokens.

Identify adjacent character pairs.

Calculate the frequency of each adjacent pair.

Merge the highest-frequency pair in BPE.

Update tokens after every merge.

Calculate WordPiece scores using the frequency formula.

Identify the highest-scoring pair.

🛠️ Technologies Used

Programming Language: Python

Libraries: collections (Counter, defaultdict)

Editor: VS Code

Platform: Windows

📂 Project Structure

BPE-WordPiece/
│
├── bpe.py
├── wordpiece.py
└── README.md

Input Words

Word and Frequency

LOW  5

LOWER  2

NEWEST  3

WILDEST  6


Working Process

Split each word into individual characters.

Identify all adjacent character pairs.

Calculate pair-wise frequencies using word frequencies.

Find the highest-frequency pair.

Merge the selected pair into a new token.

Display updated tokens.

Repeat the process for subsequent iterations.


Merge Operations

Iteration 1: e + s = es

Iteration 2: es + t = est

Iteration 3: l + o = lo

Iteration 4: lo + w = low



2. WordPiece Tokenization

WordPiece is a tokenization technique that selects adjacent token pairs based on their calculated scores.

Formula

Score of an adjacent pair:

[
Score(A,B)=
\frac{Freq(A,B)}
{Freq(A)\times Freq(B)}
]


▶️ How to Run the Project

Step 1: Install Python

Download and install Python from:

https://www.python.org/downloads/

Step 2: Open the Project Folder

Open the project folder in VS Code.

Step 3: Open Terminal

Open the VS Code terminal using:

Ctrl + `

Step 4: Run BPE

python bpe.py

Step 5: Run WordPiece

python wordpiece.py



📊 Expected Results

BPE Output

Initial character tokens.

Adjacent pair frequencies.

Pair-wise frequency calculations.

Highest-frequency pair.

Merge operations.

Updated tokens after every iteration.

Final token representation.


WordPiece Output

Individual character frequencies.

Adjacent pair frequencies.

WordPiece score calculations.

Highest-scoring adjacent pair.



📚 Conclusion

This practical demonstrates how BPE and WordPiece tokenization techniques process text into smaller tokens.

BPE identifies and merges the most frequently occurring adjacent pairs, while WordPiece calculates scores for adjacent pairs to identify the highest-scoring combination.

Through this implementation, we understand how tokenization works and why it is an important preprocessing step in NLP and Large Language Models (LLMs).
1. Byte Pair Encoding (BPE)

BPE is a tokenization technique that repeatedly merges the most frequently occurring adjacent character or token pairs.

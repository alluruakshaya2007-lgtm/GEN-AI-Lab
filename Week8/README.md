# WEEK 8 – Scaled Dot-Product Attention and Multi-Head Attention

## Aim

To implement Scaled Dot-Product Attention and Multi-Head Attention from scratch using PyTorch.

## Technologies Used

- Python
- PyTorch
- Deep Learning
- VS Code

## Tools Used

- Python
- Visual Studio Code
- PyTorch

## Folder Structure

```text
WEEK7/
├── main.py
├── requirements.txt
└── README.md
```

## Installation Steps

1. Install Python on your system.
2. Open the WEEK7 folder in VS Code.
3. Install the required packages:

```bash
pip install -r requirements.txt
```

4. Add the following package in `requirements.txt`:

```text
torch
```

## Execution Steps

Run the following command in the terminal:

```bash
python main.py
```

1. Create random Query (Q), Key (K), and Value (V) tensors.
2. Calculate Scaled Dot-Product Attention.
3. Apply softmax to generate attention weights.
4. Implement Multi-Head Attention using PyTorch.
5. Split Query, Key, and Value into multiple attention heads.
6. Combine the attention heads and generate the final output.
7. Display attention weights, output values, and tensor shapes.

## Expected Output

The program displays:

- Query, Key, and Value tensor shapes.
- Scaled Dot-Product Attention weights.
- Scaled Dot-Product Attention output.
- Number of attention heads.
- Multi-Head Attention weights shape.
- Multi-Head Attention output.
- Final output shape.

## Result

Successfully implemented Scaled Dot-Product Attention and Multi-Head Attention from scratch using PyTorch and verified their outputs and tensor dimensions.

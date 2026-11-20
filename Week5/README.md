📌 Project Overview

This project demonstrates Token Economics – Cost and Rate-Limit Budgeting Before Building an LLM Feature using Python.

The objective of this practical is to develop a budgeting tool that estimates token consumption, calculates API usage costs, checks provider rate limits, and determines whether a proposed LLM feature fits within the configured budget.

The project helps understand how to estimate the cost and resource requirements of an LLM-powered application before implementation.



🎯 Objectives

Understand input tokens, output tokens, and total tokens.

Calculate daily and monthly token consumption.

Estimate API costs using configurable input and output token prices.

Understand Requests Per Minute (RPM) and Tokens Per Minute (TPM).

Check API capacity against configured rate limits.

Apply safety margins to usage and cost estimates.

Set daily and monthly budget thresholds.

Perform what-if analysis to evaluate different usage scenarios.

Write automated tests to verify calculations.



🛠️ Technologies Used

Python

Visual Studio Code

Python-dotenv

Dataclasses

Unittest

PowerShell



📂 Project Structure

Week-5/
│
├── .env
├── budget.py
├── test_budget.py
├── requirements.txt
└── README.md


⚙️ Installation and Setup

1. Clone the Repository

git clone <your-repository-url>

2. Navigate to the Project Folder

cd Week-5

3. Create a Virtual Environment

python -m venv .venv

4. Activate the Virtual Environment

For Windows:

.venv\Scripts\activate

5. Install Dependencies

pip install -r requirements.txt




🚀 Execution

Run the Main Program

python budget.py

The program generates a Token Economics Report containing:

Input tokens per day

Output tokens per day

Total tokens per day

Estimated daily API cost

Estimated monthly API cost

Peak RPM with safety margin

Peak TPM with safety margin

Budget and capacity checks

Final recommendation

Run Automated Tests

python -m unittest test_budget.py -v




🧪 Automated Testing

The project includes four unit tests:

test_cost_estimate – Verifies daily and monthly cost calculations.

test_capacity_passes – Checks whether RPM and TPM limits are satisfied.

test_rpm_limit_fails – Verifies RPM limit failure.

test_monthly_budget_fails – Verifies monthly budget failure.

Expected Result:

Ran 4 tests

OK

All four automated tests passed successfully.



🔍 What-If Analysis

Different assumptions can be modified in the .env file to observe their impact.

Increasing requests per day increases token consumption and API costs.

Increasing input tokens increases input cost and TPM.

Increasing output tokens increases output cost and TPM.

Increasing peak requests per minute increases rate-limit pressure.

Reducing prompt size decreases input token consumption and cost.

Caching repeated content can reduce repeated model calls and token usage.




📚 Concepts Covered

Token Budgeting

Input and Output Token Estimation

API Cost Calculation

RPM and TPM Rate Limits

Safety Margin

Daily and Monthly Budget Management

Automated Unit Testing

What-If Analysis

Pre-build Go/No-Go Decision



✅ Expected Outcome

A reusable Python-based Token Economics Budget Planner that estimates token usage, calculates API costs, checks rate limits, and provides a go/no-go recommendation before building an LLM-powered feature.

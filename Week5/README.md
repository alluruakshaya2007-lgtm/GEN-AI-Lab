WEEK 5 – Token Economics

1. Aim

To estimate token consumption, API costs, and rate limits of an LLM-powered feature using Python before implementation.

2. Technologies Used

Python

Python-dotenv

Dataclasses

VS Code


4. Installation

pip install python-dotenv

5. Project Structure

Week-5/
├── .env
├── budget.py
├── test_budget.py
└── requirements.txt

6. Implementation Steps

Create a .env file to store configuration values.

Load environment variables using Python-dotenv.

Calculate daily and monthly token consumption.

Estimate API costs.

Check RPM and TPM limits.

Apply a safety margin.

Display the final budget report.

Perform automated testing and what-if analysis.

7. Execution

Run the main program:

python budget.py

Run automated tests:

python -m unittest test_budget.py -v

8. Sample Output

Input tokens/day:  2,400,000
Output tokens/day: 600,000
Total tokens/day:  3,000,000

Estimated daily cost:   $1.4400
Estimated monthly cost: $43.20

Peak RPM with margin: 36.0
Peak TPM with margin: 54000

RPM capacity: PASS
TPM capacity: PASS
Daily budget: PASS
Monthly budget: REVIEW

9. Observations

Increasing requests increases token consumption and cost.

Input and output tokens have different pricing.

RPM and TPM checks identify capacity limitations.

Safety margins help manage unexpected usage.

Budget checks identify possible cost overruns.

10. Result

Successfully implemented a Python-based Token Economics Budget Planner to calculate token consumption, estimate API costs, check rate limits, and evaluate budget limits. All four automated tests passed successfully.

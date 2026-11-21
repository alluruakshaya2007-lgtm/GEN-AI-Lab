WEEK 3 – LLM Monitoring with MongoDB

1. Aim

To monitor Gemini API calls by tracking token usage, response latency, estimated cost, and request status, and storing the records in MongoDB.

2. Technologies Used

Python

Google Gemini API

MongoDB Atlas

PyMongo

Pandas

Matplotlib

Google Colab

3. Database Structure

Database: llm_monitoring

Collection: api_usage

Stores input tokens, output tokens, total tokens, latency, estimated cost, status, timestamp, and error details.

4. Installation

Install required packages:

!pip install -q google-genai pymongo pandas matplotlib

5. Configuration

Configure the Gemini API key using Google Colab Secrets.

Create a MongoDB Atlas cluster.

Configure the MongoDB connection URI securely.

Never upload API keys or database credentials to GitHub.

6. Implementation Steps

Connect to the Gemini API.

Send prompts to the Gemini model.

Track input and output tokens.

Measure API response latency.

Estimate API request cost.

Log successful and failed API requests.

Store records in MongoDB.

Retrieve and analyze records using Pandas.

Calculate usage statistics using MongoDB aggregation.

Generate visualizations using Matplotlib.

7. Execution

Open the Week 3 notebook in Google Colab and execute all cells in order.

8. Sample Input

What is Artificial Intelligence?

9. Sample Output

Model: gemini-3.5-flash
Input Tokens: 4
Output Tokens: 571
Latency: 8.544 seconds
Estimated Cost: 0.0014287 USD
Status: success

Total API Attempts: 10
Successful Requests: 1
Failed Requests: 9

Sample values from the recorded practical execution.

10. Result

Successfully implemented an LLM monitoring system using Gemini API and MongoDB to track token consumption, response latency, estimated cost, and API request status.

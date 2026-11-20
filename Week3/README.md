Logging Tokens, Latency and Cost for Every Gemini API Call

Project Description

This project demonstrates how to monitor Large Language Model (LLM) API usage by logging token consumption, response latency, estimated 

API cost, and request status.

Google Gemini API is used to generate responses, while MongoDB stores the API usage records for monitoring and analysis.

Python libraries such as Pandas and Matplotlib are used to display, analyze, and visualize the collected monitoring data.



Objectives

Connect to the Google Gemini API using Python.

Generate responses using a Gemini model.

Track input tokens and output tokens.

Measure API response latency.

Estimate the API usage cost.

Record successful and failed API requests.

Store monitoring records in MongoDB.



Technologies Used

Python

Google Gemini API

Google GenAI SDK

MongoDB Atlas

PyMongo

Pandas

Matplotlib

Google Colab



Installation

Install the required Python libraries:

pip install google-genai pymongo pandas matplotlib


Configuration

The project requires:

A Google Gemini API key.

A MongoDB Atlas account.

A MongoDB connection URI.

A database and collection for storing API usage records.

Configure your API key and MongoDB connection URI securely using Google Colab Secrets or environment variables.

Important: Never upload API keys, MongoDB passwords, or connection strings containing credentials to GitHub.



Database Details

Database Name: llm_monitoring

Collection Name: api_usage



Project Workflow

Install the required Python libraries.

Configure the Gemini API key.

Connect to the Gemini API.

Send prompts to the Gemini model.

Capture token usage and response latency.

Estimate the API cost.

Handle successful and failed API requests.

Store monitoring records in MongoDB.

Retrieve records from the MongoDB collection.

Analyze API usage using Pandas.

Calculate total API usage using MongoDB aggregation.

Generate reports and charts using Matplotlib.


Sample Monitoring Output

The project records information such as:

Model: gemini-3.5-flash

Input Tokens: 4

Output Tokens: 571

Latency: 8.544 seconds

Estimated Cost: 0.0014287 USD

Status: success



MongoDB Verification

To verify that API records are stored in MongoDB, use MongoDB Shell:

use llm_monitoring

db.api_usage.find().pretty()

To count the stored records:

db.api_usage.countDocuments()

The records can also be viewed through MongoDB Atlas Data Explorer by opening:

llm_monitoring → api_usage



Expected Outcomes

Successful integration with the Gemini API.

Monitoring of input and output token usage.

Measurement of API response latency.

Estimation of API request costs.

Logging of successful and failed API requests.

Storage and retrieval of API monitoring records using MongoDB.

Analysis and visualization of API usage data.



Conclusion

This practical demonstrates an LLM monitoring system that tracks token consumption, latency, estimated cost, and request status for Gemini API calls. MongoDB provides persistent storage for monitoring records, while Pandas and Matplotlib help analyze and visualize API usage.

The project provides a foundation for understanding API performance, usage monitoring, and cost management in Generative AI applications.

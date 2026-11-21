📌 Project Overview

This project demonstrates how to monitor Large Language Model (LLM) API usage by tracking token consumption, response latency, estimated cost, and API request status.

The objective of this practical is to integrate the Google Gemini API with MongoDB using Python and store API monitoring information for every request.

The experiment analyzes successful and failed API attempts, retrieves stored records, calculates API usage statistics, and monitors token consumption and estimated costs.

🎯 Objectives

Understand the importance of monitoring Large Language Model applications.

Connect to the Google Gemini API using Python.

Track input and output token usage.

Measure API response latency.

Calculate estimated API usage costs.

Log successful and failed API requests.

Store API monitoring records in MongoDB.

Retrieve and analyze stored records.

Calculate total API usage using MongoDB aggregation.

Visualize monitoring data using Pandas and Matplotlib.

🛠️ Technologies Used

Python

Google Gemini API

MongoDB Atlas

Google Colab

📂 Project Structure

Week-3/

│

├── Week3_LLM_Monitoring.ipynb

└── README.md

⚙️ Setup and Installation

Step 1: Open the Project

Open the Week-3 practical notebook in Google Colab.

Step 2: Install Required Packages

Execute the following command:

!pip install -q google-genai pymongo pandas matplotlib

Step 3: Configure API Key

Generate a Google Gemini API key and configure it securely using Google Colab Secrets.

Step 4: Configure MongoDB Connection

Create a MongoDB Atlas cluster and configure the MongoDB connection URI.

Use PyMongo to establish a connection between Python and MongoDB.

Step 5: Connect to Gemini API

Initialize the Google GenAI client and select the Gemini model.

Step 6: Connect to MongoDB

Create a database and collection:

Database Name: llm_monitoring

Collection Name: api_usage

Step 7: Execute the Monitoring Program

Send prompts to the Gemini API and capture the following information:

Input tokens

Output tokens

Total tokens

Response latency

Estimated API cost

Request status

Error details

Store the monitoring information in MongoDB.

🧪 Monitoring Experiments

The following experiments are performed in this practical.

Experiment 1: Gemini API Integration

Objective: Connect to the Google Gemini API and generate AI responses using Python.

Experiment 2: Token Usage Monitoring

Objective: Track input tokens, output tokens, and total token consumption for API requests.

Experiment 3: Latency Monitoring

Objective: Measure the time taken by the Gemini API to generate responses.

Experiment 4: Cost Estimation

Objective: Estimate the API usage cost based on token consumption and applicable pricing.

Experiment 5: API Request Logging

Objective: Record both successful and failed API attempts in MongoDB.

Experiment 6: MongoDB Data Retrieval

Objective: Retrieve stored API monitoring records using PyMongo and display them using Pandas.

Experiment 7: Usage Analysis and Visualization

Objective: Calculate total API usage using MongoDB aggregation and analyze monitoring data using Pandas and Matplotlib.

🔍 Observations

API requests can be monitored using token consumption, latency, and estimated cost.

Successful API requests generate response and usage information.

Failed API requests can also be recorded with their error details.

MongoDB successfully stores API monitoring records for future analysis.

Pandas helps display and analyze the stored API records.

MongoDB aggregation helps calculate total API attempts, token usage, average latency, and estimated cost.

Matplotlib helps visualize API monitoring information.

🔄 Execution Workflow

The complete execution process follows these steps:

Install the required Python packages.

Configure the Gemini API key.

Connect to the Google Gemini API.

Connect to MongoDB Atlas.

Send prompts to the Gemini model.

Capture input and output token information.

Measure API response latency.

Estimate API usage cost.

Record successful and failed API requests.

Store monitoring records in MongoDB.

Retrieve records from the MongoDB collection.

Display records using Pandas.

Calculate API usage statistics using MongoDB aggregation.

Generate reports and visualizations using Matplotlib.

📚 Learning Outcomes

After completing this practical, I learned:

The importance of monitoring LLM applications.

How to integrate the Google Gemini API with Python.

How to track input and output token consumption.

How to measure API response latency.

How to estimate API usage costs.

How to handle and log successful and failed API requests.

How to connect Python applications with MongoDB Atlas.

How to store and retrieve API monitoring records using PyMongo.

How to analyze stored records using Pandas.

How to calculate API usage statistics using MongoDB aggregation.

How to visualize monitoring data using Matplotlib.

✅ Conclusion

This practical helped me understand how to build an LLM monitoring system using Python, Google Gemini API, and MongoDB. The experiment demonstrated how token consumption, response latency, estimated API cost, and request status can be tracked and stored for every API attempt.

It also provided practical experience in database integration, API usage analysis, and visualization, highlighting the importance of monitoring and managing Generative AI applications.

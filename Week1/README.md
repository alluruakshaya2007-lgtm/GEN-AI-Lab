📌 Project Overview

This project demonstrates how to make the first Large Language Model (LLM) API call using Python, Google Colab, and the Google Gemini API.

The objective of this practical is to understand how Python applications communicate with Large Language Models (LLMs), send prompts, and receive AI-generated responses through an API.

🎯 Objectives

Generate a Gemini API key using Google AI Studio.
Configure the API key securely using Google Colab Secrets.
Install and use the Google GenAI Python SDK.
Initialize the Gemini API client.
Send prompts to a Gemini model.
Receive and display AI-generated responses.
Experiment with different prompts and understand prompt-based interactions.

🛠️ Technologies Used
Python
Google Colab
Google Gemini API
Google GenAI SDK
Google AI Studio

📂 Project Structure
Week1_First_LLM_API_Call_Gemini/
│
├── Week1_First_LLM_API_Call_Gemini.ipynb
└── README.md

⚙️ Setup and Installation

Step 1: Open Google Colab
Visit Google Colab and create a new notebook.

Step 2: Generate Gemini API Key
Visit Google AI Studio.
Sign in using your Google account.
Click on Create API Key.
Generate and copy your API key.

Step 3: Install the Required Package
Execute the following command in a Colab code cell:
!pip install -q google-genai

Step 4: Configure API Key Using Colab Secrets
Open the Secrets section in Google Colab.
Add a new secret.
Set the name as GEMINI_API_KEY.
Paste your Gemini API key as the value.
Enable Notebook access.
Important: Never expose your API key in public notebooks or GitHub repositories.

Step 5: Access the API Key
from google.colab import userdata
GEMINI_API_KEY = userdata.get("GEMINI_API_KEY")
print("Gemini API key loaded successfully.")

Step 6: Initialize Gemini Client
from google import genai
client = genai.Client(api_key=GEMINI_API_KEY)
print("Gemini client initialized successfully.")

Step 7: Execute Your First LLM API Call
response = client.models.generate_content(
    model="gemini-3.8-flash",
    contents="Explain Artificial Intelligence in simple words."
)
print("LLM Response:")
print(response.text)

Note: Model availability depends on your Google AI Studio API project. If this model is unavailable, select another supported Gemini model.


🧪 Five New Prompt Experiments

The following five experiments demonstrate how Gemini interprets different prompts and generates responses.

Experiment 1: AI in Education
Prompt:
Explain how Artificial Intelligence is transforming
education. Give five examples.
Objective: Understand the applications of AI in modern education.

Experiment 2: Blockchain Technology
Prompt:
What is Blockchain Technology? Explain its working
with a simple real-world example.
Objective: Understand the basic concept and working of blockchain technology.

Experiment 3: Cybersecurity
Prompt:
Explain five common cybersecurity threats
and how to prevent them.
Objective: Learn about cybersecurity threats and prevention methods.

Experiment 4: Python Programming
Prompt:
Explain Python programming language and list
five important features of Python.
Objective: Understand Python and its important features.

Experiment 5: Future of Artificial Intelligence
Prompt:
Explain how artificial Intelligence may change
our daily lives in the next ten years.
Objective: Explore the future applications and impact of Artificial Intelligence.

🔄 Execution Workflow

The complete execution process follows these steps:
Python program sends a prompt to the Gemini API.
Gemini API receives the request.
Gemini model processes the prompt.
Gemini generates an AI response.
Python receives and displays the generated response.

📚 Learning Outcomes

After completing this practical, I learned:
The role of API keys in connecting applications with LLMs.
The architecture of Python-to-Gemini API communication.
How to install and use the Google GenAI Python SDK.
How to securely manage API keys using environment secrets.
How to generate AI responses using the Gemini model.
How prompts influence LLM-generated responses.
How to experiment with different real-world AI use cases.


📌 Project Overview

This project implements a Provider-Agnostic Large Language Model (LLM) Client that allows users to interact with different Large Language Model providers through a single common interface.

The application supports two LLM providers:

Google Gemini – A cloud-based LLM accessed through the Gemini API.

Ollama (Llama 3.2) – A locally running LLM that generates responses without requiring a cloud API.


The main objective 
is to create a flexible and reusable LLM client that can switch between different providers without changing the application logic.


🎯 Objectives

Build a common interface for multiple LLM providers.

Integrate Google Gemini using its API.

Integrate Ollama with the Llama 3.2 model.

Implement provider selection at runtime.

Use environment variables to securely manage API keys.

Perform unit testing using Python's unittest framework.



🛠️ Technologies Used
Python

Google Gemini API

Ollama

Llama 3.2

Visual Studio Code

📂 Project Structure

Week-2/
│
├── .env
├── llm_client.py
├── main.py
├── test_client.py
├── requirements.txt
└── README.md


⚙️ Installation and Setup

1. Install Python

Download and install Python from:

https://www.python.org/downloads/

Verify the installation:

python --version

2. Install Ollama

Download Ollama from:

https://ollama.com/download

Install Ollama on your local system.

Verify the installation:

ollama --version

3. Download Llama 3.2 Model

Open PowerShell and execute:

ollama pull llama3.2

This downloads the Llama 3.2 model to your local system.

4. Create a Project Folder

Create a folder named Week-2 in VS Code and add the required Python files.

5. Install Dependencies

Open the terminal inside the project folder and execute:

pip install -r requirements.txt

6. Configure Environment Variables

Create a .env file and add your Gemini API key:

GEMINI_API_KEY=your_api_key_here

Get your API key from:

https://aistudio.google.com/apikey

Note: Never upload your actual API key to GitHub. Add .env to .gitignore.


▶️ Execution

Run the application using:

python main.py

Select your preferred LLM provider:

Choose provider (gemini/ollama):

Enter gemini to use Google Gemini or ollama to use the local Llama 3.2 model.

Enter a question when prompted:

Enter your question: Explain Artificial Intelligence

LLM Response:

[Generated response from the selected LLM]


🧪 Testing

The project includes unit testing using Python's unittest framework.

Run the test file:

python -m unittest test_client.py

Alternatively, use pytest:

python -m pytest

The test uses a FakeProvider to verify that the common LLM client correctly generates and returns responses.


✨ Key Features

Provider Independence: Uses one common interface for different LLM providers.

Cloud Integration: Connects to Google Gemini through its API.

Local LLM Integration: Runs Llama 3.2 using Ollama.

Runtime Selection: Allows users to choose the provider while executing the application.

Reusable Architecture: Makes it easier to add additional LLM providers.

Unit Testing: Verifies the client functionality using a fake provider.


📚 Learning Outcomes

Through this project, I learned:

How to integrate cloud-based and locally hosted LLMs.

How to use Abstract Base Classes (ABC) in Python.

How to implement provider-independent architecture.

How to interact with REST APIs using Python Requests.

How to manage API keys using environment variables.

How to perform unit testing using unittest.

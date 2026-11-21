# WEEK 2 – Provider-Agnostic LLM Client

## 1. Aim
To build a provider-agnostic LLM client that uses one common interface to communicate with Gemini API and a locally running Ollama model.

## 2. Technologies Used
- Python
- Google Gemini API
- Ollama
- Llama 3.2
- Requests
- Python-dotenv

## 3. Folder Structure
WEEK2/
├── main.py
├── llm_client.py
├── test_client.py
├── requirements.txt
├── .env
└── .gitignore

## 4. Installation

Activate the shared virtual environment:

cd C:\GENAI
.\venv\Scripts\Activate.ps1

Navigate to Week 2:

cd PRACTICAL\WEEK2

Install dependencies:

pip install -r requirements.txt

## 5. Configuration

Add your Gemini API key to the .env file:

GEMINI_API_KEY=your_api_key

Never upload your actual API key to GitHub.

Install and download Ollama's model:

ollama pull llama3.2

## 6. Implementation Steps

1. Create a common LLM provider interface.
2. Implement GeminiProvider.
3. Implement OllamaProvider.
4. Create the common LLMClient.
5. Test the client using a fake provider.

## 7. Execution

Run:

python main.py

Choose your provider:

gemini

or

ollama

Enter your question.

## 8. Sample Input

Explain Machine Learning in simple words.

## 9. Testing

Run:

python test_client.py

Expected result:

Ran 1 test
OK

## 10. Result

Successfully implemented a provider-agnostic LLM client supporting both Gemini API and the local Ollama model.

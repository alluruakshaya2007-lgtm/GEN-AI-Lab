**WEEK 6 – Golden Question Set and Baseline Evaluation**

**1. Aim**

To evaluate Llama 3.2 using 30 predefined questions and compare its answers with expected answers using keyword matching.

**2. Technologies Used**
   
- Python
  
- Ollama
  
- Llama 3.2
  
- JSON
  
- CSV
  
- Requests
  
- VS Code

  
**3. Concepts Used**
   
- Golden Question Set
  
- LLM Evaluation
  
- Keyword Matching
  
- Evaluation Score
  
- PASS, REVIEW and ERROR
  
- Baseline Evaluation
  
**4. Installation**
   
ollama pull llama3.2

pip install -r requirements.txt


**5. Project Structure**
   
Week-6/
├── main.py
├── golden_set.json
├── requirements.txt
├── baseline_results.csv
└── README.md


**6. Implementation Steps**
   
1. Create a Golden Question Set with 30 questions.
   
2. Load questions using Python.
   
3. Generate answers using Llama 3.2.
   
4. Compare answers using keyword matching.
   
5. Calculate evaluation scores.
    
6. Classify results as PASS, REVIEW or ERROR.
    
7. Save results in a CSV file.

    
**7. Execution**
   
python main.py


**8. Sample Output**
Total Questions: 30
Model: llama3.2

BASELINE RUN COMPLETED!
Release v0.1 created successfully.


**9. Observations**

- Evaluated 30 questions using Llama 3.2.
  
- Keyword matching calculated answer scores.
  
- Results were classified as PASS, REVIEW or ERROR.
  
- Evaluation results were saved in a CSV file.
  
**10. Result**

Successfully implemented the LLM Baseline Evaluation system using Llama 3.2 and generated the evaluation report as Release v0.1.

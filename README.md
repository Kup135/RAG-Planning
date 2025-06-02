# RAG-Planning
A system for extracting, structuring, and visualizing data from municipal planning document. Using proprietary APIs (Claude and GPT)

## Environment
These notebooks work best with Python version 3.9.6
You can find under requirements.txt all necessary libraries and their recommended versions.

To recreate the virtual environment: 

*pip install -r requirements.txt*


## Files Structure
The PythonNotebooks folder contains the 3 notebooks to run manually the 3 stages of the system:

  (1) RAG - Embedding the original data (pdf planning instructions - הוראות - documents) using Voyage AI API, saving them to a local DB, and then using Claude (Sonnet-3.7) API to query them one by one. 
  
  (2) Structuring - Using GPT API to structure the generated answers from the RAG stage, into JSONs that can be queried (Boolean/Categorical data/Interger/Float). 
  
  (3) SemiFormal - Joining the strucutred data to the metadata (years in which the planning documents were created), using Claude API to produce code snippet for visualizing the data, and running them to produce interactive Plotly visualizations. 

## DATA 
Data to use the system include planning documents under local authority of Tel Aviv municipality. All planning documents can be accessed as open data through the governmental website of the planning authority: https://mavat.iplan.gov.il/

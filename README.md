# streamlit-fastapi-model-serving

Simple example of usage of streamlit and FastAPI for ML model serving

To run the example ,we will use virtual env for proper
package management

## virtual environment

python -m venv vir_env

### For windows

.\vir_env\Scripts\activate

### For Linux

source vir_env/bin/activate

Then run following commands for both streamlit and fastapi in their
respective folders

### streamlit

pip install -r  requirements.txt

streamlit run ui.py --server.port 8501

### fastapi

pip install -r requirements.txt -f https://download.pytorch.org/whl/torch_stable.html

uvicorn server:app  --host   0.0.0.0 --port 8000


To visit the FastAPI documentation of the resulting service, visit http://localhost:8000 with a web browser.  
To visit the streamlit UI, visit http://localhost:8501.

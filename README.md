# Langchain-Demo-with-Gemma-Model

This project demonstrates how to use the Langchain framework with the Gemma model (or any other model supported by Ollama) to create a simple question-answering application. The application is built using Streamlit for the user interface and Langchain for handling the language model interactions. Additionally, LangSmith is integrated for activity tracking, allowing you to monitor and debug your Langchain workflows.

## Prerequisites
Before running the project, ensure you have the following installed:

1. **Python 3.7 or higher**
2. **Ollama** - Download and install Ollama from : https://ollama.com/
3. **LangSmith Account** - Sign up for a LangSmith account at (https://www.langchain.com) and obtain API key for activity tracking.

## Setup
1. **Download and Run Ollama Models:**
   - Download and run the desired models using Ollama. For example:
```bash
ollama run llama3.2
ollama run gemma2:2b
```
   - use any model supported by Ollama.
2. **Environment Variables:**
   - Create a .env file in the root directory of project and add the following variables:
```bash
LANGCHAIN_API_KEY=langchain_api_key
LANGCHAIN_PROJECT=langchain_project_name
```
   - Replace langchain_api_key with  actual LangSmith API key and langchain_project_name with desired project name.
3. **Install Dependencies:**
   - Install the required Python packages by running:
```bash
pip install -r requirements.txt
```
## Running the Application
1.**Clone the Repository:**
```bash
git clone https://github.com/Tanvi3004/Langchain-Demo-with-Gemma-Model.git
```
2.**Run the Streamlit Application:**
```bash
streamlit run app.py
```
3.**Interact with the Application:**
   - Open web browser and navigate to http://localhost:8501.
   - Enter question in the text input box and press Enter.
   - The application will use the Gemma model (or any other model you specified) to generate a response.

## Features
**LangSmith Integration:** Track and debug Langchain workflows using LangSmith. All activities are logged and can be viewed in LangSmith dashboard.
**Customizable Models:** Use any model supported by Ollama by simply changing the model name in the code.
**Streamlit UI:** A simple and intuitive web interface for interacting with the language model.

## Customization
**Model Selection:** change the model by modifying the model parameter in the Ollama initialization in app.py.
**Prompt Customization:** Modify the ChatPromptTemplate in app.py to change the system message or user prompt.

## Requirements
   - The requirements.txt file lists all the dependencies needed to run this project:
   - Install the dependencies using:
```bash
pip install -r requirements.txt
```
### Streamlit App
This is how the app looks when running:
<img width="1440" alt="Image" src="https://github.com/user-attachments/assets/7971aedc-7810-495f-b553-387965f0ccc2" />

## Contributing
Feel free to contribute to this project by opening issues or submitting pull requests. Your contributions are welcome!


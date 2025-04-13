🏋️‍♂️ Personal Fitness AI Agent
This project is a chat-based AI assistant built using Langflow, Streamlit, and the Datastax Astra API, designed to help users with personalized fitness queries. From training routines to diet tips, this assistant leverages a backend Langflow flow to generate meaningful and contextual responses.

🚀 Features
✨ Chat interface built with Streamlit

🔗 Connects to Langflow API hosted on Astra

📥 Accepts free-form user fitness questions

💬 Returns contextual, conversational AI responses

🔐 Environment-based secure token usage

🧰 Tech Stack
Langflow – Visual framework for building LLM-based workflows

Streamlit – Web UI for building interactive apps

Datastax Astra – Cloud-native database and Langflow hosting

Python – Core scripting

📦 Installation
Clone the repository

bash
Copy
Edit
git clone https://github.com/yourusername/personal-fitness-ai.git
cd personal-fitness-ai
Install dependencies

bash
Copy
Edit
pip install -r requirements.txt
Set up environment variables

Create a .env file in the root directory and add your Astra Application Token:

ini
Copy
Edit
APP_TOKEN=your_application_token
Edit Flow Configuration

In main.py, update the following fields:

python
Copy
Edit
LANGFLOW_ID = "your-langflow-id"
FLOW_ID = "your-flow-id"
ENDPOINT = "your-endpoint-name"  # e.g., "customer"
You can get these values from the Langflow flow configuration screen or the API section.

▶️ Usage
Start the Streamlit app:

bash
Copy
Edit
streamlit run main.py
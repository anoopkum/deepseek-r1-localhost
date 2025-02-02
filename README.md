DeepSeek R1 - Localhost

This repository provides a step-by-step guide to deploying DeepSeek R1 locally using Azure AI Foundry. By following these instructions, you can set up and interact with the DeepSeek R1 model in a local web application.

Prerequisites

Before starting, ensure you have the following installed:

Python (latest version recommended)

Azure Account with access to Azure AI Foundry

Git

Virtual Environment (venv)

Step-by-Step Configuration

1. Clone the Repository

 $git clone https://github.com/anoopkum/deepseek-r1-localhost.git
 $cd deepseek-r1-localhost

2. Configure Azure AI Foundry

Log in to Azure Portal.

Navigate to Azure AI Foundry.

Create a Project and AI Hub.

Go to the Models section and explore the DeepSeek-R1 model.

Deploy the model directly from the portal.

3. Set Up Environment Variables

Once the model is deployed, obtain the Endpoint URL and API Key from Azure AI Foundry.

Create a .env file in the project root and add the following:

AZURE_AI_ENDPOINT=<your_endpoint_url>
AZURE_AI_KEY=<your_api_key>

4. Set Up Python Virtual Environment

On macOS/Linux:

$python3 -m venv venv
$source venv/bin/activate

On Windows:

$python -m venv venv
$venv\Scripts\activate

5. Install Dependencies

$pip install -r requirements.txt

6. Start Chatbot Interaction

Run the following command to interact with DeepSeek R1 via the command line:

$python3 chat.py

7. Deploy the Web Application

To launch the web-based chatbot locally, run:

$python3 app.py

Open your browser and visit: http://127.0.0.1:5000

Start chatting with DeepSeek R1!

Summary

This guide helps you deploy the DeepSeek R1 chatbot using Azure AI Foundry and run it locally as a web application. By following these steps, you can easily configure, interact with, and deploy the chatbot for AI-based conversations.

# RMIT-CHAT_BOT
Step-by-Step Guide
1. Create a Virtual Environment
    Command (run in your project directory where chatbot_brain.py and chatbot_ui.py are located):
    On Windows:
        python -m venv .venv
    On macOS/Linux:
        python3 -m venv .venv

    Explanation: This creates a virtual environment named .venv in your current directory, isolating your project dependencies.


2.Activate the Virtual Environment
    Command:
        On Windows:
            .\.venv\Scripts\activate
        On macOS/Linux:
            source .venv/bin/activate

    Explanation: Activating the virtual environment ensures that any Python packages you install are local to this project. You’ll see (.venv) in your terminal prompt when it’s active.


3.Update pip
    Command:
        python -m pip install --upgrade pip

    Explanation: Updates pip to the latest version to avoid compatibility issues during installation.


4. Install Required Packages Individually
    Commands (run each command one by one in the activated environment):
        pip install langchain_community==0.3.24
        pip install langchain_openai==0.3.21
        pip install langchain==0.3.25
        pip install langchain-core==0.3.64
        pip install langchain-text-splitters==0.3.8
        pip install openai==1.84.0
        pip install faiss-cpu==1.11.0
        pip install python-dotenv==1.1.0
        pip install termcolor==3.1.0
        pip install streamlit==1.45.1
    Explanation: These commands install the exact versions of the packages required by your chatbot, as identified from your code and pip list.


5.Run Your Chatbot
    Create Knowledge Base:
        python chatbot_brain.py
    Launch UI:
        streamlit run chatbot_ui.py


Notes
    Environment Setup: Perform these steps in a new directory or clean up any existing .venv if reusing the project folder.
    API Key: Ensure your .env file contains OPENAI_API_KEY=your_api_key_here for the OpenAI API to work.
    Timestamp: It’s 03:29 PM +0530 on June 09, 2025—plenty of time to set this up before your submission deadline.
    Troubleshooting: If any command fails, check for internet connectivity or permission issues. Share any error messages for further assistance.

# Chat-with-Promptflow

This repository contains a simple chat flow using Azure OpenAI and PromptFlow for handling LLM-based conversations. The main script triggers an AI response for a given input question using the Prompty object.

## Project Structure

- `flow.py`: Contains the main logic to load environment variables, initialize the Prompty object, and make the LLM call.
- `chat.prompty`: Configuration file for the Prompty object, specifying the OpenAI model and its parameters.

## Setup Instructions
### Prerequisites
- Python 3.8+
- Install dependencies: `promptflow`, `python-dotenv`, `azure-openai`

### Environment Variables
Ensure that the following environment variables are available, either via `.env` or system-wide configuration:
- `AZURE_OPENAI_ENDPOINT`
- `AZURE_OPENAI_API_KEY`

### Steps to Run
1. Clone the repository:
    ```bash
    git clone <repository-url>
    cd <repository-folder>
    ```
2. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```
3. Set up the environment variables in a `.env` file:
    ```ini
    AZURE_OPENAI_ENDPOINT=<your-endpoint>
    AZURE_OPENAI_API_KEY=<your-api-key>
    ```
4. Run the script:
    ```bash
    python flow.py
    ```
or
```bash
    pf flow test --flow flow:chat --ui 
``` 

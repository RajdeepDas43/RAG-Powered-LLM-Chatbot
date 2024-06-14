# RAG-Based-Multi-Source-Chatbot-Using-LLM

## Introduction

In general, chatbots are used for information retrieval. Traditional chatbots typically work based on predefined rules and keyword matching. These chatbots rely on a fixed knowledge base or database of predefined responses. The responses are manually inserted into the database by the developer. When a user inserts a query, the chatbot looks for the rules that match the question and provides the hardcoded response. This method doesn't support paraphrasing or generation of new responses.

Nowadays, LLM-based chatbots are in high demand. LLM-based chatbots can be of two types:

1. **LLM-Based Chatbots without RAG:** Large Language Models (LLM) such as OpenAI's GPT or Meta's LLaMA are trained with billions of parameters and huge amounts of textual data. These models can be used via APIs provided by their respective organizations. However, these chatbots generate responses directly from the data they were trained on, without considering any external knowledge base, similar to how ChatGPT operates.

2. **LLM-Based Chatbots with RAG:** RAG stands for Retrieval-Augmented Generation. This approach uses two main components: generation and retrieval. Unlike LLM-based chatbots without RAG, RAG-based chatbots utilize external data sources such as PDFs, text files, or databases as a knowledge base along with the trained LLM model. When a user asks a question, the chatbot first retrieves similar text chunks from the external knowledge base. These text chunks are then used as prompts for the LLM model, which generates a more precise and contextually relevant answer.

In this project, a multi-source chatbot using RAG has been implemented. Users can upload various types of documents like PDFs and text files as an external knowledge base and interact with the chatbot to get answers that reference the knowledge base. The chatbot utilizes both the knowledge base and the pre-trained LLM to provide reliable, relevant, and organized answers.

## High-Level Overview of the RAG-Based Chatbot

![High-Level Overview](https://github.com/semanto-mondal/RAG-Based-Multi-Source-Chatbot-Using-LLM/assets/133217806/80095c2c-a993-4296-b1dc-f802fa1875cf)

## Flow Chart of the Chatbot

![Flow Chart](https://github.com/semanto-mondal/RAG-Based-Multi-Source-Chatbot-Using-LLM/assets/133217806/6a18696a-93b8-4bd8-a548-6f3fc5eb1910)

## Navigation Bar of the Chatbot

![Navigation Bar](https://github.com/semanto-mondal/RAG-Based-Multi-Source-Chatbot-Using-LLM/assets/133217806/20301ec9-9498-4de0-be3a-b7eb3e493c23)

## Document Embedding Interface

![Document Embedding Interface](https://github.com/semanto-mondal/RAG-Based-Multi-Source-Chatbot-Using-LLM/assets/133217806/dc58999e-7740-44eb-8c97-b4929725ff49)

## Chatbot Interface

![Chatbot Interface](https://github.com/semanto-mondal/RAG-Based-Multi-Source-Chatbot-Using-LLM/assets/133217806/8c04d3ff-3fde-466b-ba06-b3ac58290d85)

## How to Run the Code

### Prerequisites

1. **Python 3.8+**: Ensure that Python is installed on your system.
2. **pip**: Package installer for Python.

### Installation

1. **Clone the Repository:**

    ```sh
    git clone https://github.com/yourusername/RAG-Based-Multi-Source-Chatbot-Using-LLM.git
    cd RAG-Based-Multi-Source-Chatbot-Using-LLM
    ```

2. **Install Dependencies:**

    ```sh
    pip install -r requirements.txt
    ```

### Running the Chatbot

1. **Start the Streamlit Application:**

    ```sh
    streamlit run chatbot_streamlit_combined.py
    ```

2. **Upload Documents:**

    - Navigate to the document embedding interface in the Streamlit app.
    - Upload the required PDF or text files as the external knowledge base.

3. **Interact with the Chatbot:**

    - Go to the chatbot interface.
    - Ask questions and get responses that reference the uploaded documents.

### Development Container (Optional)

For a consistent development environment, you can use the provided devcontainer configuration. This setup uses Visual Studio Code's Remote - Containers extension.

1. **Install Visual Studio Code and the Remote - Containers extension.**

2. **Open the Project in a Dev Container:**

    - Open the project in Visual Studio Code.
    - Press `F1` and select `Remote-Containers: Reopen in Container`.


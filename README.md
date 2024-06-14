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

## How to Run the Code

### Prerequisites

1. **Python 3.8+**: Ensure that Python is installed on your system.
2. **pip**: Package installer for Python.

### Installation

1. **Clone the Repository:**

    ```sh
    git clone https://github.com/RajdeepDas43/RAG-Based-Multi-Source-Chatbot-Using-LLM.git
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
  
# Evaluation Pipeline for RAG
## Overview
The evaluation pipeline for the Retrieval-Augmented Generation (RAG) model assesses its performance in providing accurate and contextually relevant responses based on both internal knowledge (from the trained model) and external knowledge (from provided documents). This process involves several steps:

1. Step 1: Data Preparation
Document Collection: Gather a set of documents that will serve as the external knowledge base. These can be in various formats such as PDF, text files, etc.
Query Collection: Prepare a set of queries or questions that the chatbot will respond to. These should be relevant to the content in the documents.
2. Step 2: Embedding and Indexing
Document Embedding: Convert the documents into vector embeddings using a pre-trained model. This allows the system to perform similarity searches.
Indexing: Store the document embeddings in a vector database, such as FAISS, to enable efficient retrieval.
3. Step 3: Retrieval
Query Embedding: Convert the user queries into vector embeddings.
Similarity Search: Perform a similarity search in the vector database to retrieve the most relevant document chunks based on the query embeddings.
4. Step 4: Generation
Prompt Creation: Combine the retrieved document chunks with the user query to create a prompt.
Response Generation: Use the LLM to generate a response based on the combined prompt. The LLM leverages both its internal knowledge and the retrieved document chunks to provide a more accurate and contextually relevant answer.
5. Step 5: Evaluation Metrics
Accuracy: Measure how accurately the responses answer the user queries.
Relevance: Assess the relevance of the responses to the user queries.
Fluency: Evaluate the fluency and coherence of the generated responses.
User Satisfaction: Gather feedback from users to assess their satisfaction with the chatbot’s responses.
6. Step 6: Iterative Improvement
Error Analysis: Analyze the errors or shortcomings in the responses to identify areas for improvement.
Model Tuning: Adjust the model parameters, retrain the model, or update the document embeddings and indexing process as needed.
Re-evaluation: Re-run the evaluation pipeline to assess the improvements and ensure the model is performing optimally.

## Conclusion
The evaluation pipeline for a RAG-based chatbot is crucial to ensure that the model provides accurate, relevant, and contextually appropriate responses. By leveraging both internal and external knowledge sources, the RAG model can significantly enhance the capabilities of traditional chatbots, making them more effective in a wide range of applications.


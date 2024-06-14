# RAG-Based-Multi-Source-Chatbot-Using-LLM

LINK TO THE CHATBOT: [CLICK HERE](https://rag-based-multi-source-chatbot-using-llm-bbkumqwvqftpjkut7tik6.streamlit.app/)

**Introduction**
In general, chatbots are used for information retrieval. Traditional chatbots typically work based on some predefined rules as well as keyword matching. It’s kind of a set of if-else rules predefined by the users. When a user inputs a query, the chatbot searches for specific keywords or patterns in the query to identify the appropriate response. Traditional chatbots rely on a fixed knowledge base or database of predefined responses. The responses are manually inserted into the database by the developer. When a user inserts a query, the chatbot looks for the rules that are suitable based on the question, when it finds the question then it gives the answer that is hardcoded associated with that question. It doesn’t make any paraphrasing or can’t perform any generation. Nowadays, LLM-based chatbots are in the hype. LLM-based chatbots can be of two types.
1. **LLM-Based Chatbots without RAG:** Large Language Models (LLM) such as OpenAI, llama is trained with billions of parameters as well as with huge amounts of textual data. Some of these are open-source means that can be used without any payment and some are not. We can use the chatbot for our purpose using the API provided by the respected organization of these LLMs. But here the problem is that when a user asks any question it will directly answer from the data it has been trained on without considering any external knowledge base. It will work just as ChatGPT
2. **LLM-Based Chatbots with RAG:** RAG stands for Retrieval-Augmented Generation. It has two main components generation and retrieval. Unlike LLM-based chatbots without the RAG concept, here external data sources such as PDF, text, and database are used as knowledge base along with the trained LLM model. So In this case, when any user asks for a query it first looks for a similar type of text chunk in the external knowledge base which is named retrieval, these text chunks are used as prompts to the LLM model. Based on the context and user query the LLM model can create a more precise and creative answer which can be referred to as generation. This is not possible with other types of chatbot.
In this project, a multisource chatbot using RAG has been implemented where users can upload various types of documents like pdf, and text as an external knowledge base and ask the chatbot to answer questions referring to the knowledge base. The chatbot utilizes the knowledge base as well as the pre-trained LLM to get more reliable, relative, and organized answers.

**High-Level Overview of the RAG-Based Chatbot**
![image](https://github.com/semanto-mondal/RAG-Based-Multi-Source-Chatbot-Using-LLM/assets/133217806/80095c2c-a993-4296-b1dc-f802fa1875cf)


**Flow Chart of the Chatbot**
![image](https://github.com/semanto-mondal/RAG-Based-Multi-Source-Chatbot-Using-LLM/assets/133217806/6a18696a-93b8-4bd8-a548-6f3fc5eb1910)

**Navigation Bar of the Chatbot**
![image](https://github.com/semanto-mondal/RAG-Based-Multi-Source-Chatbot-Using-LLM/assets/133217806/20301ec9-9498-4de0-be3a-b7eb3e493c23)

**Document Embedding Interface**
![image](https://github.com/semanto-mondal/RAG-Based-Multi-Source-Chatbot-Using-LLM/assets/133217806/dc58999e-7740-44eb-8c97-b4929725ff49)

**Chatbot Interface**
![image](https://github.com/semanto-mondal/RAG-Based-Multi-Source-Chatbot-Using-LLM/assets/133217806/8c04d3ff-3fde-466b-ba06-b3ac58290d85)


**Special Thanks to Rendyk for a helpful article published on Analytical Bidhay** 

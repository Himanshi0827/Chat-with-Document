# Chat-with-Document
This Streamlit application allows users to interactively chat with a document using Google Generative AI and LLAMA (Language-Model and Application) Index. This Streamlit application allows users to chat with a document using AI-powered conversational agents. The application integrates various components such as document indexing, language models, and conversational chains to facilitate interactive conversations based on the provided document's context.

# Components
# Document Indexing: 
The application uses the llama_index library to load and index documents. It leverages the VectorStoreIndex and SimpleDirectoryReader to process documents from a specified directory.

# Language Models: Two language models are utilized:

Gemini from llama_index for document embeddings and semantic understanding.
ChatGoogleGenerativeAI from langchain_google_genai for generating responses to user queries.

# Conversation Management: 
The ConversationChain manages the conversational flow, maintaining context and generating relevant responses.

Installation and Setup
# Install the required libraries using pip:

Copy code
pip install streamlit llama_index langchain_google_genai langchain_core
Obtain the necessary API keys for Gemini and ChatGoogleGenerativeAI and replace them in the code where indicated.

Place your documents in a directory (./data by default) to be indexed by the application.

# Run the Streamlit app:

arduino
Copy code
streamlit run app.py
Usage
Upon running the app, a chat interface will appear.
Start by asking questions related to the indexed documents.
The AI engine will process your query, consider the context, and provide relevant responses.
The conversation history is displayed, including messages from the user and the AI assistant.

Code Structure
app.py: Main Streamlit application code.
llama_index.py: Handles document indexing and embeddings.
langchain_google_genai.py: Integrates the Google Generative AI for chat responses.
README.md: Documentation file (this file).


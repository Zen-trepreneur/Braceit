# Branceit
# [BranceIT Writeup Doc](https://docs.google.com/document/d/e/2PACX-1vS6RRv4jSkaTzYiYVfYf5GyUTrRhPKn_GYsRJCusKHtHtpeTeKCNLaCp6E7OkSjGw/pub)
![arch](https://github.com/Zen-trepreneur/Braceit/assets/59253439/1544822d-d381-4ffd-8b56-ab9ab1bfb99e)
## Built using Chroma DB, LangChain, OpenAI API and Streamlit.
A Contexutal Parser Bot for Question Answer Generation.
## Usage
The Streamlit app is hosted and running on Replit, open your web browser and navigate to the local URL provided by Replit (https://branceml.rudrakj.repl.co/#brance-chatbot-app). You will see a simple text input box where you can type your question related to the documents required as in the Knowledge Document.

Type your question in the text input box and press Enter.

The chatbot will process your query using LangChain, GPT LLMs and ChromaDB as mentioned above and provide a response based on the information available in the indexed documents.

The chatbot's response will be displayed under the text input box as below:
![image](https://github.com/Zen-trepreneur/Braceit/assets/59253439/2be3f526-b06a-4418-811f-5ac1c97e554c)

Alongside, the Colab file 'Branceit_ML.ipynb' is the MVP for the validation of the solution architecture.
## ChromaDB is employed for semantic search, which involves the following steps:

Vectorization of Documents: The knowledge-related document is converted into numerical embeddings using Sentence Transformer,captures semantic information from the text.

Indexing Documents: The vectorized documents are indexed into ChromaDB, optimizing for similarity search based on embeddings.

Similarity Search: When a user submits a query, the chatbot performs a similarity search in ChromaDB to find the most relevant documents related to the query based on their semantic similarity with the query's embedding.
![image](https://github.com/Zen-trepreneur/Branceit/assets/59253439/d076762f-34c5-4173-983e-075ce8c9a6f8)


# My Langflow RAG Chatbot

This is a chatbot using Langflow with RAG functionality, backed by Ollama and ChromaDB, all running in Docker.


## Prerequisites:

- Docker and Docker Compose installed

## How to run:

1. Clone the repository:
   - git clone https://github.com/ToivoSeppa/chatbot-hanna
   - cd chatbot-hanna


2. Start all services (may take several minutes):
   - docker compose up -d


3. Open Langflow in your browser at http://localhost:7860


4. Click create new flow, choose any flow, and then click the langflow logo in the top left corner.


5. Load the flow configuration for the student chatbot (Student chatbot (main).json)

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/174d7e26-fa29-4406-b818-e5084b159c4f" />


6. Pull LLM and embedding-model from Ollama
   - ollama pull llama3.1
   - ollama pull nomic-embed-text


7. Upload the text-file from the data-folder (arcada_text_data_full.txt)

<img width="1920" height="1080" alt="image (2)" src="https://github.com/user-attachments/assets/d58eeb6a-3400-408a-a056-d055fca2122d" />


8. Run the ChromaDB component (takes several minutes)
     - Make sure you have the embeddings-model in the Ollama Embeddings component.

<img width="1920" height="1080" alt="image (1)" src="https://github.com/user-attachments/assets/f7de2bc9-9f5b-42af-946c-079ad44d7b1e" />


9. Start chatting with the playground function!

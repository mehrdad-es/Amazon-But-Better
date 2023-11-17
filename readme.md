## Intro
Amazon started out with selling books. However, searching books on Amazon is tedious and inaccurate if you don't know what you are exactly looking for. **Why not make it faster and easier with LLMs:)**. This chatbot's context is based on all the Kindle ebooks found in the biography section of amazon.ca .

**check out the FREE chatbot here:** https://huggingface.co/spaces/mehrdad-es/Amazon-But-Better

## Strategy
1. Gather Kindle Ebook Descriptions using selenium
2. Create Embeddings Dataset with Cohere embed and Chromadb
3. Use Langchain RetrievalQA & Cohere Command to query this the ebooks vector embeddings dataset

## Notes
* Experimenation with memory and ConversationRetrievalChain has resulted in less performance, usefulness, and more halucination. Hence, this chat bot provides one shot answers with zero memory. You can use the code in the RAG notebook to do this experimentation.
  


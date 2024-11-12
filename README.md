## GenAI - Local QnA Chatbot using RAG

#### Aim:
Create a locally running QnA chatbot using RAG pipeline, It should be able to answer the questions based on provided PDF using locally downloaded Large Language Model (LLM)<br>
We use google gemma LLM in our code and for input data we use publicly available PDF.


#### Code flow Outline:

1. Text splitting/chunking: Format the text from PDF ready for embedding model<br>
2. Embed all of the chunks of text in the textbook in numerical format<br>
3. Use vector search for retrieval system to find relevant chunks of text for a query<br>
4. Create prompt for above chunk texts<br>
5. Generate answer to a query based on passages from the textbook with help of LLM<br>


#### Setup/Installation

Install packages as below:<br>
pip install PyMuPDF tqdm sentence-transformers accelerate bitsandbytes 

<br>Make sure you have NVIDIA Cuda installed as per your GPU, if no GPU then just install torch<br>
python -m pip install torch==2.5.1+cu124 --index-url https://download.pytorch.org/whl/cu124

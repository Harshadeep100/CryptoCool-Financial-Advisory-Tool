# CryptoCool-Financial-Advisory-Tool

# Features:  
Import URLs or upload text documents that include URLs to retrieve article content. 

Utilize LangChain's UnstructuredURL Loader to process the article content.  

Create an embedding vector using OpenAI's embeddings and make use of FAISS, a robust similarity search tool, to facilitate quick and efficient retrieval of pertinent information.  

Engage with the LLM (Chatgpt) by submitting inquiries and obtaining responses along with their corresponding source URLs.

# Installation:
1.Clone this repository to your local machine

2.Navigate to the project directory

3.Install the required dependencies using pip: - pip install -r requirements.txt

4.Set up your OpenAI API key or HuggingFace API key by creating a .env file in the project root and adding your API

HuggingFaceHub_API_KEY=your_api_key_here (This has to be in your .env file)

# Usage
You can Run the Streamlit app by executing
streamlit run main.py

The web application will launch in your browser.

In the headerbar, you can directly enter URLs.

Start the data loading and processing by clicking on "Analyze URLs"

Watch the system as it conducts text splitting, creates embedding vectors, and indexes them efficiently using FAISS.

The embeddings will be stored and indexed with FAISS, improving retrieval speed.

The FAISS index will be saved in a local file path in pickle format for future reference.

You can now pose a question and receive an answer based on those news articles.

# Project Structure
main.py: This is the main Streamlit application script.

requirements.txt: A list of Python packages that is required for the project.

faiss_store_openai.pkl: FAISS index is stored in the pickle file.

.env: Configuration file for storing OpenAI/HuggingFace API key.

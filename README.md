# 🧠 Advanced RAG App with AWS Bedrock & LangChain
A powerful Retrieval-Augmented Generation (RAG) application built using AWS Bedrock and LangChain, designed to interact with custom PDF data using state-of-the-art Large Language Models (LLMs) like Claude, LLaMA2, and even generate images using Stable Diffusion.

🚀 Features

    📄 Chat with PDFs using custom embeddings and vector search

    🤖 Generate rich, contextual answers using LLaMA2 and Claude LLMs

    🧠 Powered by AWS Bedrock's Titan Embedding and Foundation Models

    🎨 Generate high-quality images using Stable Diffusion via Bedrock

    🛠 Built with LangChain, FAISS, and Streamlit

🧱 Tech Stack
Layer	Technology
LLMs	LLaMA2 (meta.llama2-70b-chat-v1), Claude (ai21.j2-mid-v1)
Embeddings	Amazon Titan (amazon.titan-embed-text-v1)
Retrieval	FAISS
Orchestration	LangChain
Frontend	Streamlit
Backend	Python + Boto3 (AWS SDK)

📂 Project Structure

├── app.py               # Main Streamlit app for interacting with PDFs
├── llama2.py            # LLaMA2-based text generation using Bedrock
├── claude.py            # Claude-based text generation using Bedrock
├── stablediffusion.py   # Image generation with Stable Diffusion via Bedrock
├── test.json            # Sample payload for model testing
├── requirements.txt     # Python dependencies
├── .gitignore

📌 Use Cases

    Internal document Q&A assistants

    Legal or medical document search tools

    Knowledge-based chatbots

    Creative tools for text & image generation

🛠 Installation & Setup

    Clone the repository

git clone https://github.com/suhan21/advanced-rag-bedrock-langchain.git
cd advanced-rag-bedrock-langchain

    Install dependencies

pip install -r requirements.txt

    Configure AWS CLI

aws configure

    Run the app

streamlit run app.py

📎 How It Works

    Upload PDFs into the /data/ directory.

    Click "Vectors Update" in the sidebar to generate and store embeddings using Titan.

    Ask any question in the input box.

    Choose either Claude Output or LLaMA2 Output to get results.

    Internally, LangChain handles retrieval + generation using FAISS and LLMs.

🖼 Bonus: Image Generation

Use stablediffusion.py to generate high-quality 4K images from prompts using Stable Diffusion XL on Bedrock.

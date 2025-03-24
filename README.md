# Shazam-Clone-Audio-Transcription-Subtitle-Search
🔍 Project Overview
 I built an intelligent search engine that allows users to find relevant video subtitles using audio queries. By leveraging vector embeddings and semantic search, this system retrieves the most relevant subtitle segments for any spoken input.
🔑 How It Works
✅ Data Processing
 🔹 Processed a 1.9 GB dataset of .srt subtitle files
 🔹 Optimized storage by converting data to Parquet format
 🔹 Indexed and cleaned 30% of the dataset for efficient search
✅ Chunking & Embeddings
 🔹 Split subtitle files into context-aware chunks
 🔹 Generated vector embeddings using ChromaDB + Sentence Transformers
 🔹 Leveraged Google Colab’s T4 GPU, completing embedding generation in ~40 minutes
✅ Search & Retrieval
 🔹 Accepted audio files (>2 mins) as input
 🔹 Converted speech to text with AssemblyAI
 🔹 Encoded text and applied cosine similarity to fetch top 5 relevant subtitle matches
✅ Deployment & UI
 🔹 Faced a few build tool challenges, so deployed on Google Colab + Gradio
 🔹 Delivered real-time search with an interactive UI for seamless audio-to-text retrieval
💡 Tech Stack
 🏹 Automatic Speech Recognition (ASR): AssemblyAI
 🏹 Vector Database: ChromaDB
 🏹 NLP Models: Sentence Transformers
 🏹 Deployment: Google Colab + Gradio
📌 Why Does This Matter?
 This project demonstrates how AI, NLP, and vector search can enhance media accessibility. It has real-world applications in video platforms, transcription services, and AI-driven media indexing.

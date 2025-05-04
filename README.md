Literature Review Generator

This project uses RAG (Retrieval-Augmented Generation) to generate literature reviews from a curated set of 12 open-access research papers. These papers span the domains of:

1. Blockchain
2. Deep Learning
3. Web Development

The goal is to allow users to query and retrieve synthesized insights from this academic knowledge base.

System Overview
LangChain	Orchestrates the RAG pipeline by integrating retrieval and generation.
ChromaDB	Stores document embeddings and enables efficient semantic search.
OpenAIEmbeddings	Converts document chunks and user queries into vector representations.
GPT-4o mini	The LLM (via OpenAI API) that generates human-like responses based on retrieved content.
Gradio UI	Provides an interactive web interface for users to input queries and view generated outputs.
To better understand the relationship between the document embeddings, we visualized their distribution using t-SNE

Environment Setup
API keys and configuration secrets are stored in a .env file. Create this file in the root of your project and add:
OPENAI_API_KEY=your_openai_key_here
⚠️ Do not commit .env to source control. Add it to .gitignore.


Research papers used for RAG:
Blockchain
Title: A Survey of Blockchain From the Perspectives of Applications, Challenges, and Opportunities
Authors: Ahmed Afif Monrat, Karl Andersson, Olov Schelén

Title: Blockchain Technology Overview
Authors: Dylan Yaga, Peter Mell, Nik Roby, Karen Scarfone

Title: Understanding Blockchain Technology
Authors: Simanta Shekhar Sarmah

Deep Learning
Title: A Survey on Visual Transformer
Authors: Kai Han, Yunhe Wang, Hanting Chen, Xinghao Chen, Jianyuan Guo, Zhenhua Liu, Yehui Tang, An Xiao, Chunjing Xu, Yixing Xu, Zhaohui Yang, Yiman Zhang, Dacheng Tao

Title: Attention Is All You Need
Authors: Ashish Vaswani, Noam Shazeer, Niki Parmar, Jakob Uszkoreit, Llion Jones, Aidan N. Gomez, Łukasz Kaiser, Illia Polosukhin

Title: Attention Mechanism, Transformers, BERT, and GPT: Tutorial and Survey
Authors: Benyamin Ghojogh, Ali Ghodsi

Title: BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding
Authors: Jacob Devlin, Ming-Wei Chang, Kenton Lee, Kristina Toutanova

Title: Sentiment Classification: Review of Text Vectorization Methods: Bag of Words, Tf-Idf, Word2vec and Doc2vec
Authors: Haisal Dauda Abubakar, Mahmood Umar, Muhammad Abdullahi Bakale

Web Development
Title: Accessible Web Development: Opportunities to Improve the Education and Practice of Web Development with a Screen Reader
Authors: Claire Ferrari, Amy Hurst

Title: Development of Web-based Metaverse Platform
Authors: Junmyeong Kim, et al.

Title: MDD4REST: Model-Driven Methodology for Developing RESTful Web Services
Authors: Amirhossein Deljouyi and Raman Ramsin

Title: Web Development: Estimating Quick-to-Market Software
Authors: Donald J. Reifer



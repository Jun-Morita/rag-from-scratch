# RAG From Scratch

LLMs are trained on a large but fixed corpus of data, limiting their ability to reason about private or recent information. Fine-tuning is one way to mitigate this, but is often [not well-suited for facutal recall](https://www.anyscale.com/blog/fine-tuning-is-for-form-not-facts) and [can be costly](https://www.glean.com/blog/how-to-build-an-ai-assistant-for-the-enterprise).
Retrieval augmented generation (RAG) has emerged as a popular and powerful mechanism to expand an LLM's knowledge base, using documents retrieved from an external data source to ground the LLM generation via in-context learning. 
These notebooks accompany a [video playlist](https://youtube.com/playlist?list=PLfaIDFEXuae2LXbO1_PKyVJiQ23ZztA0x&feature=shared) that builds up an understanding of RAG from scratch, starting with the basics of indexing, retrieval, and generation. 

LLM（大規模言語モデル）は、大規模ではあるものの固定されたデータコーパスで訓練されるため、最新の情報やプライベートな情報に基づいて推論する能力が制限されています。ファインチューニングはこの問題を軽減する一つの方法ですが、[事実のリコールには適していない](https://www.anyscale.com/blog/fine-tuning-is-for-form-not-facts)ことが多く、[コストがかかる](https://www.glean.com/blog/how-to-build-an-ai-assistant-for-the-enterprise)場合もあります。これを解決するために、外部のデータソースから取得した文書を用いて、LLMの生成をインコンテキスト学習で補強する「Retrieval Augmented Generation（RAG）」が、知識ベースを拡張する強力な手法として注目されています。このノートブックは、RAGを基礎から理解するための[ビデオプレイリスト](https://youtube.com/playlist?list=PLfaIDFEXuae2LXbO1_PKyVJiQ23ZztA0x&feature=shared)に対応しており、インデックス作成、検索、生成の基本から始めて構築していきます。

![rag_detail_v2](https://github.com/langchain-ai/rag-from-scratch/assets/122662504/54a2d76c-b07e-49e7-b4ce-fc45667360a1)

## Environment Setup

> conda create -n rag-from-scratch python=3.11  
> conda activate rag-from-acratch  

> pip install notebook ipython langchain_community tiktoken langchain-openai langchainhub chromadb langchain youtube-transcript-api pytube cohere  

or 

> pip install -r requirements.txt  



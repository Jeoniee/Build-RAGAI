# Build-RAGAI
Description

This project seeks to teach you how to build Python applications with generative AI functionality by using the LangChain and Transformers libraries.


[1주차] 기본과제 - MNIST를 분류 모델로 학습하기

[1주차] 심화과제 - MNIST 예측 모델에 deep learning techniques 적용하기

[2주차] 기본과제 - 주어진 문장에서 나올 다음 단어를 예측하는 모델 구현

[2주차] 심화과제 - Multi-head Attention으로 감정 분석 모델 구현하기

[3주차] 기본과제 - DistilBERT로 뉴스 기사 분류 모델 학습하기

[3주차] 심화과제 - Pre-trained 모델로 효율적인 NLP 모델 학습하기





# 🧠 Last Word Prediction with Transformer

간단한 문장 데이터를 기반으로, Transformer 모델이 문장의 마지막 단어를 예측하도록 학습한 실험입니다.  
Self-Attention부터 Multi-Head Attention, Residual Connection, LayerNorm, Dropout까지 직접 구현하여 적용했습니다.

---

## 🏗️ 모델 구조

- Embedding + Positional Encoding
- Multi-Head Self-Attention (4-head)
- Feed-Forward Network (FFN)
- Residual Connection + Layer Normalization + Dropout
- 마지막 `[CLS]` 위치를 활용해 단어 분류


Test Your First Notebook
If you're totally new to building AI powered applications with access to external data, specifically retrieval augmented generation, check out the RAG Basics notebook. It's the most straightforward notebook, and its concepts are built upon in every other 'RAG' notebook.

Google Colab
Click the badge below to open the RAG Basics notebook in Colab.

Open 'rag_basics.ipynb' In Colab


```text
Input → Embedding + Positional Encoding
      → [Transformer Layer × 5]
      → Linear(vocab_size) → Predicted token


입력: "I love"
모델 예측: "you"









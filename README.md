# spartaAI
항해99 AI 과제

[1주차] 기본과제 - MNIST를 분류 모델로 학습하기

[1주차] 심화과제 - MNIST 예측 모델에 deep learning techniques 적용하기


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

```text
Input → Embedding + Positional Encoding
      → [Transformer Layer × 5]
      → Linear(vocab_size) → Predicted token

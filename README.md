# Natural-Language-Processing

## Natural-Language-Processing 정의
- 자연어 처리는 인간의 언어를 컴퓨터가 해석하고 처리할 수 있도록 하는 기술 분야다.
- 이 분야는 텍스트나 음성 데이터를 분석하고 이해하며, 필요에 따라 적절한 반응을 생성하는 것을 목표로 한다.
- NLP는 인공지능, 컴퓨터 과학, 언어학의 교차점에 위치해 있으며, 텍스트 분류, 감정 분석, 기계 번역 등 다양한 응용 분야를 포함한다.

## Natural-Language-Processing 과정
1. 데이터 전처리(Data Preprocessing)
- 텍스트 정규화(Text Normalization): 문장과 단어를 토큰화하고, 대소문자를 통일하며, 불용어 제거 등을 수행한다.
- 형태소 분석(Morphological Analysis): 단어를 기본 형태로 변환(예: "running" -> "run").
2. 특성 추출(Feature Extraction)
- 벡터화(Vectorization): 텍스트를 수치적 형태로 변환한다(예: Bag of Words, TF-IDF).
- 단어 임베딩(Word Embedding): 단어를 밀집 벡터로 표현한다(예: Word2Vec, GloVe).
3. 모델링(Modeling)
- 기계 학습(Machine Learning) 또는 딥러닝(Deep Learning) 모델을 사용하여 특정 작업을 수행한다.
4. 평가(Evaluation)
- 모델의 성능을 평가하며, 이를 통해 모델을 튜닝하고 개선한다.
5. 응용(Application)
- 개발된 모델을 실제 응용 프로그램에 통합한다.(예: 챗봇, 음성 인식 시스템)

## Natural-Language-Processing에 사용되는 딥러닝 기법
- 순환 신경망 (Recurrent Neural Networks, RNNs)
순환 신경망은 시퀀스 데이터를 처리하는 데 특화된 신경망의 한 종류이다.
RNN은 시간에 따라 정보를 기억하며, 각 시간 단계에서 입력을 받아 이전 단계의 정보를 반영하여 출력을 생성한다.
RNN은 자연어 처리(NLP)와 같이 순차적 정보가 중요한 분야에 주로 사용된다.
이러한 네트워크는 기본적으로 과거의 정보를 "기억"하고 현재의 입력과 결합하여 출력을 생성한다.
RNN은 다양한 구조를 가질 수 있으며, 단일 입력에서 여러 출력을 생성하는 'One to Many', 여러 입력에서 단일 출력을 생성하는 'Many to One', 여러 입력에서 여러 출력을 생성하는 'Many to Many' 등이 있다.
하지만 RNN은 계산이 느리고 미래의 입력을 고려하지 못하는 문제가 있다. 또, 'Vanishing Gradient' 문제(신경망이 학습되는 과정에서, 오차를 역전파하는 과정에서 그래디언트(경사)가 점점 줄어들어 결국 0에 가까워지는 현상)로 인해 학습이 어려울 수 있다.

- 트랜스포머(Transformer) 및 BERT와 GPT
트랜스포머와 BERT, GPT 같은 모델들은 현재 NLP 분야에서 매우 중요한 역할을 하고 있다.
이들 모델은 복잡한 자연어 처리 작업을 수행하기 위해 고안되었다.
트랜스포머는 자기 주의 메커니즘을 사용하여 전체 입력 시퀀스를 한 번에 처리하는 반면, BERT와 GPT는 각각 양방향 및 단방향 맥락을 이해하는 데 강점을 가지고 있다. 이러한 모델들은 전이 학습을 통해 다양한 NLP 작업에 적용될 수 있으며, 기존의 순환 신경망보다 더 효율적인 성능을 보여준다.
트랜스포머, BERT 및 GPT에 대한 자세한 내용은 해당 모델들을 소개하는 문헌 및 온라인 자료를 통해 더 깊이 있게 탐구할 수 있다.

## Natural-Language-Processing 관련 논문
- "Attention Is All You Need" by Vaswani et al. (2017): 이 논문에서는 트랜스포머(Transformer) 아키텍처가 처음 소개되었던 논문이다. 트랜스포머는 전통적인 RNN 및 LSTM에 의존하지 않고,
'자기 주의(Self-Attention)' 메커니즘을 활용하여 시퀀스 데이터를 처리한다. 이 새로운 접근 방식은 NLP 분야에서 중요한 발전을 이루었으며, 효율적인 병렬 처리와 빠른 학습 속도로 인해 다양한 언어 처리 작업에서 널리 채택되었다.
  
- "BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding" by Devlin et al. (2018): BERT(Bidirectional Encoder Representations from Transformers)는 텍스트의 양방향 맥락을 이해하는 데 초점을 맞춘 모델이다. BERT는 사전 훈련된 딥러닝 모델을 활용하여 다양한 NLP 작업에 적용될 수 있으며, 언어 이해에 있어서 기존 모델들보다 향상된 성능을 보여주었습니다. 이 논문은 NLP 분야에서 BERT가 어떻게 다양한 언어 처리 작업의 성능을 개선하는지에 대한 내용을 담고 있다.



# 6주차 개인 학습 정리

네이버 부스트캠프 AI Tech 2023. 12. 12. (월) - 2023. 12. 15. (금) 주간 학습 회고입니다.

## 종합 평가

| 항목           | 평가  | 비고                                                                                       |
| -------------- | ----- | ------------------------------------------------------------------------------------------ |
| 🧑‍🏫 강의 이해도 | ★★★★☆ | RecSys 분야의 비교적 최신 모델 및 논문들과, 실무에 적용되는 방법에 대한 종합적 이해도 상승 |
| 📝 과제/퀴즈   | ★★★★☆ | 대회 시작 이후 서버 환경 구축 및 모델 이해에 시간을 많이 쏟아 성능 최적화를 위해 추가 학습이 필요 |
| 🎯 목표 도달   | ★★★☆☆ | 성능 최적화 작업에 대한 팀원간의 서로 다른 의견 검증을 위한 추가적인 이론 공부가 필요 |

## Remote Config

팀원들과 환경 설정 중 버전 및 환경 통일을 위한 회의를 거쳐 다음 설정으로 확정함

```
pandas==1.5.3
numpy==1.23.5
seaborn==0.12.2
matplotlib==3.7.1
re==2.2.1
PIL== 9.4.0
requests== 2.31.0
scikit-learn==1.2.2
torch==2.0.1+cu118
scipy==1.11.3
xgboost==2.0.0
surprise==1.1.3
lightgbm==3.3.4
catboost==1.2.2
```

## 추가 학습 내용

최신 게재 논문에 대한 스터디

### A Lightweight Method for Modeling Confidence in Recommendations with Learned Beta Distributions
by Norman Knyazev (Radboud University) and Harrie Oosterhuis (Radboud University).

> Most recommender systems (RecSys) do not provide an indication of confidence in their decisions. Therefore, they do not distinguish between recommendations of which they are certain, and those where they are not. Existing confidence methods for RecSys are either inaccurate heuristics, conceptually complex or very computationally expensive. Consequently, real-world RecSys applications rarely adopt these methods, and thus, provide no confidence insights in their behavior. In this work, we propose learned beta distributions (LBD) as a simple and practical recommendation method with an explicit measure of confidence. Our main insight is that beta distributions predict user preferences as probability distributions that naturally model confidence on a closed interval, yet can be implemented with the minimal model-complexity. Our results show that LBD maintains competitive accuracy to existing methods while also having a significantly stronger correlation between its accuracy and confidence. Furthermore, LBD has higher performance when applied to a high-precision targeted recommendation task. Our work thus shows that confidence in RecSys is possible without sacrificing simplicity or accuracy, and without introducing heavy computational complexity. Thereby, we hope it enables better insight into real-world RecSys and opens the door for novel future applications.

### BVAE: Behavior-aware Variational Autoencoder for Multi-Behavior Multi-Task Recommendation
by Qianzhen Rao (Shenzhen University), Yang Liu (Shenzhen University), Weike Pan (Shenzhen University) and Zhong Ming (Shenzhen University).

> A practical recommender system should be able to handle heterogeneous behavioral feedback as inputs and has multi-task outputs ability. Although the heterogeneous one-class collaborative filtering (HOCCF) and multi-task learning (MTL) methods has been well studied, there is still a lack of targeted manner in their combined fields, i.e., Multi-behavior Multi-task Recommendation (MMR). To fill the gap, we propose a novel recommendation framework called Behavior-aware Variational AutoEncoder (BVAE), which meliorates the parameter sharing and loss minimization method with the VAE structure to address the MMR problem. Specifically, our BVAE includes address behavior-aware semi-encoders and decoders, and a target feature fusion network with a global feature filtering network, while using standard deviation to weigh loss. These modules generate the behavior-aware recommended item list via constructing better semantic feature vectors for users, i.e., from dual perspectives of behavioral preference and global interaction. In addition, we optimize our BVAE in terms of adaptability and robustness, i.e., it is concise and flexible to consume any amount of behaviors with different distributions. Extensive empirical studies on two real and widely used datasets confirm the validity of our design and show that our BVAE can outperform the state-of-the-art related baseline methods under multiple evaluation metrics.

### (Industry Report) Amazon.com Recommendations: Item-to-Item Collaborative Filtering

by Greg Linden, Brent Smith, and Jeremy York (Amazon.com)

> There are three common approaches to solving the recommendation problem: traditional collabora- tive filtering, cluster models, and search-based methods. Here, we compare these methods with our algorithm, which we call item-to-item collab- orative filtering. Unlike traditional collaborative filtering, our algorithm’s online computation scales independently of the number of customers and number of items in the product catalog. Our algo- rithm produces recommendations in realtime, scales to massive data sets, and generates high- quality recommendations.

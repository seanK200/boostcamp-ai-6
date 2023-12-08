# 5주차 개인 학습 정리

네이버 부스트캠프 AI Tech 2023. 12. 4. (월) - 2023. 12. 8. (금) 주간 학습 회고입니다.

## 종합 평가

| 항목           | 평가  | 비고                                                                                       |
| -------------- | ----- | ------------------------------------------------------------------------------------------ |
| 🧑‍🏫 강의 이해도 | ★★★★☆ | RecSys 분야의 비교적 최신 모델 및 논문들과, 실무에 적용되는 방법에 대한 종합적 이해도 상승 |
| 📝 과제/퀴즈   | ★★★★☆ | Model들 간의 특징 이해 부족으로 인한 퀴즈 오답 일부 발생으로 인한 복습 필요                |
| 🎯 목표 도달   | ★★★★☆ | 강의/과제에 대한 개인 목표치 달성 완료. 심화 과제 완료하지 못해 추가 학습 필요             |

## 피어 세션

팀원들과 함께 현재 학습 상황과 과제 현황, 질문사항들을 활발하게 공유하였음. 특히나, 이해가 잘 되지 않았던 부분은 자율적으로 직접 발표 형식으로 준비해 와서 팀원들 앞에서 설명하는 방식으로 피어 세션을 진행하여 이해가 되지 않던 부분을 스스로도 확실히 정리하고, 잘못 이해한 부분이 있다면 서로 바로잡아주는 방식의 세션을 진행하였음.

프로젝트에 관련된 결정을 해야 하는 시점이 다가옴에 따라, 수행할 프로젝트 내용에 대한 이야기를 나누기 시작하였음. 각자 과거 경험과 주요 관심사, 희망 주제 등을 공유하며 이야기를 나누었음.

## 학습 내용

- 컨텍스트 기반 추천(Context-aware Recommendation)
- 클릭률 예측(Click-throughout Rate Prediction, CTR Prediction)
- FM(Factorization Machine), FFM(Field-aware Factorization Machine)
- Boosting, GBM(Gradient Boosting Machine), XGBoost, LightGBM, CatBoost

### LinkedIn Engineering: CTR Prediction Model

$$
CTR = \frac{clicks}{impressions} \times 100\%
$$

[https://hyperconnect.github.io/2021/04/26/hakuna-recsys-gb.html](https://hyperconnect.github.io/2021/04/26/hakuna-recsys-gb.html)

![the challenges](https://content.linkedin.com/content/dam/engineering/site-assets/images/blog/posts/2022/08/adsctrmodel/image6.jpg)

> At LinkedIn, our ads business is powered by click-through-rate (CTR) prediction, a core machine learning model. CTR prediction estimates the probability of clicks between a LinkedIn member and a potential advertisement. That probability is then used for ads auctions, which decide the order of ads being displayed to members. A better CTR model can enhance the member and advertiser experience by bringing more relevant ads and more efficient advertiser budget spending.

[https://engineering.linkedin.com/blog/2022/challenges-and-practical-lessons-from-building-a-deep-learning-b](https://engineering.linkedin.com/blog/2022/challenges-and-practical-lessons-from-building-a-deep-learning-b)

### Predicting Ad Click-Through Rate with Random Forest

[https://www.analyticsvidhya.com/blog/2023/04/predicting-ad-click-through-rate-with-random-forest/](https://www.analyticsvidhya.com/blog/2023/04/predicting-ad-click-through-rate-with-random-forest/)

- How to find the features that affect the ad click-through rate prediction?
- How do you calculate the CTR score based on the number of users who either clicked on the ad?
- How to use Random Forest Classifier model to predict the ad click-through rate?

### Classification in Click-Through Rate Prediction in Display Advertising

[https://medium.com/analytics-vidhya/classification-in-click-through-rate-prediction-in-display-advertising-a487a03f8631](https://medium.com/analytics-vidhya/classification-in-click-through-rate-prediction-in-display-advertising-a487a03f8631)

#### Challenges in Multi-Field Categorical Dta

- 1- Feature interactions are prevalent and need to be specifically modeled.
- 2- Features from one field often interact differently with features from different other fields.
- 3- Potentially high model complexity needs to be taken care of.

> According to these mentioned problems, normally usual classification models won’t operate well enough on this kind of data. in this article, first of all, we will explain characteristics of our data set, second, we will implement some famous classification algorithms such as logistic regression, SVM, random forest, and so on.

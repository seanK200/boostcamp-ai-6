# 3주차 개인 학습 정리

네이버 부스트캠프 AI Tech 2023. 11. 20. (월) - 2023. 11. 24. (금) 주간 학습 회고입니다.

## 종합 평가

| 항목           | 평가  | 비고                                                                                     |
| -------------- | ----- | ---------------------------------------------------------------------------------------- |
| 🧑‍🏫 강의 이해도 | ★★★★☆ | CNN, RNN, Generative Model들에 대한 기본적인 이해 학습 완료                              |
| 📝 과제/퀴즈   | ★★★★☆ | Generative model의 probablistic analysis에 대한 이해 부족으로 발생한 퀴즈 오답 일부 발생 |
| 🎯 목표 도달   | ★★★★☆ | 강의/과제에 대한 개인 목표치 달성 완료. 심화 과제 완료하지 못해 추가 학습 필요           |

## 학습 내용

### MLP vs CNN

|              | MLP                              | CNN                          |
| ------------ | -------------------------------- | ---------------------------- |
| Input        | Vector                           | Vector & Matrics             |
| Network Type | Fully-connected                  | Spatially connected          |
| Problem      | Capable of non-linear problems   | Linear problems only         |
| Application  | Simple image classification, ... | Complex image classification |

#### Advantages of MultiLayer Perceptron Neural Network

- MultiLayer Perceptron Neural Networks can easily work with non-linear problems.
- It can handle complex problems while dealing with large datasets.
- Developers use this model to deal with the fitness problem of Neural Networks.
- It has a higher accuracy rate and reduces prediction error by using backpropagation.
- After training the model, the Multilayer Perceptron Neural Network quickly predicts the output.

#### Disadvantages of MultiLayer Perceptron Neural Network

- This Neural Network consists of large computation, which sometimes increases the overall cost of the model.
- The model will perform well only when it is trained perfectly.
- Due to this model’s tight connections, the number of parameters and node redundancy increases.

> [Reference](https://www.shiksha.com/online-courses/articles/understanding-multilayer-perceptron-mlp-neural-networks/)

### MLP vs. RNN vs. CNN

![MLP RNN CNN SVM](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FcEZJBF%2FbtqNpGOj3Ob%2Fzj6suBvXW1kK0IKy5SoEwk%2Fimg.png)

![MLP RNN CNN Comparison](https://av-eks-blogoptimized.s3.amazonaws.com/table.png)

### RNN (Recurrent Neural Network)

e.g. 텍스트 처리 시 텍스트 간의 연관성을 사용하여 분석

![RNN](https://cdn.analyticsvidhya.com/wp-content/uploads/2020/02/1d_POV7c8fzHbKuTgJzCxtA.gif)

![RNN](https://av-eks-blogoptimized.s3.amazonaws.com/The-standard-RNN-and-unfolded-RNN-300x131.png)

![RNN](https://av-eks-blogoptimized.s3.amazonaws.com/1a5EbLhyxbPR78PhiV5Esjg-300x10388108.png)

### CNN (Convolution Neural Network)

Feature Extraction --> **Feature Map**

![CNN Feature Map](https://av-eks-blogoptimized.s3.amazonaws.com/Untitled-Diagram.png)

Kernels (Filter)

![CNN Filter](https://cdn.analyticsvidhya.com/wp-content/uploads/2020/02/1BMngs93_rm2_BpJFH2mS0Q.gif)

> [Reference](https://www.analyticsvidhya.com/blog/2020/02/cnn-vs-rnn-vs-mlp-analyzing-3-types-of-neural-networks-in-deep-learning/)

## 기타 참고 자료

- [08-01 순환 신경망(Recurrent Neurla Network, RNN) - 딥러닝을 사용한 자연어 처리 입문 - 위키독스](https://wikidocs.net/22886)

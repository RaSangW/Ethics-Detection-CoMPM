# CoMPM을 이용한 한국어 텍스트의 비윤리적 대화 식별 개선(2023)
Improving Unethical Dialogue Identification in Korean Text using CoMPM(2023)


본 연구에서는 한국어를 중심으로 디지털 영역에서 비윤리적인 대화를 식별하는 작업에 화자의 사전 학습된 기억 추적을 이용한 맥락 모델링(Context Modeling with Speaker's Pre-Trained Memory Tracking, CoMPM) 모델을 적용합니다.
기존 접근 방식은 주로 영어로 제공되는 외부 구조화 데이터에 크게 의존하기 때문에 다른 언어에 적용하는 데 한계가 있습니다.
우리는 한국어 텍스트 윤리성 검증 데이터로 사전 학습된 모델인 KcELECTRA를 미세 조정하고 문맥과 사전 지식을 고려하는 CoMPM 접근법을 구현하여 이러한 한계를 해결했습니다.
그 결과 문맥이 텍스트 인식에 중요한 역할을 하며, 이는 짧은 디지털 교환에서도 마찬가지입니다.
F1 점수를 사용하여 문맥을 고려하지 않은 모델과 우리 모델의 성능을 비교한 결과, 0.61에서 0.647로 크게 개선된 것으로 나타났습니다.
문맥 변화 시 부정확한 예측, 제한된 데이터 세트로 인한 과적합 가능성 등의 한계에도 불구하고 이러한 결과는 향후 문맥 모델링 개선, 데이터 확장, 모델 단순화 등을 통해 모델 성능을 향상시킬 수 있는 유망한 연구 방향을 제시합니다.

##### 모델 구조
<img width="600" alt="Architecture" src="https://github.com/RaSangW/Ethics-Detection-CoMPM/assets/52962920/bb2c9e4f-850e-441e-901c-d13dd11bf026">

##### 대화문 모델 에시
<img width="600" alt="Dialogue" src="https://github.com/RaSangW/Ethics-Detection-CoMPM/assets/52962920/a2eeb58c-ab97-438e-b651-4053f08db0ea">

##### 파일 설명
Model_CoMPM.ipynb: 사전학습 모델을 CoM과 PM구조를 결합한 모델에 대입하여 비윤리적 대화를 판별합니다. 

Model_CoM.ipynb: 사전학습 모델을 CoM구조에 대입하여 비윤리적 대화를 학습시킵니다. 

Model_PM.ipynb: 사전학습 모델을 PM구조에 대입하여 비윤리적 대화를 학습시킵니다. 

Model_KcELECTRA.ipynb: KcELCTRA를 사용하여, 비윤리적 대화를 학습시킵니다. 

NLP_Preprocessing.ipynb: 전처리 과정입니다. 


---
자세한 내용은 pdf를 참조해주시기 바랍니다.

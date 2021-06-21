## **머신러닝 시스템의 종류**   
### + 사람의 감독하에 훈련되는 것인가 아닌가(지도, 비지도, 준지도, 강화학습)
### + 실시간으로 점진적인 학습을 하는가 아닌가(온라인 학습, 배치학습)
### + 단순하게 알고 있는 데이터 포인트와 새 데이터 포인트를 비교하는 것인지 아니면 훈련 데이터셋에서 패턴을 발견하여 예측 모델을 만드는지(사례 기반 학습과 모델 기반 학습)
-------------------------
#### 1. 지도학습 : 알고리즘에 주입하는 훈련 데이터에 레이블이라는 원하는 답이 포함된다.
>* 분류가 전형적인 지도학습이며 예측 변수라 부르는 특성을 사용해 타깃수치를 예측하는 것으로 회귀라고도 부른다.
#### 2. 비지도 학습 : 훈련 데이터에 레이블이 없다. 시스템이 도움 없이 학습한다.
>* 군집은 데이터가 어떤 그룹에 속하는지 알고리즘을 알려줄 데이터 포인트를 찾기 위해 알고리즘이 연결고리를 찾는 것으로 계층 군집 알고리즘을 사용하면 더 작은 그룹으로 세분화 가능
>* 시각화는 고차원 데이터를 도식화 가능한 2D나 3D로 만들어 어떻게 조직되었는지와 패턴을 발견할 수 있다. 
>* 차원 축소는 시각화와 비슷한 작업으로 너무 많은 정보를 잃지 않으면서 데이터를 간소화 한다.
>* 이상치 탐지는 샘플을 보고 정상 데이터인지 이상치인지 판단함
>* 특이치 탐지 : 훈련 세트에 있는 모든 샘플과 달라 보이는 새로운 샘플을 탐지하는 것이 목적
>* 연관 규칙 학습은 대량의 데이터에서 특성 간의 흥미로운 관계를 찾는 것
#### 3. 준지도 학습 : 알고리즘이 일부만 레이블이 있는 데이터를 다룰 수 있는것.(준지도 학습은 지도와 비지도 학습의 조합으로 이루어짐)
>* 심층 신뢰 신경망은 제한된 볼츠만 머신이라는 비지도 학습이 기초하고 전체 시스템이 지도 학습 방식으로 세밀하게 조정됨
#### 4. 강화 학습 : 학습하는 시스템을 에이전트라 부르며 환경을 관찰, 행동해서 결과로 보상과 벌점을 받는다.
#### 5. 배치 학습 : 먼저 시스템을 훈련시키고 제품 시스템에 적용하면 더이상 학습 없이 실행됨. 학습한 것을 적용만 하며 오프라인 학습이라고도 한다.
#### 6. 온라인 학습 : 데이터를 순차적으로 미니배치라 부르는 작은 단위로 주입하여 시스템을 훈련시킨다. 학습 단계가 빠르고 비용이 적어 데이터가 도착하는데로 학습 가능.
>* 온라인 학습은 빠른 변화에 스스로 적응해야 하는 시스템에 적합하다
>* 아주 큰 데이터셋을 학습하는 시스템에도 적용 가능(외부 메모리 학습)
>* 학습률은 시스템이 데이터에 얼마나 빨리 적응하는가로 학습률이 높으면 빠르게 적응하지만 예전 데이터를 잊고, 낮으면 느리게 학습하지만 데이터 포인트에 덜 민감해진다.
#### 7. 사례 기반 학습 : 시스템이 훈련 샘플을 기억함으로 학습한다. 그리고 유사도 측정을 사용해 새 데이터와 학습한 샘플을 비교하는 식으로 일반화 함.
#### 8. 모델 기반 학습 : 샘플들의 모델을 만들어 예측에 사용하는 것.
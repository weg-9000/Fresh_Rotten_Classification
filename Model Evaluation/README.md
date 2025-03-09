# img src="https://github.com/weg-9000/image/blob/main/logo_mini.PNG" alt="Example Image" width="32" height="32" style="vertical-align: middle;"> AzureCustomVision vs ResNet vs DenseNet

## 📝개요

AzureCustomVision, ResNet, DenseNet 3가지 모델에 대한 [Precision, Recall, Accuracy] 3가지 성능을 평가하고
Bar chart 및 Radar chart로 시각화

## 🛠️각 모델 성능자료 만들기

1. 실시간 유추 파이프라인으로 만든 모델을 선택
2. 해당 모델 작업
3. evaluate model Metric
4. 사용자 지정 차트 만들기 [막대형 차트 -> x축: 단계 -> y축: macro_precision, macro_recall, overall_accuracy -> 로그 y축]
5. tsv파일 저장
   (Azure CV는 tsv로 제공되지 않기 때문에 3가지 metric에 대하여 수기작성)

## ⚙️분석

Label

1. ResNet - Densenet
2. AzureCV - Densenet
3. AzureCV - ResNet

수치간의 차이가 굉장히 작다. 즉, 수치로써 성능차이를 보기에는 큰 무리가 있어보인다.
매우 작은 수치로 차이를 보여주기 위해 2모델의 성능의 차이를 하나의 라벨로 지정

(바 차트의 특이사항으로 값이 매우 작거나 0이면 △>0 , ▽<0 ━ = 0 의 기호를 이용하여 가시성 높임)

## 🧠평가

ACV가 전체적으로 (작은 수치) 성능이 좋았음. 이는 ACV에 대한 Resnet model이 알려져 있지 않으며
ResNet과 AlexNet을 사용하며 더 복잡한 구조를 가지고 있을 것으로 보인다.

DenseNet과 Resnet비교에서 데이터의 양과 크기가 굉장히 중요함을 알 수 있었다.
데이터의 양이 적으면 깊은 모델에서는 과적합으로 인해 Densenet보다 성능이 떨어짐을 보여준다.

resnet의 다양한 모델 resnet18, resnet50, resnext50, resnext101을 비교해본 결과
데이터에 따라 선택해야하는 모델이 달라짐을 확인 가능했음

이미지 학습모델에서는
앞서 말했듯이 수치적차이가 소수점4자리 이하이기에 큰 의미가 없다.

여기서 가장 중요한 것은 어떤 이미지를 학습시키고 어떤 이미지를 테스트하느냐에 따라
결과가 큰 차이를 보여준다.

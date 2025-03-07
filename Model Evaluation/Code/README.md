# 📊 모델 성능 비교 및 시각화

## 📌 개요

이 스크립트는 **Densenet**, **ResNet**, **Azure Custom Vision(AzureCV)** 모델의 성능을 비교하고 시각화하는 것을 목표로 합니다.
각 모델의 Precision, Recall, Accuracy 값을 비교하여 차이를 분석하고, 이를 **막대 그래프**와 **레이더 차트**로 시각화합니다.

---

## 🛠️ 설치 및 요구 사항

스크립트를 실행하기 전에 다음 라이브러리를 설치해야 합니다:

```bash
pip install pandas numpy matplotlib
```

---

## 🚀 사용 방법

### 1️⃣ 성능 데이터 파일 준비

각 모델의 성능 지표가 포함된 **TSV 파일**을 준비해야 합니다.
예제 파일 구조는 다음과 같습니다:

```plaintext
metric	value
Macro_Precision	0.85
Macro_Recall	0.83
Overall_Accuracy	0.87
```

- `Densenet`: `densenet.tsv`
- `ResNet`: `resnet18.tsv`
- `AzureCV`: `ACV.tsv`

> 🔹 TSV 파일은 **탭(\t) 구분자**를 사용합니다.

### 2️⃣ 스크립트 실행

파일 경로를 설정하고 스크립트를 실행하면 모델 간 성능 차이를 분석하고 시각화할 수 있습니다.

#### ✅ 주요 기능

- `Macro_Precision`, `Macro_Recall`, `Overall_Accuracy` 비교
- **Densenet을 기준으로** 다른 모델들과의 차이 계산
- **막대 그래프**로 차이값을 표시 (양수=파랑, 음수=빨강)
- **레이더 차트**로 성능 차이 시각화

---

## 📊 시각화 예제

### 1️⃣ 모델 간 성능 차이 (막대 그래프)

각 모델의 성능 차이를 나타내며, 색상을 통해 차이를 직관적으로 확인할 수 있습니다.

| Metric           | ResNet - Densenet | AzureCV - Densenet | AzureCV - ResNet |
| ---------------- | ----------------- | ------------------ | ---------------- |
| Macro_Precision  | +0.02             | -0.01              | -0.03            |
| Macro_Recall     | -0.01             | +0.03              | +0.04            |
| Overall_Accuracy | +0.01             | +0.02              | +0.01            |

> 🔹 **차이가 매우 작은 값(0.001 이하)은 특수 기호(△ ▽ ━)로 표시**

### 🔹 예제 그래프

<img src="bar_chart_example.png" alt="Bar Chart Example" width="600">

---

### 2️⃣ 모델 간 성능 차이 (레이더 차트)

모델 간 성능 차이를 **레이더 차트**로 나타내어 각 성능 지표의 상대적 변화를 시각적으로 확인할 수 있습니다.

### 🔹 예제 그래프

<img src="radar_chart_example.png" alt="Radar Chart Example" width="600">

---

## 📢 추가 정보

- 성능 데이터는 **Densenet을 기준**으로 비교됩니다.
- 데이터가 없는 경우, 스크립트 실행 시 오류가 발생할 수 있으니 필수 데이터가 포함되었는지 확인하세요.
- `matplotlib`을 사용하여 시각화하며, 그래프를 저장하려면 `plt.savefig('파일이름.png')`을 추가하세요.

---

## 🔥 실행 예제

```bash
python model_Evaluation.py
```

✅ 실행하면 모델 간 성능 차이를 분석하고, 결과를 시각화합니다!

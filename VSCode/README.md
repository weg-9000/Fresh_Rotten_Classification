# <img src="https://github.com/weg-9000/image/blob/main/logo_mini.PNG" alt="Example Image" width="32" height="32" style="vertical-align: middle;"> ResNet을 활용한 과일 및 채소 이미지 분류

## 📌 프로젝트 개요

이 프로젝트는 **ResNet**을 활용하여 **과일과 채소의 종류 및 신선도 분류**를 수행하는 AI 모델을 학습 및 평가하는 것을 목표로 합니다.

머신러닝 모델을 활용해 **3단계 분류**를 진행하며, 이미지 데이터를 전처리하고 최적의 성능을 도출합니다. 🚀

---

## 🌟 주요 기능

✅ **정규화 및 리사이징을 통한 이미지 전처리** 📷

✅ **과일/채소 분류를 위한 ResNet 모델 학습 및 평가** 🏆

✅ **3단계를 통한 정교한 분류 과정** 🔍

- 🥦 **1단계:** 과일 vs. 채소
- 🍏 **2단계:** 신선도 분류 (Fresh/Rotten)
- 🍎 **3단계:** 개별 품목 인식 (예: Apple, Tomato, Carrot)

✅ **결과 시각화 및 이미지 저장 기능 제공** 🖼️

---

## ⚙️ 환경 설정

### 🔧 필수 요구사항

🛠️ **Python 3.9 이상**

🛠️ **Jupyter Notebook 설치 필요**

---

## 📂 프로젝트 구조

```
VSCode/
│
├── Models/           
│   ├── 1_Fruit_Veg.ipynb  
│   ├── 2_1_Fruit_fresh_rotten.ipynb     
│   ├── 2_2_Veg_fresh_rotten.ipynb  
│   ├── 3_1_Fruit_8class.ipynb
│   ├── 3_2_Veg_14class.ipynb   
│
├── Evalution/               
│   └── Evaluation.ipynb          
│
└── README.md        
```

---

## 🛠️ 실행 방법

### 1️⃣ 단계별 모델 생성 및 저장

```bash
jupyter notebook Models/1._Fruit_Veg.ipynb
```

🔹 **Jupyter Notebook 실행**: 해당 노트북을 실행하여 총 3단계의 학습을 진행합니다.

🔹 **학습 완료 후 모델 가중치 파일이 자동 저장됩니다.**

### 2️⃣ 예측 및 평가

🔹 **Jupyter Notebook 실행**: `Evaluation.ipynb` 노트북을 실행하여 모델을 로드하고 예측을 진행합니다.

🔹 **저장된 모델을 활용하여 과일/채소 → 신선도 → 개별 품목 순으로 결과를 확인할 수 있습니다.**

---

## 📊 결과 예시

✅ **1차 분류 (과일/채소 판별)** 🍉🥕

```plaintext
Step 1 - Category: Vegetable (60.29%)
```

🍏 **2차 분류 (신선도 판별)** 🥦

```plaintext
Step 2 - Fresh/Rotten: Fresh (76.62%)
```

🍎 **3차 분류 (품목 분류)** 🍅

```plaintext
Step 3 - Final Category: Tomato (63.60%)
```

---

## ⚠️ 주의사항

🚨 **이미지 크기 조정 필수:** 224x224 크기로 조정하여 최적화된 모델 성능 유지

🚨 **고화질 이미지 권장:** 선명한 이미지일수록 높은 정확도를 보장 🎯


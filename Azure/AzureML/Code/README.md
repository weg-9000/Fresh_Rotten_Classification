# 🍎 Azure Machine Learning Designer를 활용한 과일 및 채소 이미지 분류

## 📌 프로젝트 개요

이 프로젝트는 **Azure Machine Learning Designer**를 활용하여 **5개의 모델을 파이프라인으로 설정**하고, API를 연동하여 **과일 및 채소의 종류 및 신선도를 분류**하는 기능을 제공합니다.

Azure의 GUI 기반 설계를 활용하여 **직관적으로 모델을 구성**할 수 있으며, API를 통해 **실시간 이미지 분류**가 가능합니다. 🏆

---

## 🚀 주요 기능

✅ **Azure Machine Learning Designer를 활용한 프로젝트 파이프라인 설정**  
✅ **과일/채소 분류 및 실시간 API 호출을 통한 분석**  
✅ **이미지 변환 (PNG → JPG) 및 리사이징 기능**  
✅ **3단계 분류: 과일/채소 → 신선도 → 개별 품목 인식**  
✅ **분류 결과 출력 및 이미지 저장**

---

## ⚙️ 환경 설정

### 필수 요구사항

🛠 **Python 3.9 이상**  
🛠 **Azure Machine Learning Designer 계정 및 구독**  
🛠 **Azure API Endpoint 및 Key 설정**

### 프로젝트 구조

```
Azure_ML_Classification/
│
├── src/               # 소스 코드 디렉토리
│   ├── main.py        # 과일/채소 이미지 분류 실행 코드
│
└── README.md          # 프로젝트 설명서
```

---

## 🔧 실행 방법

### 1️⃣ Azure Machine Learning Designer 설정

1. **Azure Portal**에서 **Machine Learning** 서비스를 생성합니다.
2. **Designer** 화면에서 **5개 모델을 포함한 파이프라인을 설정**합니다.
3. **API Endpoint를 생성하고 Key를 발급받습니다.**

### 2️⃣ Python 실행

```sh
python src/main.py
```

- `IMAGE PATH`에 분석할 이미지 경로를 입력합니다.
- API를 호출하여 **과일/채소 → 신선도 → 개별 품목** 순으로 분류합니다.
- 결과를 터미널에서 확인할 수 있습니다.

---

## 📊 결과 예시

### 🥝 1차 분류 (과일/채소 판별)

```
Step 1 - Category: Fruit (95.2%)
```

### 🍏 2차 분류 (신선도 판별)

```
Step 2 - Fresh/Rotten: FRESH (87.3% FRESH, 12.7% ROTTEN)
```

### 🍎 3차 분류 (품목 분류)

```
Step 3 - Final Category: Apple (92.5%)
```

### 🖼️ 이미지 출력

분류한 이미지를 화면에 출력하고 저장할 수 있습니다.

---

## ⚠️ 주의사항

🔹 **이미지 크기 조정**: 224x224 크기로 조정하여 API 호출 최적화  
🔹 **API 호출 제한**: Azure의 호출 제한을 고려하여 사용해야 함  
🔹 **고화질 이미지 권장**: 선명한 이미지일수록 정확도가 향상됨

📩 문의 사항이 있으면 언제든지 연락 주세요! 😊🚀

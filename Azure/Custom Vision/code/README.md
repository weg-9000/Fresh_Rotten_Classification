# 🧠 Azure Custom Vision api연동

## 📝 개요

Azure Custom Vision API를 활용하여 과일 및 채소의 상태와 종류를 분석하는 이미지 분류 모델을 구축하였습니다. 본 프로젝트는 사용자가 업로드한 이미지를 분석하여 해당 과일 또는 채소의 종류와 신선도를 예측하는 기능을 제공합니다.

## 🚀 주요 기능

✅ **Azure Custom Vision API 연동을 통한 이미지 분석**  
✅ **총 5가지 이미지 분류 모델 개발 및 API 연동**:

1. **과일 및 채소 분류 (1-1)**
2. **과일 썩음 판별 (2-1)**
3. **채소 썩음 판별 (2-2)**
4. **과일 종류 분류 (3-1)**
5. **채소 종류 분류 (3-2)**

✅ **업로드된 이미지를 분석하여 예측된 결과 반환**  
✅ **Python을 활용한 API 호출 및 결과 처리**

## ⚙️ 환경 설정

### 🔹 필수 요구사항

- Python 3.9 이상
- Azure Custom Vision Subscription

### 🔹 필요한 패키지 설치

```bash
pip install -r requirements.txt
```

## 📁 프로젝트 구조

```
custom_vision_project/
│
├── data/              # 테스트용 이미지 데이터
├── AzureCV.py         # 모델 구축 및 실행 코드
├── README.md          # 문서
└── requirements.txt   # 필요한 패키지 목록
```

## 🛠️ 모델 테스트 방법

1. **Azure 포털에서 Custom Vision 생성**
2. **다중 클래스 분류 모델 5개 생성**
3. **각 카테고리(신선함/썩음, 종류)에 맞게 데이터 라벨링**
4. **데이터 학습 진행**
5. **각 모델의 API 키 및 엔드포인트 확보**
6. **AzureCV.py 실행하여 결과 확인**

```bash
python AzureCV.py
```

## ⚠️ 주의사항

### 📌 데이터

- 저작권 문제가 없는 이미지 사용 필수
- 한 이미지에 한 가지 과일 또는 채소만 포함될 것

### 📌 Microsoft Azure 관련

- API 키 및 엔드포인트를 안전하게 보관할 것

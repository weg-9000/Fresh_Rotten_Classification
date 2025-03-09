# <img src="https://github.com/weg-9000/image/blob/main/logo_mini.PNG" alt="Example Image" width="32" height="32"> Azure Custom Vision을 활용한 과일 및 채소 이미지 분류

## 📌 프로젝트 개요
이 프로젝트는 **Azure Custom Vision API**를 이용하여 과일 및 채소 이미지를 분석하고 **신선도 및 종류를 예측**하는 프로그램입니다.

총 5개의 모델을 활용하여 다음과 같은 기능을 수행합니다:
1. **과일 vs 채소 분류 (1차 분류)**
2. **신선도 판별 (2차 분류)**
   - 신선한(FRESH)
   - 중간 상태(MILD)
   - 썩은(ROTTEN)
3. **종류 분류 (3차 분류)**
   - 과일 종류
   - 채소 종류

## 🚀 주요 기능
✅ **Azure Custom Vision API를 활용한 이미지 분석**  
✅ **과일 및 채소 자동 분류**  
✅ **신선도 판별 및 상세 정보 제공**  
✅ **PIL 및 Matplotlib을 이용한 이미지 시각화**  

---

## ⚙️ 환경 설정

### 🔹 필수 요구사항
- Python 3.9 이상
- Azure Custom Vision 구독
- 필요한 Python 패키지 설치

```bash
pip install -r requirements.txt
```

### 🔹 프로젝트 구조
```
custom_vision_project/
│
├── src/               # 소스 코드 디렉토리
│   ├── main.py        # 이미지 분석 실행 코드
│   ├── utils.py       # 보조 함수 모음
│
├── README.md          # 프로젝트 설명
└── requirements.txt   # 필요 패키지 목록
```

---

## 🛠️ 실행 방법

### 1️⃣ **Azure Custom Vision 설정**
- Azure Portal에서 **Custom Vision 서비스**를 생성합니다.
- 필요한 **API Key와 엔드포인트** 정보를 확보합니다.
- 각 모델의 **Project ID 및 Model Name**을 설정합니다.

### 2️⃣ **이미지 분석 실행**

```bash
python main.py
```

- `IMAGE PATH`에 분석할 이미지의 경로를 입력합니다.
- 프로그램이 Custom Vision API를 호출하여 분석 결과를 출력합니다.

---

## 📊 결과 예시
### 1️⃣ 1차 분류 (과일/채소 판별)
```
1차 분류 결과: Fruit (95.2%)
```

### 2️⃣ 신선도 판별
```
신선도 판별: FRESH (87.3% FRESH, 12.7% ROTTEN)
```

### 3️⃣ 종류 분류
```
종류 분류: Apple (92.5%)
```

### 4️⃣ 이미지 출력
분석한 이미지를 화면에 출력합니다.

---

## ⚠️ 주의사항
- 분석할 이미지는 **고해상도**일수록 정확도가 높아집니다.
- **Azure Custom Vision API의 호출 제한**을 확인하세요.
- 모델 성능을 개선하려면 **더 많은 학습 데이터를 추가**해야 합니다.

---

## 📌 향후 개선 사항
🔹 **모델 성능 개선**: 추가적인 데이터 수집 및 재학습 진행 

---

## 💡 라이선스
이 프로젝트는 MIT 라이선스를 따릅니다. 자유롭게 수정 및 활용하실 수 있습니다. 😊

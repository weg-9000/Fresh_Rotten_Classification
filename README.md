# 🍏 Fresh & Rotten Classification

이 프로젝트는 **과일과 채소의 신선도를 분류하고, 종류를 식별**하는 시스템입니다. **Azure ML, Azure Custom Vision, VSCode(ResNet)**를 활용하여 3단계 분류 작업을 수행합니다.


## 📌 프로젝트 기능 

총 5개의 모델을 활용하여 다음과 같은 기능을 수행합니다:

1. **과일 vs 채소 분류 (1차 분류)** 🍇🥦
2. **신선도 판별 (2차 분류)**
   - 신선한(FRESH) 🍏
   - 중간 상태(MILD) 🥬
   - 썩은(ROTTEN) 🍌
3. **종류 분류 (3차 분류)**
   - 과일 종류 🍓🍊
   - 채소 종류 🥕🌽


## 🧑‍💻 기술 스택
✅ **Azure ML**: 모델 학습을 위한 플랫폼
✅ **Azure Custom Vision**: 이미지 인식 모델 개발   
✅ **ResNet**: 이미지 분류를 위한 심층 신경망 모델    

---


## ⚙️ 필수 요구사항
- Azure Custom Vision, ML 구독
- Python 3.9 이상
- 필요한 Python 패키지 설치


### 🔹 프로젝트 구조
```
Fresh_Rotten_Classification/
│
├── Azure/               
│   ├── AzureML      
│   └── Custom Vision     
│
├── Data/
│   ├── Dataset     
│   └── Preprocessing       
│
├── Model Evaluation/    
│   ├── Metric_Evaluation      
│   └── Preprocessing      
│
├── VSCode/    
│   ├── Models     
│   └── Evaluation    
│
├── Unity/      
│
└── README.md    
```

---

# ![logo](https://github.com/weg-9000/image/blob/main/logo_mini.PNG)  프로젝트 개요

이 리포지토리는 두 가지 주요 프로젝트로 구성되어 있습니다:

1. **Azure Custom Vision을 활용한 과일 및 채소 이미지 분류**
2. **DenseNet/ResNet 모델을 활용한 이미지 분류 파이프라인**

---

## 1. Azure Custom Vision을 활용한 과일 및 채소 이미지 분류

이 프로젝트는 Azure Custom Vision API를 사용하여 과일과 채소를 **신선도** 및 **종류**에 따라 자동 분류합니다.

### 주요 기능:

- **과일 vs 채소 분류**
- **신선도 판별**: 신선한, 중간 상태, 썩은
- **종류 분류**: 과일/채소의 종류 구분

### 기술 스택:

- Azure Custom Vision API
- Python (PIL, Matplotlib)

---

## 2. DenseNet/ResNet 모델을 활용한 이미지 분류 파이프라인

이 프로젝트는 DenseNet 또는 ResNet 모델을 사용하여 이미지 분류 모델을 훈련하고 평가하는 머신 러닝 파이프라인입니다.

### 주요 단계:

1. 데이터셋 로드 및 변환
2. 훈련, 검증, 테스트 데이터 분할
3. 모델 훈련 및 평가

### 기술 스택:

- Python
- DenseNet, ResNet (PyTorch/TensorFlow)

---

## 📊 프로젝트 구조

### 1. **Azure Custom Vision을 활용한 과일 및 채소 이미지 분류**
```
Azure AI CustomVision/
├── code/
| ├ AzureCV.ipynb
| └── README.md
└── README.md
```
### 2. **DenseNet/ResNet 모델 훈련 및 평가**
```
Azure ML/
├── code/
| ├ MLDesigner.ipynb
| └── README.md
└── README.md
```
---

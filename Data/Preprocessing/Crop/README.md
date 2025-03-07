# 🖼️ 이미지 배경 제거 및 리사이즈

## 📌 개요

이 스크립트는 OpenCV의 GrabCut 알고리즘을 활용하여 이미지의 배경을 제거하고, 지정된 크기로 리사이즈하여 흰색 배경으로 저장하는 기능을 제공합니다. 기계 학습, 프레젠테이션, 제품 사진 등 다양한 용도로 활용할 수 있습니다.

## 🛠️ 설치 및 요구 사항

### 필수 라이브러리

- OpenCV (cv2)
- NumPy (numpy)
- PIL (Pillow)

다음 명령어를 실행하여 라이브러리를 설치하세요:

```bash
pip install opencv-python-headless numpy pillow
```

## 🚀 사용 방법

### 1. 입력 및 출력 폴더 설정

처리할 이미지가 있는 폴더와 결과를 저장할 폴더 경로를 지정합니다.

```python
input_folder = "C:/path/to/input"
output_folder = "C:/path/to/output"
```

### 2. 이미지 처리

- 입력 폴더에서 PNG, JPG, JPEG 이미지를 필터링합니다.
- GrabCut 알고리즘을 사용하여 배경을 제거하고 흰색 배경을 추가합니다.
- 이미지를 600x600 픽셀로 리사이즈합니다.
- DPI를 300으로 설정하여 저장합니다.

## 🎉 결과 예시

- 처리된 이미지는 출력 폴더에 저장됩니다.
- 각 이미지가 처리될 때 완료 메시지가 출력됩니다.

✅ **Processed and saved: C:/path/to/output/image.png**

### 🎊 모든 이미지 처리 완료!

# Snap Classify

**Snap Classify**는 카메라를 사용하여 실시간으로 객체를 인식하고 분류할 수 있는 Android 애플리케이션입니다. 이 프로젝트는 TensorFlow Lite 기반의 딥러닝 모델을 활용하여 경량화된 실시간 객체 감지를 제공합니다. 심플하고 모던한 UI와 강력한 성능으로 다양한 사용 사례에 적용할 수 있습니다.

---

## 주요 기능

1. **실시간 객체 감지 및 분류**
   - 카메라를 통해 실시간으로 객체를 탐지하고 분류합니다.
2. **경량화 모델 사용**
   - TensorFlow Lite를 사용하여 모바일 환경에서 빠르고 효율적인 성능을 제공합니다.
3. **모던한 UI**
   - 깔끔한 검은색 테마와 사용자 친화적인 디자인.
4. **플러그앤플레이 지원**
   - 설정 없이 바로 실행 가능한 구조.

---

## 사용된 모델과 데이터셋

1. **사용된 모델**
   - **MobileNet SSD**: 경량화된 객체 감지 모델로, 모바일 환경에서 빠른 감지 성능을 제공합니다.
   - **TensorFlow Lite 모델**: MobileNet SSD 모델을 TFLite로 변환하여 사용.

2. **데이터셋**
   - **COCO Dataset**: 다양한 객체 감지를 위한 사전 학습 데이터셋으로, 80개 이상의 클래스(예: 사람, 자동차, 동물 등)를 포함합니다.

---

## 프로젝트 구조

```
snap-classify/
├── app/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/org/tensorflow/lite/examples/detection/
│   │   │   │   ├── DetectorActivity.java    # 메인 액티비티
│   │   │   │   ├── TFLiteObjectDetectionAPIModel.java  # 모델 로딩 및 감지 처리
│   │   │   ├── res/
│   │   │   │   ├── layout/
│   │   │   │   │   ├── activity_camera.xml  # UI 레이아웃
│   │   │   │   ├── drawable/  # 아이콘 및 그래픽 리소스
│   │   ├── assets/
│   │       ├── detect.tflite    # 객체 감지 모델
│   │       ├── labelmap.txt     # 객체 분류 라벨
├── build.gradle
└── README.md
```

---

## 주요 파일 설명

1. **DetectorActivity.java**
   - 카메라와 객체 감지 모델을 연결하여 실시간 결과를 화면에 표시합니다.
2. **TFLiteObjectDetectionAPIModel.java**
   - TensorFlow Lite 모델을 로드하고 객체 감지 및 분류 작업을 처리합니다.
3. **activity_camera.xml**
   - 앱의 UI 레이아웃을 정의한 파일.
4. **detect.tflite**
   - MobileNet 기반 사전 훈련된 TensorFlow Lite 모델.
5. **labelmap.txt**
   - 객체 분류에 사용되는 라벨 목록.

---

## 사용된 기술 스택

- **Android**
- **TensorFlow Lite**
- **CameraX**
- **Java**

---

## 시연 영상


https://github.com/user-attachments/assets/3ba0d2eb-7f9a-41c0-bd33-269060b1b4a6



## 라이선스

이 프로젝트는 [MIT License](LICENSE)에 따라 라이선스가 부여됩니다.

---

## 문의

- 개발자: [dustin0618](https://github.com/dustin0618)
- 이메일: [dustin0618@example.com](mailto:dustin0618@example.com)


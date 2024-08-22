train과 Test의 분포가 다름.
1. 2개의 음성 데이터 섞음
2. speaker diarization(화자가 몇명인지 판별)

speaker diarization을 위해 pyannote/speaker-diarization-3.1 모델 사용
audio deepfake detection을 위해 AASIST모델 사용

speaker diarization 모델의 평가를 위해 1200 여개의 unlabeled data에 대해 화자가 몇명 있는지 라벨링

Domain Adaptation을 위해 Smooth Adversarial Training기법을 사용

최종 inference에서 eval metric의 score를 높이기 위해 Postprocessing.

자세한 내용은 pdf, pptx에 있습니다.
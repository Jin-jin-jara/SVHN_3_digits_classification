# Small-Project1 : two digits with blank classification

사이킷런에서 기본적으로 제공하는 load_digits 데이터셋을 가공하여 새 데이터 셋을 만들고, CNN 모델에 학습시켜 예측해보겠습니다. <br>

- 목적 : 이번 프로젝트에서는 간편하게 사용하던 keras의 Sequential 모델이 아닌 아닌 tensorflow를 이용한 전문가용 모델을 직접 구축해 데이터를 학습시키고 예측해보려고 합니다.<br>
"The Keras functional and subclassing APIs provide a define-by-run interface for customization and advanced research. Build your model, then write the forward and backward pass. Create custom layers, activations, and training loops." <br>
- 데이터셋 : load_digits는 8x8픽셀의 숫자(0-9) 이미지 데이터셋입니다. 이번 프로젝트에서는 기본 이미지를 사용하는 것이 아니라 8x8 이미지를 좌우로 붙여 8x16픽셀의 새로운 데이터셋으로 만들겠습니다. 새로운 이미지 데이터셋에는 0-9까지 숫자뿐만 아니라 한쪽은 아무 숫자도 없는 비어있는 이미지도 존재합니다.<br>
- 모델 : CNN 모델은 keras.Sequential() 모델과 <a href="https://www.tensorflow.org/tutorials/quickstart/advanced?hl=ko">tensorflow 전문가용 모델</a> 두 버전으로 만들어보겠습니다.


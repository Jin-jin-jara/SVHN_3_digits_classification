# Small-Project : SVHN 3 digits classification

SVHN 3 digits classification 프로젝트에서는 간편하게 사용하던 keras의 Sequential 모델이 아닌 아닌  <a href="https://www.tensorflow.org/tutorials/quickstart/advanced?hl=ko">tensorflow 전문가용 모델</a>을 직접 구축해 데이터를 학습시키고 예측해보려고 합니다. 또 정제된 기본 데이터가 아닌 노이즈가 많은 실제 데이터를 사용해 예측을 진행하겠습니다.<br><br>

이번 프로젝트에서 사용할 데이터셋은 <a href="http://ufldl.stanford.edu/housenumbers/">Google Street View House Number</a>입니다. 구글이 촬영한 street view에서 집 번호만 추출한 데이터입니다. 다만 SVHN 전체 데이터셋(Full Numbers)은 너무 용량이 커 사용하기 어렵기 때문에 각 숫자 이미지를 잘라놓은 Cropped Digits 데이터 셋(그 중에서도 test데이터셋만을)을 사용하겠습니다. Cropped Digits 데이터셋은 하우스 넘버 이미지를 한 자리 수로 잘라놓은 데이터셋입니다. 한 자리수 이미지들을 붙여 세 자리로 만든 후 기계를 학습시키고 예측하도록 하겠습니다.<br>

이 프로젝트의 목표는 90% 이상의 정확도로 세 자리 하우스 넘버 이미지를 맞추는 것입니다. 

SVHN 프로젝트를 위한 사전 연습으로 two_digits_with_blank_classification에서 사이킷런에서 기본적으로 제공하는 load_digits 데이터셋을 가공하여 새 데이터 셋을 만들고, CNN 모델에 학습시켜 예측해보겠습니다.

<img src="http://ufldl.stanford.edu/housenumbers/examples_new.png">

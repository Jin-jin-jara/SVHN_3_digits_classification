# Small-Project : SVHN 3 digits classification

이번 프로젝트에서는 간편하게 사용하던 keras의 Sequential 모델이 아닌 아닌 tensorflow를 이용한 전문가용 모델을 직접 구축해 데이터를 학습시키고 예측해보려고 합니다. 또 정제된 기본 데이터가 아닌 노이즈가 많은 실제 데이터를 사용해 예측을 진행하겠습니다.

구글 <a href="http://ufldl.stanford.edu/housenumbers/">Street View House Number</a>이미지를 다운받아 이미지 속의 숫자를 기계가 학습하고 예측하도록 합니다. 다만 SVHN 전체 데이터셋(Full Numbers)은 너무 용량이 커 사용하기 어렵기 때문에 각 숫자 이미지를 잘라놓은 Cropped Digits 데이터 셋(그 중에서도 test데이터셋만을)을 사용하겠습니다.


SVHN 프로젝트를 위한 사전 연습으로 two_digits_with_blank_classification에서 사이킷런에서 기본적으로 제공하는 load_digits 데이터셋을 가공하여 새 데이터 셋을 만들고, CNN 모델에 학습시켜 예측해보겠습니다.


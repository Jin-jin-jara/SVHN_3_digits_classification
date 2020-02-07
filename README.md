# Small-Project : The Street View House Number 3 digits classification<br>
## recognizing digits and numbers in natural scene images

### Goal
이 프로젝트의 목표는 직접 구축한 CNN 모델로 실제 이미지 데이터를 훈련시켰을 때 이미지 안의 숫자를 잘 분류해내는 모델을 만드는 것입니다. 이번 프로젝트에서는 간편하게 사용하던 keras의 Sequential 모델이 아닌 아닌  <a href="https://www.tensorflow.org/tutorials/quickstart/advanced?hl=ko">tensorflow 전문가용 CNN모델</a>을 직접 구축해 데이터를 학습시키고 예측해보려고 합니다. 구축한 모델로 90% 이상의 정확도로 세 자리 하우스 넘버를 예측하는것을 목표로 하겠습니다.<br>

### Dataset
이번 프로젝트에서 사용할 데이터셋은 <a href="http://ufldl.stanford.edu/housenumbers/">Google Street View House Number</a>입니다. 구글이 촬영한 street view에서 집 번호만 추출한 데이터입니다. 이 데이터셋은 사이킷런에서 기본으로 제공하는 MNIST손글씨 데이터처럼 32x32 픽셀의 데이터입니다. 다만 잘 가공된 연습용 데이터가 아닌 노이즈가 많은 실제 세상의 데이터입니다.<br>

SVHN 전체 데이터셋(Full Numbers)은 너무 용량이 커 사용하기 어렵기 때문에 각 숫자 이미지를 잘라놓은 Cropped Digits 데이터 셋(그 중에서도 test데이터셋만을)을 사용하겠습니다. Cropped Digits 데이터셋은 하우스 넘버 이미지를 한 자리 수로 잘라놓은 데이터셋입니다. 한 자리수 이미지들을 붙여 세 자리로 만든 후 기계를 학습시키고 예측하도록 하겠습니다.<br>

<img src="http://ufldl.stanford.edu/housenumbers/32x32eg.png" style="margin-left: auto; margin-right: auto; display: block;"/><br>

### Before start
SVHN 프로젝트를 위한 사전 연습으로 <a href="https://github.com/Jin-jin-jara/Small-Project1--SVHN_3_digits_classification/blob/master/small_project1_two_digits_with_blank.ipynb">two_digits_with_blank_classification</a>에서 사이킷런에서 기본적으로 제공하는 load_digits 데이터셋을 가공하여 새 데이터 셋을 만들고, CNN 모델에 학습시켜 예측해보겠습니다.<br>

### Conclusion
<a href="https://github.com/Jin-jin-jara/Small-Project1--SVHN_3_digits_classification/blob/master/small_project_SVHN_3_digits_classification.ipynb">결과</a>가 잘 나왔습니다!
<img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fk.kakaocdn.net%2Fdn%2F23hWM%2FbtqBO8BnK0I%2Fg7pyzF0UqOJM5mkroc9jvK%2Fimg.png"><br>




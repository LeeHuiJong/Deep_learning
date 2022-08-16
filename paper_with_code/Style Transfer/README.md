# Style Transfer
## 1. Introduction
우선 예시를 보자.
<p align="left">
    <img src="images/example.png">
</p>
왼쪽이 원래 이미지(input), 오른쪽의 작은 이미지가 스타일을 추출할 이미지, 그리고 오른쪽 큰 이미지가 변환된 인풋 이미지다.
<br> Style Transfer 는 말그대로 이미지의 스타일을 변환시키는 것이다. 이에 base가 되는 모델은 VGG를 사용했다.

## 2. Content representation
<p align="left">
    <img src="images/example.png">
</p>

# Style Transfer
## 1. Introduction
우선 예시를 보자.
<p align="left">
    <img src="images/example.png">
</p>
왼쪽이 원래 이미지(input), 오른쪽의 작은 이미지가 스타일을 추출할 이미지, 그리고 오른쪽 큰 이미지가 변환된 인풋 이미지다.
<br> Style Transfer 는 말그대로 이미지의 스타일을 변환시키는 것이다. 이에 base가 되는 모델은 VGG를 사용했다.

## 2. Content representation
이미지에서 우선 디테일한 픽셀의 정보는 지우고 high level content 만 보존하는 식으로 가는데 이는 아래의 그림처럼 진행된다.

<p align="left">
    <img src="images/content r pic.png">
</p>

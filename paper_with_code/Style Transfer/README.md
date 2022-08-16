# Style Transfer
## 1. Introduction
우선 예시를 보자.
<p align="left">
    <img src="images/example.png">
</p>
왼쪽이 원래 이미지(input), 오른쪽의 작은 이미지가 스타일을 추출할 이미지, 그리고 오른쪽 큰 이미지가 
<br>변환된 인풋 이미지다. Style Transfer 는 말그대로 이미지의 스타일을 변환시키는 것이다. 이에 base가 
<br>되는 모델은 VGG를 사용했다.

## 2. Content representation
이미지에서 우선 디테일한 픽셀의 정보는 지우고 high level content 만 보존하는 식으로 가는데 이는 
<br>아래의 그림처럼 진행된다.
<br>
<p align="left">
    <img src="images/content r pic.png">
</p>
뒤로 갈수록 사진은 뭔가 일그러진것 처럼 보이지만 이미지에 있는 핵심 feature 들은 보존하고 있는 상태다. 
<br>세세한 부분은 모두 생략해버린 것이다. 즉 content image에 대해 전체적인 느낌을 살린 것이다.

## 3. style representation

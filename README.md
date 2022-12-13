<h3>주제</h3>
태양의 움직임에 따른 태양 전지 패널 제어
<h3>내용<h3> 
태양 전지 패널의 효율을 극대화하기 위하여 시간에 따른 태양의 움직임을 추적하는 태양전지 패널을 제작해보자.<br/>
<h3>사용언어<h3>  
  
<img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/matlab/matlab.png" width="32" height="32" class="d-block rounded-1 mr-3 flex-shrink-0" alt="matlab logo">

<h3>패널과 모터의 Equation</h3> 

![스크린샷_20221213_084037](https://user-images.githubusercontent.com/87568714/207310432-024e000a-359c-4d4b-90dd-0f019f04ebb4.png)
다음은 패널과 모터의 방정식이다. 위 식을 토대로 SIMULINK를 활용하여 제어 모델을 제작해보자.

<h3>패널 모델 제작</h3>

![스크린샷_20221213_085917](https://user-images.githubusercontent.com/87568714/207312289-ddacc9de-3934-4db6-b0e5-ad3fe0381a1a.png)
여기서 J = 8.6 , Kd = 5로 설정하였다.

<h3>모터 모델 제작</h3>
  
![스크린샷_20221213_090208](https://user-images.githubusercontent.com/87568714/207312753-b569ef07-fd68-4d43-a938-dbd5cec05e3b.png)
여기서 R = 10 , Kg = 2000, Kt = Kf = 0.07 로 설정하였다.

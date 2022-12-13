<h3>주제</h3>
태양의 움직임에 따른 태양 전지 패널 제어
<h3>내용<h3> 
태양 전지 패널의 효율을 극대화하기 위하여 시간에 따른 태양의 움직임을 추적하는 태양전지 패널을 제작해보자.<br/>
<h3>사용언어<h3>  
MATLAB & SIMULINK

<h3>패널과 모터의 Equation</h3> 

![image](https://user-images.githubusercontent.com/87568714/207320023-1e93d58d-3eaf-4475-ac94-7a9debfbc7ea.png)<br/>
다음은 패널과 모터의 방정식이다. 위 식을 토대로 SIMULINK를 활용하여 Physical System을 제작해보자.

<h3>패널 모델 제작</h3>

![스크린샷_20221213_085917](https://user-images.githubusercontent.com/87568714/207312289-ddacc9de-3934-4db6-b0e5-ad3fe0381a1a.png)<br/>
여기서 J = 8.6 , Kd = 5로 설정하였다.

<h3>모터 모델 제작</h3>
  
![스크린샷_20221213_090208](https://user-images.githubusercontent.com/87568714/207312753-b569ef07-fd68-4d43-a938-dbd5cec05e3b.png)<br/>
여기서 R = 10 , Kg = 2000, Kt = Kf = 0.07 로 설정하였다.
  
<h3>제어기 모델 제작</h3>  
  
![image](https://user-images.githubusercontent.com/87568714/207319287-c1724d23-4649-40d7-8ac1-21566616374d.png)<br/>
대표적인 제어 모델중 하나인 PID 제어기를 사용하여 제작해보았다.
이때, 태양의 위치는 미리 설정해두었던 Data를 불러와 설정하였고 15시간에 대한 시뮬레이션을 진행하였다.
태양의 위치에 따른 패널의 위치에 대한 그래프는 아래와 같았다.

![image](https://user-images.githubusercontent.com/87568714/207319167-4cb1d82d-0536-46ba-8f87-86f2c3c8b3e1.png)<br/>
노란색 선이 태양의 위치 그리고 파란색 점선이 패널의 위치이다. 태양의 위치가 변함에 따라 패널의 위치 또한 이를 추적하여 변하는것을 확인할 수 있었다.


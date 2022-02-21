## STM32 System 설정하는법.
---

- STM32CubeIDE로 H/W 또는 F/W의 코드를 작성하기 위해서는 CubeMX를 사용해서 MCU의 System setUP을 지정해줘야 한다 쉽게 말하면 pin 하나, 하나 무슨 기능을 할지 미리 설정해두는 단계를 의미한다
- 설정이 완료 되면 우측 상단의 GENERATE CODE를 눌러 STM32CubeIDE에 코드를 작성 할 수 있게 적용을 시켜줘야 한다, 적용이 완료 되면 자동으로 뼈대가 되는 코드가 생성되고 그 안에 USER CODE를 작성하면 된다

---
### CubeMX의 설정 화면
---
![system](https://user-images.githubusercontent.com/84003327/154901283-9cbc9d6b-b967-4ac1-a505-38ac4f930dbc.PNG)

위 사진의 내용처럼 기본적으로 주어지는 default Setting과 사용자가 추가로 지정한 녹색의 USER Setting을 볼 수 있다, 또한 좌측의 System Core, Analog, Computing, Timeres와 같은 별도의 메뉴들로 
추가적인 시스템 설정 을 할 수 있다

또한 상단의 메뉴인 Clock Configuration, Project Manager 와 같은 세부 셋팅 또한 가능하다.

---
### Clock Configuration
---

![캡처](https://user-images.githubusercontent.com/84003327/154913637-bc54c34c-ce99-4f5c-9e85-3c2da551e2c9.PNG)

clock signal 이란?

- 클럭 신호(영어: clock signal)는 논리상태 H(high,논리 1)와 L(low,논리 0)이 주기적으로 나타나는 방형파(square wave) 신호를 말한다.

클럭 신호의 요소는
- 신호의 크기
- 주기를 결정하는 주파수
- 한 주기 동안 상태 high와 low의 시간비인 듀티(duty)비율 or PWM (Pulse Width Modulation) <펄스 폭 변조>












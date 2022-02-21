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













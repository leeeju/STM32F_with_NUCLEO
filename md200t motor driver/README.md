## MD200T motor driver
---

모터 및 모터드라이브는 모바일봇(이동로곳)을 만드는데 있어 핵심이 되는 H/W이다 모터 및 모터드라이브는 쉽게 말하면 사람의 다리 역할을 하는 것 모터와 그 모터를 제어 하는 모터 드라이브로
나뉜다 

이와 같은 H/W를 다울때는 Datasheet의 존재가 반드시 필요하다, 판매사 또는 제조사의 홈페이지를 가면 해당 제품의 데이터시트를 쉽게 구할 수 있다, 또는 https://www.alldatasheet.co.kr/ 에 접속하여 
대부분의 반도체 및 MCU 부품들의 세부 정보를 알 수 있다.

또한 대부분의 드라이버들은 제조사가 제공하는 테스트 플렛폼이 존제한다, 다음 사진은 MD200T motor TEST를 위한 프로그램 UI 이다

![화면 캡처 2022-02-28 142658](https://user-images.githubusercontent.com/84003327/155929001-d268f6ce-712a-4913-9286-a8298164f697.png)

해당 프로그램을 사용하여 받아온 모터의 성능 및 작동 테스트를 진행 할 수 있다, 초반에 간과한 일은 가장 기본적인 실수를 해서 머슥했던 일이 있다.
제품의 데이터 시트를 보지 않고 눈대중으로 연결해서 왜 안되지 하는 사건이 있었다, TX와 RX를 잘 보고 연결했어야 했는데 눈대중으로 맞겠지 하고 왜 통신이 안되지 하는 일이 있었고...
중도에 해결하긴 했지만 오전시간을 가장 간단한 문제로 해결하지 못했던 기억이 남는다

### RS485통신이란?
---
모터 드라이브는 RS485를 사용한 통신 방식을 사용한다. 시리얼 통신의 일종으로 직렬(1:1)로 데이터를 송.수신 하는것을 이야기 한다 
시리얼 통신의 종류는 RS232 / RS423 / RS485 등이 있으며 그중 에서 가장 많이 사용하는 방식은 RS232와 RS485가 있다 

### pinmap
---
![PINMAP](https://user-images.githubusercontent.com/84003327/155947002-d35dc3f8-2db6-493f-9688-f21de48c4fb2.PNG)

해당 드라이버가 시리얼 통신을 하기 위해서는 RS485를 사용한 통신을 해야만 한다, 때문에 위 사진의 pinmap의 보이는 14번 15번 선을 통신케이블 USB to RS485를 사용해서 데이터를 송,수신 할 수 있다
또한 자세한 드라이버의 성능 및 정보를 위해서 데이터 시트 열람을 추천한다 
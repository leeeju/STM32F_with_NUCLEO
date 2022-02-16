## STM32CubeIDE를 사용한 F/W 연습


## NUCLEO란?
MCU 의 최소 기능만으로 구성된 개발 보드로 ST사(STMicroelectronics)에서 제작한 개발 보드이다. 연결되지 않은 나머지 핀들을 사용자가 자유롭게 사용할수 있도록 확장핀 커낵터로 연결되어 있다.
높은 성능, 실시간 기능, 디지털 신호 처리 및 저전력, 저전압등의 장점이 있다 

공식 홈페이지 자료실 --> https://www.st.com/ko/stm32/stm32/reflibrary.html

개인 링크 --> https://www.youtube.com/watch?v=lG1DBbBNUas

필자가 사용할 NUCLEO-F429ZI 보드를 소개한다

![image](https://user-images.githubusercontent.com/84003327/153141052-f172cc14-cede-418c-9bf3-5b237f2a1096.png)

|구분|내용|
|:---:|---|
|코어|ARM 32비트 Cortex_M4 프로세서|
|최대 동작 주파수|180MHz|
|동작속도|1.25 DMIPS/MHz |
|메모리 | 512 ~ 2048KB |
|플레시 메모리 | 256KB|
|동작전압| 1.8 ~ 3.6V|
|입출력핀|82 ~ 168 pin|
|타이머| 범용 10개, 고성능 2개, 기본2개|
|주변장치| USBOTG FS 1개, USBOTG HS 1개, CAN, SPI, I2C, 이더넷, 카메라, TFTLCD 디스플레이|
|AD 변환기 | 12bit ADC 3개 (16 OR 24C)|
|DA 변환기 | 12bit ADC 1개 (2C)|
|패키지 PIN| 100 ~ 216pin|

## STM32 F/W의 전체 구조

![qwd](https://user-images.githubusercontent.com/84003327/153317245-63ed5212-c846-4b82-8ca1-eb97dd3f846c.PNG)


## STM32 F/W의 세부 구조

![캡처](https://user-images.githubusercontent.com/84003327/153317329-cba6b4d6-4af3-4d64-afc1-0d45b3c291e7.PNG)

## STM32 코드 작성툴 3가지 

STM32의 코드 작성 및 디버그를 하기 위한 툴은 다양하게 있지만 크게 3가지로 나뉜다.

### STM32CubeMX

먼저 STM32CubeMX는 STM32 마이크로컨트롤러 및 마이크로프로세서를 매우 쉽게 구성할 수 있는 그래픽 도구이며 기코 코드를 만들기전의 mcu의 설정을 편하게 할 수 있는 장점이 있다

![mx](https://user-images.githubusercontent.com/84003327/154198786-a6f706a9-3f90-41e5-aa2b-2c70ab8ebde7.PNG)

### STM32CubeIDE

다음으로는 가장 많이 사용되는 STM32CubeIDE는 STM32Cube 소프트웨어 에코시스템의 일부인 올인원 다중 OS 개발 도구입니다,  STM32 마이크로컨트롤러 및 마이크로프로세서를 위한 주변 장치 구성, 코드 생성, 코드 컴파일 및 디버그 기능을 갖춘 고급 C/C++ 개발 플랫폼입니다

![ide](https://user-images.githubusercontent.com/84003327/154198976-e6baa3fa-dfc3-4e68-ae8e-a4579f0f3025.PNG)

### Atollic TrueSTUDIO

Atollic TrueSTUDIO는 Eclipse, CDT 에 구축된 상업적으로 향상된 C/C++ IDE입니다., GCC 및 GDB 컴파일러를제공하여 개발자에게 쉽고 효율적인 개발 도구 이다,
가장 큰 장점으로는 무려 한글지원이 가능하다는 장점이 있다

![스튜디오](https://user-images.githubusercontent.com/84003327/154199205-1d5c6579-663b-4ab1-b17f-b04793a088e0.PNG)

전부 사용해본 결과 STM32CubeMX와 STM32CubeIDE를 함깨 사용하는것이 가장 효율적이지만 전부 영문이라는 단점이 있다..



### 꿀tip
[내pc] --> [사용자] --> [STM32Cube] --> [STM32Cube_FW_F4_V1.26.2] --> [Projects] 에 들어가 보면다 다양한 뉴클레오 보드들의 이름이 나올것이다, 그중에 자신이 사용하고 
있는 보드를 선택해 열어보면 [Examples] 폴더 안에 다양한 예제들이 들어있는 것을 확인 할 수 있다




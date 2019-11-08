# Arduino IDE

 아두이노 IDE는 아두이노의 통합개발 도구로서, 스캐치(프로그래밍), 컴파일, 업로드 등의 과정을 하나의 화면에서 작업할 수 있도록 합니다.

## 개발 환경 만들기

 1. 아두이노 IDE 다운 받기

    홈페이지 : [https://www.arduino.cc/](https://www.arduino.cc/)

    IDE 다운로드 : [https://www.arduino.cc/en/Main/Software](https://www.arduino.cc/en/Main/Software)

    다운로드 링크에서 자신의 PC OS와 맞게 설치 파일을 다운로드 합니다. 설치파일을 누르게 되면 Donate 화면이 나오는데, 다운로드만 받고 싶으시면 JUST DOWNLOAD를 눌러 줍니다.

 2. 아두이노 IDE 설치하기
    
    다운 받은 설치 파일을 실행시킵니다. 그 후 설치가 진행되는데 저는 기본 설정에서 건드리지 않았습니다. 저장 경로 정도는 본인의 상황에 맞게 바꿔 주시면 될 것 같습니다.

 3. 아두이노 보드와 PC 연결하기

    IDE의 설치가 완료되셨다면, 프로그램을 실행 시킵니다. 그리곤 준비한 아두이노 보드를 PC에 연결 시켜줍니다.

 4. 보드 종류와 포트를 설정합니다.

    아두이노 IDE를 켜고, 툴 탭에 보시면 보드와 포트 설정이 각각 있습니다. 보드의 경우 자신의 PC에 연결한 보드를 선택하시면 되고, 포트의 경우 현재 연결한 보드가 있어서 자동적으로 뜨는 것을 선택해 주시면 되겠습니다.


## 예제 실행하기

 1. LED 깜박이기

 아두이노 IDE의 탭에서 파일 - 예제 - 01.Basics - Blink 순으로 클릭을 해주시면 아두이노 보드의 LED를 깜박이게 하는 기본예제가 나옵니다. 이를 보드에 업로드 해주시면 보드의 LED가 깜빡이는 것을 확인할 수 있습니다.

 2. 업로드 상태 초기화 시키기

 예제들을 실행 해보다 보면 보드에 업로드된 것들을 초기화 하고 싶을 때가 있습니다. 이때는 파일 - 예제 -  EEPROM - eeprom_clear 파일을 열고 이를 업로드 해주시면 됩니다.

## Arduino Online IDE

 아두이노에서는 Online IDE를 제공하고 있습니다. 이를 이용하면 최신상태의 IDE를 사용하고 작성한 스케치를 cloud에 저장해서 언제든 쓸 수 있다는 장점이 있습니다. 항상 인터넷 연결이 보장된 곳에서 개발을 하신다면 이를 이용하는 것도 좋은 방법입니다.
 

## VScode에서의 사용

 아두이노 개발을 VScode로도 하실 수 있습니다. 하지만 기본적으로 Arduino IDE는 설치가 되어 있어야 합니다.

 VScode로 아두이노를 개발 하시려면, VScode Marketplace에서 Arduino를 검색하고 Microsoft에서 제공하는 Arduino for Visual Studio Code를 설치해줍니다.
 이것이 제공하는 기능은 아래와 같습니다.

 1) IntelliSense and syntax highlighting for Arduino sketches
 2) Verify and upload your sketches in Visual Studio Code
 3) Built-in board and library manager
 4) Built-in example list
 5) Built-in serial monitor
 6) Snippets for sketches
 7) Automatic Arduino project scaffolding
 8) Command Palette (F1) integration of frequently used commands (e.g. Verify, Upload...)
 9) Integrated Arduino Debugging 
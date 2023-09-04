# Java Download
여기서 설명하는 것은 Java SE 20, 윈도우 운영체제를 기반으로 한다. 자바를 사용하기 위해서는 우선 코드 작성과 컴파일 및 디버깅, JVM을 포함해야하기 때문에 JDK(Java Development Kit)를 다운로드해야 한다. JDK 다운로드는 https://www.oracle.com/kr/java/technologies/downloads/#jdk20-windows 에서 받을 수 있다.
# 환경 변수 설정
JDK를 다운받았다면 환경변수를 설정해야 하는데 `윈도우 검색 -> 시스템 환경 변수 편집 -> 시스템 변수`에 변수 이름은 `JAVA_HOME`, 변수 값은 자바가 설치된 위치를 작성하고 새로 만들기를 한다. 변수 값 예시는 다음과 같다. `C:\Program Files\Java\jdk-20`

다음은 `CLASSPATH` 환경 변수를 설정해야 한다. 시스템 변수에 변수 이름은 `CLASSPATH`, 변수 값은 `%JAVA_HOME%\lib`를 작성한다.
2개 모두 작성했다면 마지막으로 시스템 변수에서 Path 변수에 편집(또는 더블 클릭)을 누르고 `새로 만들기 -> %JAVA_HOME%\bin 작성 -> 확인`을 한다.
# IDE 다운로드
IDE(Integrated Development Environment, 통합 개발 환경)는 이클립스 또는 IntelliJ IDEA를 사용할 것이다.

- 이클립스: https://www.eclipse.org/downloads/
- Intelij IDEA: https://www.jetbrains.com/ko-kr/idea/
# Java SE, Java EE, Java ME
Java SE는 자바 표준 플랫폼으로 일반적인 환경에서 쓰이는 JVM과 API를 정의한다. Java SE는 다른 플랫폼의 기반이 되며 가상 머신, 개발 도구, 배포 기술, 다양한 API 및 툴킷 등을 제공한다.

Java EE(Enterprise Edition)는 Java SE 위에 탑재되며 다양한 웹 프로그래밍 기능을 포함한다. 주로 서버측 개발에 이용되며 대규모, 다계층, 확장성, 신뢰성, 보안 네트워킹 API 등을 제공한다.

Java ME(Micro Edition)는 모바일 환경과 같은 작은 규모의 가상 머신으로 동작시킬 수 있는 API를 제공한다. Java ME 또한 Java SE를 기반으로 하며 전용 API를 제공한다. Java EE의 클라이언트측 개발에 이용되기도 한다.
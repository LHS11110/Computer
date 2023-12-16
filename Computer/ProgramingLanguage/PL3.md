# 코딩 컨벤션(Coding Conventions)
코딩 컨벤션은 개발자가 코드의 가독성과 유지보수를 위해 지켜야 할 일종의 코딩 스타일 규약을 말한다.<br/>
대규모 프로젝트와 같은 협업이 필요한 환경에서는 자신의 코드가 남들에게 어떻게 동작하는지 효과적으로 전달해야 하며<br/>
메소드와 클래스, 변수의 이름 또한 그 의미가 확실해야 한다.<br/>
<br/>
대부분의 유지보수는 해당 코드를 작성한 개발자가 해결하는 것이 아니라 다른 개발자가 맡아서 해결한다.<br/>
만약 여러 개발자가 자신만이 이해할 수 있는 스타일로 코드를 작성한다면<br/>
다른 개발자가 유지보수를 위해 코드를 이해하는데 생각보다 큰 비용과 시간이 소모되며 기능을 오해하는 경우까지도 갈 수 있다.<br/>
이러한 문제점을 해결하기 위해 사전에 코딩 스타일을 통일함으로써 소모되는 시간과 비용을 절감시킬 수 있다.<br/>
<br/>
자바 코딩 컨벤션에는 다양한 형태가 있으며 다음 3가지가 가장 많이 쓰인다.

- NAVER : 캠퍼스 핵데이 Java 코딩 컨벤션(https://naver.github.io/hackday-conventions-java/)
- Google : Google Java Style Guide(https://google.github.io/styleguide/javaguide.html)
- Oracle : Code Conventions for the Java(https://www.oracle.com/java/technologies/javase/codeconventions-contents.html)

## 코딩 컨벤션의 장점
1. 통일된 코딩 스타일은 기능과 구조를 명확하게 한다.
2. 기능과 구조를 명확히 할 수 있는 코딩 스타일은 코드를 이해하는데 드는 시간과 비용을 줄일 수 있다.
3. 유지보수에 대한 비용이 절감된다. 다시 말해 가독성이 좋아진다.
### 명명 규칙(Naming Rule)
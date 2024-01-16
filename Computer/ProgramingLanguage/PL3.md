# 코딩 컨벤션(Coding Conventions)
코딩 컨벤션은 개발자가 코드의 가독성과 유지보수를 위해<br/>
지켜야 할 일종의 코딩 스타일 규약을 말한다.<br/>
<br/>
자바 코딩 컨벤션에는 다양한 형태가 있으며 다음 3가지가 가장 많이 쓰인다.

- NAVER : 캠퍼스 핵데이 Java 코딩 컨벤션(https://naver.github.io/hackday-conventions-java/)
- Google : Google Java Style Guide(https://google.github.io/styleguide/javaguide.html)
- Oracle : Code Conventions for the Java(https://www.oracle.com/java/technologies/javase/codeconventions-contents.html)

## 네이밍 컨벤션(Naming Conventions)
네이밍 컨벤션은 코딩 컨벤션 중 하나로 변수명, 함수명, 클래스명 등<br/>
식별자를 명명할 때 사용하는 규칙이다.<br/>

### 스네이크 표기법(Snake Case)
영문자를 모두 소문자로 표기하며 단어 사이를 언더바(_)로 구분<br/>
`ex) snake_case`
### 카멜 표기법(Camel Case)
첫 번째 단어를 제외하고 모든 단어마다 첫 글자를 대문자로 표기<br/>
`ex) camelCase`
### 파스칼 표기법(Pascal Case)
모든 단어마다 첫 글자를 대문자로 표기<br/>
`ex) PascalCase`
### 케밥 표기법(Kebob Case)
영문자를 모두 소문자로 표기하며 단어 사이를 하이픈(-)으로 구분<br/>
`ex) kebob-case`
### 스크림 스네이크 표기법(Scream Snake Case)
주로 상수를 표현할 때 사용한다.<br/>
영문자를 모두 대문자로 표기하며 단어 사이를 언더바(_)로 구분<br/>
`ex) SCREAM_SNAKE_CASE`

## 코딩 컨벤션의 장점
코딩 컨벤션을 준수하면 일관성있는 코드를 작성할 수 있어<br/>
기능과 의미를 보다 빠르게 이해할 수 있다.<br/>
즉, 코드의 가독성과 유지보수성을 향상시킬 수 있다.
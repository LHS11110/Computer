# 객체(Object)
# 클래스(Class)
### 필드(Field)
멤버 변수(Member Variable), 속성(Attribute)이라고도 한다.<br/>
필드는 클래스 내에 정의된 변수로 객체를 통해서 접근할 수 있으며 서로 독립적인 공간을 사용하고 객체가 소멸되면 필드도 함께 소멸된다.

```java
class Exemple
{
	// 필드
	int member1;
	float member2;
    ...
}
```
### 메서드(Method)
멤버 함수(Member Function)라고도 하며 어떤 기능을 수행하기 위한 코드 집합이다.<br/>
Java에서는 함수와 메서드를 구분하지 않지만 Python에서는 함수와 메서드를 구분한다.<br/>
메서드는 클래스 내에 정의된 함수로 객체를 통해서 호출할 수 있다.

```java
class Exemple
{
	// 메서드
    void method1()
    {
        ...
    }

    int method2()
    {
        ...
    }

    ...
}
```
# 인스턴스(Instance)
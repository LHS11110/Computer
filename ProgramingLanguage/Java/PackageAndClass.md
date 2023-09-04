# 패키지
모든 프로그램들이나 파일들은 식별자를 통해서 구분한다. 이는 매우 당연한 얘기이며 파일의 이름이 중복되어선 안된다는 것을 의미하기도 한다. 컴퓨터를 다루다 보면 같은 이름을 사용하는 파일이 생길 수 있는데 이러한 문제를 디렉토리를 통해서 해결한다. 자바 또한 클래스의 이름이 중복되지 않게 하기 위한 패키지라는 것이 있으며 디렉토리와 동일한 개념이다. 때문에 패키지는 단순히 클래스들과 또 다른 패키지를 포함하는 하나의 카테고리 역할을 한다. 패키지는 또 다른 패키지를 포함할 수 있다고 말했는데 여기서 패키지를 포함하는 패키지를 상위 패키지, 패키지에 포함된 내부 패키지를 하위 패키지라고 부른다. 패키지를 통해 비슷한 범주의 작업을 처리하는 클래스들은 모두 하나의 패키지에 담을 수 있으며 외부에서 해당 클래스에 대한 접근 방법은 다음과 같은 것들이 있다.

1. import : import 키워드를 사용하면 해당 클래스에는 또 다른 클래스가 포함된다.
2. FQCN(Fully Qualified Class Name) : 패키지를 포함하여 클래스명까지 모두 기술하는 것을 말한다.

위 방법들을 사용할 때는 `상위 패키지.하위 패키지.클래스`와 같이 점을 통해서 상위 패키지와 하위 패키지, 클래스 이름을 구분하고 `package` 키워드와 이름을 기술하여 현재 소스 파일이 어느 패키지에 포함되었다는 것을 알려준다.

```java
package 자바;       // 현재 소스 파일은 자바라는 패키지에 포함되어 있다는 것을 의미하는 코드
import Test.Object; // Test는 패키지 이름, Object는 클래스 이름이다.

public class HelloWorld {
	public static void main(String[] args) {
		Object t = new Object();
		t.obj_print();
	}
}
```

```java
package 자바;

public class HelloWorld {
	public static void main(String[] args) {
		Test.Object t = new Test.Object(); // FQCN, 패키지와 클래스 이름을 모두 기술
		t.obj_print();
	}
}
```
# 클래스
클래스는 객체 지향에서 사용되는 개념이며 자바는 기본적으로 객체 지향 프로그래밍 언어이다. .java 확장자를 사용하는 소스 파일들은 모두 하나의 클래스를 의미하며 소스 파일들에는 파일과 같은 이름을 사용하는 public 클래스가 하나 존재해야 한다. (가독성과 유지 보수를 위함이며 이것이 꼭 지켜지지 않아도 됨)

```java
// 파일 이름: test.java
package test;

public class test /* 파일과 같은 이름을 사용하는 클래스가 하나 존재해야 한다. */{
	public static void main(String[] args) {
		Test.Object t = new Test.Object(); // FQCN, 패키지와 클래스 이름을 모두 기술
		t.obj_print();
	}
}
```

클래스는 사실 소스 파일의 이름과 상관없이 접근될 수 있고 선언할 수 있다. 소스 파일이 항상 하나의 클래스를 가르키는 것은 아니며 이처럼 오해하는 것은 public class가 조금 특별한 문법을 가지기 때문이다. 다른 접근 제어자를 가진 클래스는 여러개가 선언될 수 있으며 허용하는 범위만큼 접근이 가능하다. public class는 모든 외부에서 접근이 가능하며 해당 클래스의 이름은 항상 소스 파일의 이름과 같아야 한다. (단, 중첩 클래스는 예외)

```java
// object.java
package Test;

class object1 {
	public void print(String msg)
	{
		System.out.println(msg);
	}
}

class object2 {
	public void print(String msg)
	{
		System.out.println(msg);
	}
}
```

```java
package Test;

public class testObject {
	public void method(String msg)
	{
		System.out.println(msg);
        
		object2 obj2 = new object2(); // 이처럼 파일의 이름과는 상관없이 선언된 클래스에 접근할 수 있다.
		obj2.print("abcdefg\n");

		object1 obj1 = new object1();
		obj1.print("abcdefg2\n");
	}
}

```

```java
package Main;

public class HelloWorld {
	public static void main(String[] args) {
		Test.testObject tobj = new Test.testObject();
		tobj.method("Hello World!\n");;
	}
}

/* output
Hello World!

abcdefg

abcdefg2
*/
```
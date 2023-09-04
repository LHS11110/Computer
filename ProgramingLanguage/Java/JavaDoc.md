# 주석(Comment)
주석은 프로그래밍 언어에서 컴파일되지 않는 문자열로 문법에서 무시된다. 주로 의견이나 설명을 위한 용도로 변수나 함수, 클래스의 이름으로도 충분히 의미를 전달할 수 있지만 그러지 못한 경우 주석을 사용하여 더 쉽게 이해할 수 있도록 돕는다. 개인 개발이나 간단한 구현이 아닌 경우 의미 전달이 쉽도록 협업이나 복잡한 코드에서 많이 보인다. 자바에서 사용되는 주석은 아래와 같다.

```java
package Test;

public class Main {
	// 라인 주석, 한 줄만으로도 충분한 경우 라인 주석을 쓴다.
    /* 블록 주석, 여러 줄의 설명이 필요할 때 쓰인다. */
	public static void main(String[] args) {
		
	}

}

```
# JavaDoc
자바 Doc은 클래스, 함수, 변수 등 소스 파일에 대한 문서를 작성할 때 쓰인다. 작성할 때는 `/** */`와 같이 시작은 슬래시 1개와 별표 2개, 끝은 별표 1개와 슬래시 1개이다. 이클립스에서 html 문서를 생성할 때는 다음 절차를 따른다. `class 또는 package 우클릭 -> Export -> Java/Javadoc 선택 -> 설정 -> Finish`

자바 Doc을 작성할 때 별표 이전의 공백이나 탭 문자는 무시되므로 아래와 같이 작성된다.

```java
package Test2;

public class Main {
	/**
	 * main 함수입니다.
	 * ...
	*/
	public static void main(String[] args) {
		
	}

}

```

모든 주석은 전처리 과정에서 제거되므로 코드에 영향을 주지 않는다.
자바 Doc의 구성은 크게 설명문과 태그 섹션으로 나뉘며 html 태그가 유효하다. 설명문 다음으로 태그 섹션이 나오며 태그 섹션 이후로는 설명문을 작성할 수 없다.
아래는 자바 Doc의 태그들이다.

```
annotation                          description
@version x.x                        버전

@author name                        작성자

@deprecated deprecated-text         해당 클래스나 메소드 등을 더 이상 사용하지 않을 것을 권장하는 경우에 사용

@see reference                      다른 클래스나 메소드 또는 외부 링크나 텍스트를 표시하는 경우에 사용, 외부 사이트의 링크를 사용하는 경우 html의 a 태그 사용
                                    내부 참조의 경우 패지키명#필드/생성자/메소드, 현재 클래스의 멤버일 경우 #필드/생성자/메소드

@since x.x                          도입된 버전을 명시할 때 사용, @version은 현재 버전을 명시하는 반면, @since는 어떤 버전에서 도입 되었는지를 명시

@param param-name description       해당 매개 변수에 대한 설명

@return description                 반환 값에 대한 설명

@throws class-name description      던져질 수 있는 예외에 대한 설명, @exception 태그는 @throws와 동일하다.

{@link package.class#member label}  @see와 같은 역할을 하며 설명문이나 다른 태그들의 description/deprecated-text에 포함될 수 있다.
                                    label은 생략할 수 있으며 명시된 경우 label로 표시, {@linkplain} 태그는 해당 참조를 일반 텍스트로 표시한다.

{@code source-code}                 예제 코드
```

아래는 자바 Doc의 예시이다.

```java
/**
 * ...
 */
class List {
	/**
	 * 리스트의 마지막에 정수값 n을 추가합니다.
	 * 처음에 추가하고 싶은 경우, {@link #push_front(long)}를 사용하세요.
	 * @param n 정수값
	 */
	public void push_back(int n)
	{
		...
	}
	
	/**
	 * ...
	 */
	public void push_front(int n)
	{
		...
	}
}

```
# 배열
배열은 동일한 데이터 타입이 연속적으로 나열된 자료구조를 말한다. 이러한 배열은 반드시 유한해야 하며 인덱스와 데이터가 하나씩 대응되는 형태를 가진다.
프로그래밍에서는 배열의 인덱스가 0부터 시작하며 중괄호를 통해 배열을 작성한다. 아래는 배열을 작성하는 것과 인덱스에 대한 예시이다.
- `int`형 배열 : {13, 6, 20, 100, 32, 49, 62}
- `float`형 배열 : {3.14, 0.32, 1.0, 6.7, 32.23, 4.13, 54.23}
- `int`형 배열의 배열 또는 `int`형 2차원 배열 : {{3, 2, 5}, {7, 23, 87}, {34, 654, 123}}
배열에 대한 특징으로는 아래와 같은 것들이 있다.
- `0`차원 배열은 `Data`를 의미한다.
- `n`차원 배열이란 `n - 1`차원 배열들의 연속적인 나열을 의미한다.
- `n`차원 배열에서 `m`차원 배열들의 길이가 모두 같을 필요는 없다. `(n > m)`
- `n`차원 배열에서 `Indexing`은 `n - 1`차원 배열으로의 접근을 의미한다.
- `Indexing`의 시간 복잡도는 `O(1)`이다.
- 배열의 크기는 고정이다.
- 잘못된 `Indexing`은 예외를 던진다.
아래는 자바에서의 배열 작성에 대한 예시이다.
```java
package Test;

public class Main {

	public static void main(String[] args) {
		int[] arr = {1, 2, 3};
		int[] arr2 = new int[10];
		for (int i = 0; i < arr2.length; i++)
			arr2[i] = i;
	}
}
```
# for-each문
`for-each`문은 배열의 원소를 하나씩 꺼내오는 제어문이다. 기존 `for`문은 배열의 원소를 인덱싱을 통해 접근했지만 `for-each`문을 통해 좀 더 직관적이고 간단한 코드 작성이 가능해졌다. 또한 `for-each`문은 배열의 길이만큼 반복한다.

```java
package Test;

public class Main {

	public static void main(String[] args) {
		int[] arr = {1, 2, 3};
		for (int n : arr) // for-each문
			System.out.println(n);
	}
}
```

위 코드는 `int`형 변수 `n`에 `int`형 배열 `arr`의 원소를 하나씩 할당하여 실행하는 코드이다.
# 0605 정보처리기사 실기

### Python 코드의 출력 결과 작성하기

```python
a = "Hello Python"
b = a[0:3]
c = a[-3:-1]
print(b+c)
```
- 답: Heltho

### JAVA 코드의 출력 결과 작성하기
```java
package jscskws;

class A{
	private String s;
	A(){}
	A(String s){
		this.s= s+"A";
	}
	public void fn(String s) {
		System.out.println(this.s + s);
	}
}

class B extends A{
	private String s;
	B(String s){
		this.s = s + "B";
	}
	public void fn(String s) {
		System.out.println(this.s + s);
	}
}

public class exam01 {

	public static void main(String[] args) {
		A a= new B("Hello");
		a.fn("Hi");

	}

}
```

- 답: HelloBHi

### C 언어의 출력 결과 작성하기
```c
#include <stdio.h>
#include <stdlib.h>

int fn(int n) {
	if (n <= 1)
		return 1;
	else
		return n * fn(n - 1);
}

void main() {
	printf("%d", fn(4));
}
```
- 답: 24

### JAVA 코드의 출력 결과 작성하기
```java
package jscskws;

public class exam02 {

	public static void main(String[] args) {
		String s = "red";
		boolean [] b = new boolean[1]; //기본 값을 참으로 세팅완료 
		if(b[0]) s = "blue"; // b[0] false 이므로 실행이 되지 않음
		System.out.println(s);
	}

}

```
- 답: red

### C 코드의 출력 결과 작성하기
```c
#include <stdio.h>
#include <stdlib.h>

void main() {
	int i,j;
	int temp;
	int a[5] = {75,95,85,100,50};

	for (i = 0; i < 4; i++) {
		for (j = 0; j < 4-i; j++) {
			if (a[j] > a[j+1]) {
				temp = a[j];
				printf("%d ", temp);
				a[j] = a[j + 1];
				
				a[j + 1] = temp;
				
			}
		}
	}

	for (i = 0; i < 5; i++) {
		printf("%d ", a[i]);
	}
}
```
- 답: 50,75,85,95,100
- 해설
1. 반복 i:i가 0일때 부터 4보다 작을때까지, 즉 i는 0,1,2,3이 됨.
2. 반복 j: j가 0일때 부터 j가 4-i보다 작아질 때까지
※ 요약 
i가 0일 때, j는 0,1,2,3
i가 1일 때, j는 0,1,2
i가 2일 때, j는 0,1
i가 3일 때, j는 0
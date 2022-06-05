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
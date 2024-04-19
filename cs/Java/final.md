final은 변수, 메서드 클래스를 포함한 여러 곳에 붙을 수 있다.

## 변수에 붙을 때

### 상수와 리터럴

상수는 변하지 않는 저장공간. 리터럴은 기존에 우리가 알던 상수 그 자체 값.

상수는 final키워드로 선언한다.

리터럴은 굳이 상수 변수가 아닌 변수에 있는 Rvalue도 리터럴이다. 자체 값은 변할 수 없기 때문.

```java
final int MAX_SPEED = 100;
int num = 20;
```

100, 20 모두 리터럴.

### 리터럴 접미사

정수형은 L 사용, 실수형은 f,d 사용. d는 생략가능.

```java
long l = 100L;
float pi = 3.14f;
float pi = 3.14; // 에러
double d = 1.23;
```

### 리터럴 진법 접미사

16진수 : 0x
8진수 : 0
2진수 : 0b

### 메소드의 파라미터 변수에 붙을 때

마찬가지로 복사해온 값을 변경할 수 없게 된다.

### 필드로 사용될때

- 반드시 초기화가 필요하다. 생성자 초기화 혹은 필드 초기화.
- 단, 필드초기화는 사실상 중복값이 생성되는 것이기 때문에, static final 변수로 만드는 것이 바람직하다.
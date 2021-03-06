# Lambda 식

## 사용 용도

- 인터페이스의 추상 메소드를 실제로 구현할 때 사용.

## 람다식 형태

- `(parameters) -> 구현부;`

  - 함수명이나 return 타입을 명시하지 않아도됨.
    - 컴파일러가 알아서 찾아줌.
  - 변수명이 하나인 경우 소괄호 생략가능
  - 구현부가 2줄이상인 경우 중괄호를 써야함.

- 람다식을 인터페이스 변수에 담아서 사용할 수 있음.
  - ` Printable printThing = () -> System.out.print("Meow");`

## 람다식 사용 조건

- 람다식을 쓰려면 인터페이스에 추상 메소드가 1개만 있어야함
  - 이런 인터페이스를 SAM(Single Abstract Method) 인터페이스라고도 한다.
- `@FunctionalInterface` 어노테이션을 붙히면 2개이상의 추상 메소드를 구현하는 경우 오류를 나타내기 때문에 기능적 인터페이스 어노테이션을 붙혀주는 것이 좋다.

## 람다식 장점

- 기존 인터페이스를 구현하려면 클래스에 `implements` 예약어를 붙히고 추상메소드를 override하여 구현하는 번거로움이 있다.
- 람다식을 쓰면 위의 방식보다 간단하게 구현 가능함.

### 참고 영상 : https://www.youtube.com/watch?v=tj5sLSFjVj4

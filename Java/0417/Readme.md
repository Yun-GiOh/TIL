# Null Pointer Exception

- 어느 주소도 지정하지 않는 것이 Null Pointer 임

## NPE가 발생하는 상황

### 1. 사용자 클래스 변수

- 한 클래스 변수가 null 이고 그 변수를 통해 접근하려할 경우 NPE가 발생.

### 2. Wrapper 클래스 변수

- boolean 형의 Wrapper 클래스인 Boolean 변수에 null을 할당하고 if문을 사용해도 NPE 발생.
  - 따라서 Boolean 보다는 primitive type인 boolean을 쓰는것이 좋다.

### 3. List와 같은 자료구조 변수

## NPE 해결방법

1. NPE가 발생되는 Null인 변수 정확히 확인하기
2. 초기화하기
3. if문 처리하기
   - method chaining이 여러번 된 값은 그만큼 많은 null 처리를 해야하는 상황 발생 -> 단순하지만 코드가 지저분 해지고 번거로운 방법

### String 객체의 eqauls 함수를 쓸경우 NPE가 발생가능한 변수에 사용하는 것보다 확실히 null이 아닌 String 변수에 equals를 사용하는 것이 좋다.

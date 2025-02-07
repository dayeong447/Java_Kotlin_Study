# 클래스 (Class)
+ 정의: 객체를 생성하기 위한 설계도. 클래스명은 소스 파일명과 동일해야 하며, 첫 글자는 대문자로 시작한다. 여러 단어로 구성된 클래스명은 각 단어의 첫 글자를 대문자로 한다 (예: ```MyClass```).
+ 구성 요소:
멤버 변수 (Member Variable): 클래스 내부에 선언된 변수. 객체의 속성을 나타낸다.
메서드 (Method): 클래스 내부에 정의된 함수. 객체의 동작을 나타낸다.
+ 주석:
블록 주석 (```/* ... */```): 클래스나 메서드에 대한 설명을 작성할 때 사용.
라인 주석 (```// ... ```): 코드 한 줄에 대한 설명을 작성할 때 사용.

# 자료형 (Data Type)
+ 정수형:
```int```: 4바이트 정수 (-2,147,483,648 ~ 2,147,483,647)
```long```: 8바이트 정수 (-9,223,372,036,854,775,808 ~ 9,223,372,036,854,775,807). long 타입 값을 사용할 때는 숫자 뒤에 ```L``` 또는 ```l```을 붙인다 (예: ```1234567890123456789L```).
+ 실수형:
```float```: 4바이트 실수. 숫자 뒤에 ```F``` 또는 ```f```를 붙인다 (예: ```3.14F```).
```double```: 8바이트 실수 (기본 실수형).
+ 문자형:
```char```: 2바이트 문자. 작은따옴표 (```' '```)로 묶는다 (예: ```'A'```).
+ 문자열형:
```String```: 문자열. 큰따옴표 (```" "``` )로 묶는다 (예: ```"Hello"``` ).
+ 논리형:
```boolean```: 참 (```true```) 또는 거짓 (```false```) 값을 갖는다.

# 연산자 (Operator)
+ 증감 연산자:
```i++```: 값을 참조한 후에 1 증가.
```++i```: 값을 참조하기 전에 1 증가.
+ 기타 연산자: ```+```, ```-```, ```*```, ```/```, ```%```, ```=```, ```==```, ```!=```, ```>```, ```<```, ```>=```, ```<=```

# 제어문 (Control Statement)
+ 조건문:
```if```: 조건이 참일 때 코드 블록 실행.
```else```: 조건이 거짓일 때 다른 코드 블록 실행.
```else if```: 여러 조건을 순차적으로 확인하여 참인 경우 코드 블록 실행.
+반복문:
```for```: 정해진 횟수만큼 코드 블록 반복 실행.
```while```: 조건이 참인 동안 코드 블록 반복 실행.
```do-while```: 코드 블록을 먼저 실행하고 조건을 확인하여 참인 경우 반복 실행.
+ 기타 제어문:
```break```: 반복문이나 switch 문을 빠져나감.
```continue```: 반복문의 다음 반복으로 건너뜀.

# 배열 (Array)
+ 정의: 동일한 자료형의 여러 데이터를 순서대로 저장하는 자료구조.
+ 선언 및 초기화: ```자료형[] 배열명 = new 자료형[크기];``` (예: ```int[] arr = new int[5];``` )
+ 접근: ```배열명[인덱스]``` (인덱스는 0부터 시작).

# 리스트 (List)
+ ```ArrayList```: 동적으로 크기가 변하는 배열. ```java.util.ArrayList``` 클래스를 사용.
+ 사용법:
```ArrayList<자료형> 리스트명 = new ArrayList<>();```
```리스트명.add(값)```: 리스트에 값 추가.
```리스트명.get(인덱스)```: 리스트의 값 접근.
```리스트명.remove(인덱스)```: 리스트의 값 삭제.

# 맵 (Map)
+ ```HashMap```: 키-값 쌍을 저장하는 자료구조. ```java.util.HashMap``` 클래스를 사용.
+ 사용법:
```HashMap<키자료형, 값자료형> 맵명 = new HashMap<>();```
```맵명.put(키, 값)```: 맵에 키-값 쌍 추가.
```맵명.get(키)```: 키에 해당하는 값 접근.
```맵명.remove(키)```: 키에 해당하는 키-값 쌍 삭제.

# 문자열 (String)
+ ```String``` 클래스: 문자열을 다루는 클래스.
+ 주요 메서드:
```length()```: 문자열 길이 반환.
```charAt(인덱스)```: 특정 인덱스의 문자 반환.
```substring(시작인덱스, 끝인덱스)```: 부분 문자열 반환.
```equals(문자열)```: 문자열 비교.
```concat(문자열)```: 문자열 연결.
+ ```StringBuffer``` 와 ```StringBuilder```
```StringBuffer```: 문자열을 변경할 수 있는 클래스. 멀티 스레드 환경에서 안전.
```StringBuilder```: StringBuffer 와 유사하지만 싱글 스레드 환경에서 더 빠름.
+ 주요 메서드:
```append(문자열)```: 문자열 추가.
```insert(인덱스, 문자열)```: 특정 위치에 문자열 삽입.
```toString()```: String 객체로 변환.

# 열거형 (Enum)
+ 정의: 연관된 상수들의 집합을 정의하는 자료형.
+ 사용법: ```enum 열거형명 { 상수1, 상수2, ... }```
+ 장점:
코드 가독성 향상.
잘못된 값 사용으로 인한 오류 방지.

# 메서드 (Method)
+ 정의: 클래스 내부에 정의된 함수.
+ 구성 요소:
접근 제어자: 메서드의 접근 권한을 지정 (예: ```public```, ```private```).
반환 자료형: 메서드 실행 후 반환하는 값의 자료형.
메서드명: 메서드의 이름.
매개변수: 메서드에 전달되는 입력값.
메서드 몸체: 메서드의 실제 동작을 정의하는 코드 블록.
호출: ```객체.메서드명(인수)```

# 객체 (Object)
+ 정의: 클래스의 인스턴스.
+ 생성: ```클래스명 객체명 = new 클래스명();```
+ 접근: ```객체명.멤버변수```, ```객체명.메서드명()```

# 생성자 (Constructor)
+ 정의: 객체 생성 시 자동으로 호출되는 메서드.
+ 특징:
클래스명과 이름이 동일.
반환 자료형 없음.
+ 역할: 객체 초기화.

# 상속 (Inheritance)
+ 정의: 기존 클래스의 기능을 물려받아 새로운 클래스를 작성하는 것.
```extends``` 키워드 사용: ```class 자식클래스 extends 부모클래스 { ... }```
+ 장점: 코드 재사용성 향상, 클래스 계층 구조 형성.

# 오버라이딩 (Overriding)
+ 정의: 부모 클래스의 메서드를 자식 클래스에서 재정의하는 것.
+ 목적: 부모 클래스의 메서드를 자식 클래스에 맞게 변경.

# 오버로딩 (Overloading)
+ 정의: 동일한 이름의 메서드를 여러 개 정의하는 것.
+ 조건: 매개변수의 개수 또는 자료형이 달라야 함.

# 인터페이스 (Interface)
+ 정의: 추상 메서드와 상수만으로 이루어진 자료형.
+ ```implements``` 키워드 사용: ```class 클래스명 implements 인터페이스```

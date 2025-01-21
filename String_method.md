문자열 내장 메서드
----------------------

### **indexOf**
+ 특정 문자열이 시작되는 위치 **값**을 리턴
  ```java
  String a = "Hello Java";
  System.out.println(a.indexOf("Java")); // 6 출력
  ```

### **contains**
  + 특정 문자열이 포함되어 있는지 **여부**를 리턴
  ```java
  String a = "Hello Java";
  System.out.println(a.contains("Java")); // true 출력
  ```

### **charAt**
  + 특정 위치의 **문자**를 리턴
  ```java
  String a = "Hello Java";
  System.out.println(a.charAt(6)); // J 출력
  ```

### **replaceAll**
+ 특정 문자열을 다른 문자열로 **바꿀 때** 사용 후 리턴
```java
String a = "Hello Java";
System.out.println(a.replaceAll("Java", "World"); // Hello world 출력
```

### **substring**
+ 특정 문자열을 **뽑아낼 때** 사용 후 리턴 (단, 시작위치 <= a < 끝위치)
```java
String a = "Hello Java";
System.out.println(a.substring(0, 4); // Hell 출력
```

### **toUpperCase**
+ 모두 **대문자**로 변경해서 리턴 (소문자로 변경시에는 toLowerCase)
```java
String a = "Hello Java";
System.out.println(a.toUpperCase()); // HELLO JAVA 출력
```

### **split**
+ 특정한 **구분자**로 나누어 문자열 **배열**로 리턴
```java
String a = "a:b:c:d";
String[] result = a.split(":"); // {"a", "b", "c", "d"} 출력
```

### **String.format**
+ 포매팅된 문자열 리턴
```java
System.out.println(String.format("I eat %d apples.", 3)); // I eat 3 apples. 출력
```
```java
System.out.println(String.format("I eat %s apples.", "five")); // I eat five apples. 출
```
```java
int number = 3;
System.out.println(String.format("I eat %d apples.", number)); // I eat 3 apples. 출력
```
```java
int number = 10;
String day = "three";
System.out.println(String.format("I ate %d apples. so I was sick for %s days.", number, day)); // I ate 10 apples. so I was sick for three days. 출력
```
+ %s format code
```java
System.out.println(String.format("I have %s apples.", 3)); // I have 3 apples. 출력
System.out.println(String.format("Rate is %s.", 3.234)); // Rate is 3.234. 출력
```

#### **System.out.printf**
+ 포매팅된 문자열 출력
```java
System.out.printf("I eat %d apples.", 3); // I eat 3 apples. 출력




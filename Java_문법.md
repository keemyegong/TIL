# Java 문법
### 1. 반복문
```java
  package chap_04;

  public class _Quiz_04 {
    public static void main(String[] args) {
      // int fee = 4000;
      String type = "경차";
      int hour = 5;
      int fee = 0;
      for (int i = 0; i < hour; i++) {
        fee += 4000;
        if (fee >= 30000) {
          fee = 30000;
          break;
        }
    }
    if (type == "경차" || type == "장애") {
      fee *= 0.5;
    };

    System.out.println(type + " 차량 " + hour + "시간 주차 시 " + fee + "원");
    }
  }
```
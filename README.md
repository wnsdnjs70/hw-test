# hw-test


# 사용한 디자인 패턴
1. Factory Method Pattern
2. Abstract Factory Pattern
3. State Pattern
4. Mediator Pattern

이번 과제에서 공부한 패턴은 위와 같다. <br>
먼저 수업 시간에 Factory Method 패턴에 대해 다루며 Abstract Factory 패턴과 어떤 차이가 있는지 궁금했고,<br>
각 패턴은 어떤 특징이 있으며 어떠한 상황에서 Factory Method 패턴 혹은 Abstract Factory 패턴을 쓰는지에 대해 고민해보며 정리하였다. <br>
다음으로 수업 시간에 State 패턴에 대해 공부하며 발생했던 문제를 Mediator 패턴을 통해 해결할 수 있다는 생각이 들어 정리해보았다. <br>

## Simple Factory Pattern
팩토리 패턴에는 Factory Method 패턴과 Abstract Factory 패턴이 있다. 이 두가지 패턴에 앞서 Simple Factory 패턴에 대해 정리하였다.<br>
Simple Factory Pattern은 간단히 말해 객체를 생성하는 클래스를 따로 두는 패턴을 말한다. <br>
factory_pattern 패키지의 SimplePhoneFactory 클래스를 보면 createPhone 메서드의 switch문를 통해 <br>
클라이언트가 주문할 휴대폰의 객체를 직접 생성하는 것을 볼 수 있다. <br>
심플 팩토리는 단순히 객체를 만드는 작업을 하나의 팩토리 클래스에 모아두는 것을 의미한다. <br>

## Factory Pattern
팩토리 메소드 패턴의 정의는 아래과 같다.<br>

객체를 생성하기 위한 인터페이스를 정의하는 과정에서 어떤 클래스의 인스턴스를 만들지는 서브클래스에서 결정한다. <br>
즉, 클래스의 인스턴스를 만드는 일을 서브클래스에게 맡기는 것이다. <br>

다시 말해 심플 팩토리 패턴에서 createPhone() 부분에서 Factory에서 직접 객체를 만드는 것을 Factory를 상속한 서브클래스에서 객체를 만들게끔 하는 것이 팩토리 메소드 패턴이다. <br>

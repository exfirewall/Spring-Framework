## JPA란?
 * Java Persistence API (자바 ORM 기술에 대한 API 표준 명세)
 * ORM을 사용하기 위한 인터페이스를 모아둔 것 이라고 볼 수 있다.
 * 자바 어플리케이션에서 관계형 데이터베이스를 사용하는 방식을 정의한 인터페이스이다.
 * ORM에 대한 자바 API 규격이며 Hibernate, OpenJPA 등이 JPA를 구현한 구현체 이다.
 * Hibernate 이외에도 EcipseLink, DataNucleus, OpenJPA, TopLink 등이 있다.
 
※결국 인터페이스이기 때문에 JPA를 사용하기 위해서는 JPA를 구현한 Hibernate, EclipseLink, DataNucleus 같은 ORM 프레임워크를 사용해야 한다.

## Hibernate?
 * JPA를 사용하기 위해서 JPA를 구현한 ORM 프레임워크중 하나.
   (자바를 위한 오픈소스 ORM(Object-relational mapping) 프레임워크를 제공한다.)
 * Hibernate는 JPA 명세의 구현체이다. javax.persistence.EntityManager와 같은 JPA의 인터페이스를 직접 구현한 라이브러리이다.

▶ 장점
 - 생산성이 뛰어나고 유지보수가 용이하다.(데이터베이스 중심 설계에서 객체 중심 설계로 변경됨에 따른)
 - 객체 지향적인 코드로 인해 더 직관적이고 비즈니스 로직에 더 집중할 수 있게 도와준다.
 - 객체지향적으로 데이터를 관리할 수 있기 때문에 전체 프로그램 구조를 일관되게 유지할 수 있다.
 - SQL을 직접적으로 작성하지 않고 객체를 사용하여 동작하기 때문에 유지보수가 더욱 간결하고, 재사용성도 증가하여 유지보수가 편리해진다.
 - DB컬럼이 추가될 때마다 테이블 수정이나 SQL 수정하는 과정이 많이 줄어들고, 값을 할당하거나, 변수 선언등의 부수적인 코드 또한 급격히 줄어든다.
 - 각각의 객체에 대한 코드를 별도로 작성하여 코드의 가독성도 올라간다.

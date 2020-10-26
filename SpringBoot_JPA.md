## JAP란?
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

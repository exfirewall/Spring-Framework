# Spring boot dashboard 

### spring boot란?
스프링을 쉽게 사용하게 하기 위해 필요한 초기 설정을 대부분 미리 세팅해놓은 스프링 프로젝트

### spring boot의 특징
* 단독으로 실행이 가능한 스프링 애플리케이션을 생성함
* Tomcat, Jetty, Undertow 등 서버 내장
* 상용화에 필요한 통계, 상태 체크, 외부 설정 등을 제공
* 설정을 위한 XML 코드를 생성하거나 요구하지 않음
* jar파일 형식으로 배포 가능

### spring boot 시작하기

[visual code에서 spring boot 시작하기](https://medium.com/@boxone80/visual-studio-code-%EC%97%90%EC%84%9C-spring-boot%EC%82%AC%EC%9A%A9%EB%B2%95-a20e2595be2d)  
난 익숙한 vscode에서 할래....

----------------------
### 시작부터 막힘

`Error : Failed to configure a DataSource: 'url' attribute is not specified and no embedded datasource could be configured.`

MySQL 초기설정을 빠뜨렸다. src > main > resources > application.properties 에 들어가서 아래와 같이 설정해준다.

spring.datasource.url=jdbc:mysql://localhost:3306/[DB스키마명]?serverTimezone=UTC&characterEncoding=UTF-8  
spring.datasource.username=[DB접속Id]  
spring.datasource.password=[DB접속Password]  
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver  



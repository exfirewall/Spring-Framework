# 1. Spring MVC

![spring_mvc_architecture](./springmvc-architecture.png)

### spring 전체 흐름
`client request -> DispatcherServlet -> Controller(Servlet) -> response (Model & View 이용) -> View(JSP), ViewResolver`

* Dispatcher
  * model2로 가면서 controller와 분리
  * 단순히 request를 전달하는 역할만 하는 것이 아니라 controller가 사용하기 쉽게 포맷을 만들어서 전달해줌
  * 기본형 뿐만아니라 객체도 전달 가능. controller 측에서는 servlet 라이브러리 사용안하고 처리 가능해짐
  * spring MVC를 쓴다는 것은 DispatcherServlet.class를 사용하는 것

# 1. Spring MVC

![spring_mvc_architecture](./springmvc-architecture.png)

### spring 전체 흐름
`client request -> DispatcherServlet -> Controller(Servlet) -> response (Model & View 이용) -> View(JSP), ViewResolver`

* Dispatcher
  * Controller와 분리된 이유

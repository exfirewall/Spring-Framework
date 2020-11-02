# Errors you may encounter
------------


1. 에러
```
Error Code: 1364(HY000) Field 'id' doesn't have a default value
```

2. 원인  

이는 파일에 정의 된 STRICT_TRANS_TABLES SQL 모드로 인해 발생합니다. 
```
%PROGRAMDATA%\MySQL\MySQL Server 5.6\my.ini
```
3. 해결

* 해당 설정을 제거하고 MySQL을 다시 시작하면 문제가 해결된다.
* 스키마에 기본값을 할당한다. ALTER 명령으로 수행.

```SQL
ALTER TABLE employee MODIFY empno int NOT NULL AUTO_INCREMENT;
```
---------

column 명명 규칙을 지키지 않으면 자동으로 column명을 바꿔서 새로운 column을 추가한다.
```java  
@Column(name="empCode")
  private Integer empCode;
```
에서 column을 empCode라 했을 때  

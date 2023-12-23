# ServerStudy6Cloud
이 리포지토리를 통해서 Spring Boot에서 AWS RDS의 데이터를 조회 및 업로드하는 기능을 구현할 수 있습니다.

## To-Do List
1. application.yml 파일을 수정해주세요.
```yaml
# RDS
spring:
  datasource:
    url: jdbc:mysql://[AWS RDS Endpoint]:3306/study6
    username: admin
    password: [Password]
    driver-class-name: com.mysql.cj.jdbc.Driver
  # hibernate
  jpa:
    show-sql: true
    hibernate:
      ddl-auto: update
      dialect: org.hibernate.dialect.MySQL8Dialect
```

2. RdsRepository.java 파일을 수정해주세요.
```java
public class RdsRepository {
    //DB에 새로운 책 저장하는 메서드

    //DB에서 모든 책 리스트 가져오는 메서드
}

```

3. RdsService.java 파일을 수정해주세요.
```java
public class RdsService {
    //RdsRepository를 사용해 DB에 저장하는 로직

}
```

4. BookForm.java 파일 내용을 완성하고, RdsController.java 파일을 수정해주세요.
```java
public class BookForm {
    //책 이름, 책 좋아하는 이유
}

```
```java
public class RdsController {
    //AWS RDS에서 Book list를 가져오는 GetMapping

    //AWS RDS에 Book 객체를 저장하는 PostMapping
}

```

# Using AspectJ with Spring boot applications 

기존에 JavaFX + Spring Boot의 조합으로 프로젝트를 진행한 적이 있었다. 

프로젝트를 진행하면서 제일 아쉬웠던 부분은 특정 오브젝트는 Spring Bean으로 생성하는게 아닌 `new`로 인스턴스화를 해야 하는데

그럴때 마다 Spring의 @Autowired를 사용하지 못하는게 정말 아쉬웠다.

AspectJ를 이용하면 일반 인스턴스를 생성하면서도 스프링의 IoC를 이용할수 있다.

> Load-time weaving 설정에 필요한 파일은 'ext_lib/spring-instrument.jar'에 두웠다.


## 참고

[@Configurable 사용방법](https://docs.spring.io/spring/docs/4.3.12.RELEASE/spring-framework-reference/htmlsingle/#aop-atconfigurable)

[Load-time weaving 설정](https://docs.spring.io/spring/docs/4.3.12.RELEASE/spring-framework-reference/htmlsingle/#aop-aj-ltw)
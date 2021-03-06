
@WebFluxTest – we can use the @WebFluxTest annotation to test Spring Webflux controllers. It’s often used along with @MockBean to provide mock implementations for required dependencies.

@JdbcTest – we can use the @JdbcTest annotation to test JPA applications but it’s for tests that only require a DataSource. The annotation configures an in-memory embedded database and a JdbcTemplate.

@JooqTest – To test jOOQ-related tests we can use @JooqTest annotation, which configures a DSLContext.

@DataMongoTest – To test MongoDB applications @DataMongoTest is a useful annotation. By default, it configures an in-memory embedded MongoDB if the driver is available through dependencies, configures a MongoTemplate, scans for @Document classes, and configures Spring Data MongoDB repositories.

@DataRedisTest – makes it easier to test Redis applications. It scans for @RedisHash classes and configures Spring Data Redis repositories by default.

@DataLdapTest – configures an in-memory embedded LDAP (if available), configures a LdapTemplate, scans for @Entry classes, and configures Spring Data LDAP repositories by default

@RestClientTest – we generally use the @RestClientTest annotation to test REST clients. It auto-configures different dependencies like Jackson, GSON, and Jsonb support, configures a RestTemplateBuilder, and adds support for MockRestServiceServer by default.

Refer to: Spring boot testing (https://www.baeldung.com/spring-boot-testing)

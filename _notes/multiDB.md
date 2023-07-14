
Java Spring framework provides support for multiple databases through the use of multiple DataSources. Each DataSource can be configured to connect to a different database and can be referenced in the application by its unique identifier. The configuration can be done in the application.properties or application.yml file and can be defined using the spring.datasource prefix followed by the relevant properties.

For example, to define two databases in the application, the configuration would look like this:

spring.datasource.db1.url=jdbc:mysql://localhost:3306/db1 spring.datasource.db1.username=root spring.datasource.db1.password=password

spring.datasource.db2.url=jdbc:mysql://localhost:3306/db2 spring.datasource.db2.username=root spring.datasource.db2.password=password

In the code, the application can reference the different databases by annotating the relevant repositories or services with the @Qualifier annotation and the DataSource name.

For example,

@Autowired @Qualifier("db1") private DataSource dataSource1;

@Autowired @Qualifier("db2") private DataSource dataSource2;




trace 폴더 통으로 삭제 
메일 주
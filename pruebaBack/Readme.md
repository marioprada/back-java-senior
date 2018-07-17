# Prueba Técnica: Proyecto base
Actualmente en The Cocktail, utilizamos:
- IDE: IntelliJ IDEA
- Lenguaje: Groovy/Java
- Framework: Spring boot (puedes usar Spring MVC)
- Pruebas: Spock framework (puedes utilizar cualquier herramienta)
- BBDD: Oracle (puedes usar la que quieras, recomendamos H2 u otra BBDD in memory)
Para el desarrollo de nuestras aplicaciones tenemos unos módulos reutilizables de arquitectura, que no son necesarios para este proyecto.
## Proyecto base
Se adjunta la estructura del proyecto en el repo (pruebaBack). Esta estructura está creada en Groovy. Si prefieres hacerlo en Java, puedes generar el proyecto con  Spring Initializr, desde su [web](https://start.spring.io/) o en el wizard integrado en IntelliJ con las siguientes dependencias:
### Grupo: Web
- Módulo: Web
Full-stack web development with Tomcat and Spring MVC
### Grupo: SQL
- Módulo: JPA
Java Persistence API including spring-data-jpa, spring-orm and Hibernate
- Módulo: H2 (En caso de elegir H2 como BBDD)
H2 database (with embedded support)

**Documentar el API Rest con swagger y swagger-ui.**
### Configuración Datasource
Si utilizas H2 como database, añade al application.yml la configuración:
> spring.datasource.url=jdbc:h2:mem:domain;DB_CLOSE_ON_EXIT=FALSE
> spring.datasource.username=
> spring.datasource.password=
> spring.datasource.driver-class-name=org.h2.Driver
> spring.jpa.hibernate.ddl-auto=create-drop
> spring.jpa.database-platform=org.hibernate.dialect.H2Dialect
> spring.jpa.show-sql=false

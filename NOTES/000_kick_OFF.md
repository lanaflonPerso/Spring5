### About Spring
- Versions: Spring 3.0 (2009) > Spring3.1 (2011) > Spring4.3.16() > Spring5()

#### A. Resources
1. [tutorialspoint](https://www.tutorialspoint.com/spring/spring_overview.htm)
2. [mykong](https://www.mkyong.com/spring)

***

#### B. Feature:
1. `open source` Java platform that provides comprehensive **infrastructure support** for developing robust Java applications. 
2. Application developed using POJOs, no EJB needed. Lightweight IoC containers compared to EJB Container.
3. Servlet Container Analogy.

***

#### C. Core Feature 
##### C.1. DI / IOC
1. Loosely coupled code.
2. Class A and Class B - dependency exmaple.
3. Factory Design pattern.



##### C.2. AOP
1. cross-cutting concerns (logging, transactions, security, caching, metric, etc) --> separate from the application's business logic

***

#### D. Framework of frameworks
- Spring provides multiple Modules.

1. Data Access/Integration
> `JBDC` - JDBC-abstraction layer that removes the need for tedious JDBC related coding

> `ORM` - Support to JPA and Hibernate framework.

> `JMS` - features for producing and consuming messages.

> `Transaction` - programmatic and declarative transaction management

2. Core Modules  
> `core` - IoC and Dependency Injection features

> `Bean` - BeanFactory

> `Context`  - ApplicationContext

> `SpEL` - powerful expression language for querying and manipulating an object graph at runtime. - extension over EL deined in JSP like : method invocation,accessing collection,etc.

3. web
> `web-MVC` - Spring MVC for webapp.

> `web, portlet, websocket,etc` - ?


4. Test
> Junits

5. AOP 
- aspect-oriented programming 
- method-interceptors and pointcuts to cleanly decouple code.

***



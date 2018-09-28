## Spring Cotainer
- Understand it with Analogy with Servlet Container.
- in a spring project can have multiple AC.
- can load multiple xml config into a single AC.
- light weigth container - no installion is needed, just collection of jars.

***
### Features:
- factory of `Beans (POJO)`.
- handles construction > `life Cycle` > destruction of Beans.
- Container needs `metadata` to create Bean. `Spring-config.xml` at classPath.
- `BeanFactory` and `ApplicationContext` - provides interface to BeanFactory to get Bean. 


***
### ApplicationContext
#### 1. Different Implementation
> 1. `ClassPathXmlApplicationContext("s.xml")`

> 2. `FileSystemXmlAC()`
***
### BeanFactory
#### 1. Different Implementation
> 1. `XmlBeanFactory(NewFileSystemResource("s.xml"))`


***
### Difference between ApplicationContext and BeanFactory
1. BF lazy loads the Singleton.
2. AC can do everytime BF does. BF still their for backward compatibility.



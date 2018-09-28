## Injection
- Inject primitive type, object, collection (List,Map,Set).
- Spring Context is also responsible for injection dependencies in the bean, either through `setter` or `constructor` or `autowiring`.

***

### A. Setter Injection
- `<property>` - it uses setter method to inject.
- attribites: 
> `ref` - to inject object type by bean name, bean id, bean alias name.

> `idref` - to inject object type by bean id.

> `value` - to inject primitive type.

***
### B. Constructor Injection

#### key point
- `<contructor-arg>` - it invokes constructor to inject.
- use `index` (start with 0) and `type`
- type = "int", "java.lang.String", "float",etc.  // String is not primitive type.

***
### C. Autowiring
#### C.1. autowire attribute

#### C.2. @autowire

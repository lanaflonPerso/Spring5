### About Bean
- POJO class
- `inner Bean` - how to create it and purpose.
- create alias of Bean : 
`<alias name="id of bean" alias-name="new name">`

- `<Bean>` attributes
> 1. `id`

> 2. `class`

> 3. `scope`

> 4. `name` and `alias-name`

> 5. `parent` - to inherit bean definiton from abstract bean template.

***

### A. Scope
#### 1. Prototype

#### 2. Singleton (default)

`Note` : 3 more types, only for web appication:
#### 3. Request
- new Bean per http request

#### 4. Session
- new bean per session request

#### 5. Global
- new one bean for entire web app.

***
### B. LIFE-CYCLE of a Bean:

***

### C. Callback Life cycle method
- Sometimes we want to initialize resources in the bean classes - initialize services, database connections,etc before initialization of bean.
- Spring different ways of post-initialization and pre-destroy in a spring bean life cycle.
1. By implementing `InitializingBean` and `DisposableBean` interfaces. Overide:
> `destroy()` 
> `afterPropertiesSet()`

2. Providing `init-method` and `destroy-method` attribute.
```
<bean name="id1" class="abc" 
    init-method="init" destroy-method="destroy">
```

3. `@PostConstruct` and `@PreDestroy` annotations.
```
@PreDestroy 	public void destory(){ ... }
@PostConstruct	public void init(){ ... }
```
- [detailed eg - journelDev](https://www.journaldev.com/2637/spring-bean-life-cycle#spring-bean-life-cycle)

***

### D. Bean Aware:
interface which bean class implements to make itself aware about Application context, bean name, classloader,etc

#### 1. ApplicationContextAware.

#### 2. ApplicationContextEvent.

#### 3. BeanClassLoaderAware.

#### 4. BeanNameAware.
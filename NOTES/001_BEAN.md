### About Bean
- POJO class
- `inner Bean` - how to create it and purpose.
- create alias of Bean : 
`<alias name="id of bean" alias-name="new name">`

- `<Bean>`
> `id`

> `class`

> `scope`

> `name` and `alias-name`

> `parent` - to inherit bean definiton from abstract bean template.

***

### A. Scope
#### 1. Prototype

#### 2. Singleton (default)

Note : 3 more only for web appication:

#### 3. Request
- new Bean per http request

#### 4. Session
- new bean per session request

#### 5. Global
- new one bean for entire web app.

***
### B. LIFE-CYCLE of a Bean:

***
### C. Bean Aware:
interface which bean class implements to make itself aware about Application context, bean name, classloader,etc

#### 1. ApplicationContextAware.

#### 2. ApplicationContextEvent.

#### 3. BeanClassLoaderAware.

#### 4. BeanNameAware.
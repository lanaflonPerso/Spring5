## Annotation Based Container Specification

### feature:
1. For Each annotation there is a correspoding BeanPostProcessor, that has to be present in spring.xml to make that annotation work.
2. eg: @required, add: `<bean=...RequiredAnnotationBeanPostProcessor>` in spring.xml.
3. rathor than adding beanpostProcessor for each anno, just add global config for all anno: `<context:annotation:config/>`

### Annotation:
#### 1. @required
> To mark a mandatory instance.

#### 2. @autowire @qualifier(name="")
- `<bean=...RequiredAnnotationBeanPostProcessor>`
- It looks for _bean type_ and if ambigious, then looks for _bean name_
- cant use with primitive, String, Integer,etc.
- type:
1. **by name**

2. **by type**

#### 2. Stereotype annotation
##### key points:
- default bean id --> [ Eg Class - Abc, then id is abc.]

##### anno
> 1. `@Component` 

> 2. `@Controller`

> 3. `@Repositoty`

> 4. `@Service`



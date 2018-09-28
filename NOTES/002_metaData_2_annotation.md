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
- type:
1. **by name**

2. **by type**

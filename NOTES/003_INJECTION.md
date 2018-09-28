## Injection
- Inject primitive type, object, collection (List,Map,Set).
- Spring Context is also responsible for injection dependencies in the bean, either through `setter` or `constructor` or `autowiring`.
- Step:
```
1. object created > 
2. inject dependencies >
3. which object to inject : find by strategies 
    3.1 if xml autowire attribute,then 5 strategies : no, auto,type, name, contructor 
    3.2. @autowire anno then 2 stragies: type then name)
    
    note: All strategies either invoke setter or contructor to inject object. these are only 2 ways or types of injection.
```
***
#### A. Types:
### TYPE 1. Setter Injection
- `<property>` - it uses setter method to inject.
- attribites: 
> `ref` - to inject object type by bean name, bean id, bean alias name.

> `idref` - to inject object type by bean id.

> `value` - to inject primitive type.

***
### TYPE 2. Constructor Injection
#### key point
- `<contructor-arg>` - it invokes constructor to inject.
- use `index` (start with 0) and `type`
- type = "int", "java.lang.String", "float",etc.  // String is not primitive type.

### TYPE 3. method Injection (One more)

***

### B. Strategies for Autowiring
#### 1. autowire attribute - 5 Strategies
> [ no, auto,type, name, contructor ]

1. it autowires all properties of class ABC - o1 and o2.
```
class ABC{
    Object1 o1;
    Object2 o2;
}

< bean class="ABC" autowire="name"/> // o1 and o2 both get autowired.
```

#### 2. @autowire - 2  Strategies
> [type, name]

1. we can restrict autowiring to specific property.
```
@autowire 
Object1 o1;

Object2 o2; //never be autowired.
```
***


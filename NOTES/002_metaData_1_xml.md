## XML based Metadata:

### key points
1. id must be unique
2. name must be unique ?

### 1. Placehlder
1. [PropertyPlaceholderConfigurer example ](https://www.mkyong.com/spring/spring-propertyplaceholderconfigurer-example/)
2. ${variable} format
3. code eg:
```
<bean 
class="org.springframework.beans.factory.config.PropertyPlaceholderConfigurer">
        <property name="location">
			<value>database.properties</value>
        </property>
</bean>
    
```

### 2. Autowire
- developer dont need to explicity inject all properties inside bean by using `<constructor-arg>` or `<parameter>`. Autowiring will inmplicitly inject other properties based on match. Below are 5 types to get best match.
```
<bean id="" class="" autowire="">
```
> 1. 'by name' --> one of class property is `Object1 abc` > spring will search for bean (with name=abc or id="abc") in container and inject it. [ Object name and Bean id must be same ]


> 2. 'by type' --> one of class property is `Object1 abc` > spring will search for bean (with type=Object1) in container and inject it. If Object1 abc2 exist, then error.

> 3. 'autodetect'

> 4. 'constructor'

> 5. 'no' (default)
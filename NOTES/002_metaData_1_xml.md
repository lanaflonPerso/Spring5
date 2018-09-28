## XML based Metadata:

### Placehlder
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
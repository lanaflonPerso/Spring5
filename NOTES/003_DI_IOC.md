## DI - Dependency Injection
- Class dependency chain. (class1 has a class2 has a class3 ...). Difficult to maintain if any of these class in modified.
- hence defined these dependencies in one central location. outSurce the object creation task
- Before Spring : factory Design pattern.
- Spring's implementation of **Factory Design pattern** which removes class dependency from code. hence makes code `loosely coupled` which is `maintainable`.
- These dependencies are defined in external metadata (`configurable`) and spring injects these dependencies explicity via 3 ways: setter, constructor aor autowire.

- So whenever a object is intialized all it dependent would also be created and injected to it by Spring Container.




## IOC - Inversion of Control
- Spring Inversting the control of creating object.
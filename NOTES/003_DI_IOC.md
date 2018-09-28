## DI - Dependency Injection
- Class dependency chain. (class1 has a class2 has a class3 ...). Difficult to maintain if any of these class in modified.
- hence defined these dependencies in one central location.
- Before Spring : factory Design pattern.
- Spring's implementation of **Factory Design pattern** which removes class dependency from code. hence makes code `loosely coupled` which is `maintainable`.
- These dependencies are defined in external metadata (`configurable`) and spring injects these dependencies explicity via 3 ways: setter, constructor aor autowire.




## IOC - Inversion of Control
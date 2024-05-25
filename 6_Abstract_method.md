- Abstract modifier is applicable only for classes and methods
- Abstract method only has a declaration but not an implementation. Their implementation should be provided by child classes
```java
public abstract void m1() {} // incorrect
public void m1(); // incorrect
public abstract void m1(); // correct
public void m1() {} // correct
```
- If a class contains at least one abstract method, the class needs to be declared as abstract
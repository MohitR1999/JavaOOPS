- Whenever we are extending any abstract class, the child class must provide implementations for all abstract methods inside that class, otherwise we will get compile time error
- If we are not providing implementations for all the methods in the child class, then we need to declare the child class as abstract too. Then its child will provide implementation for the remaining methods and only that class can be instantiated.
#### Example
```java
/*
Abstract class vehicle
*/
public abstract class Vehicle {
	public abstract int getWheels();
}
```
```java
/*
Concrete class Bus
*/
public class Bus extends Vehicle {
	@Override
	public int getWheels() {
		return 6;
	}
}
```
```java
/*
Concrete class Auto
*/
public class Auto extends Vehicle { 
	@Override
	public int getWheels() {
		return 3;
	}
}
```
```java
/*
Driver code
*/
public class App {
	public static void main(String[] args) {
		Vehicle vehicle = new Bus();
		System.out.println(vehicle.getWheels()); // output : 6
		vehicle = new Auto();
		System.out.println(vehicle.getWheels()); // output : 3
	}
}
```

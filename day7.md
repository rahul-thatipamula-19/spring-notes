**java configurations**

Dependency Injection:
	objects created by spring framework are injected into another object.
	Dependency Injection (DI) in Spring is a design pattern that allows the Spring framework to manage the dependencies of a class automatically. Instead of creating dependencies manually inside a class, they are **injected** by the Spring container at runtime. This promotes loose coupling and makes code more maintainable and testable.

### **How Dependency Injection Works in Spring?**

Spring provides DI by automatically injecting required dependencies into a class. It does this using:

1. **Constructor Injection**
2. **Setter Injection**
3. **Field Injection (Not Recommended)**  //not supported by XML config
![[Pasted image 20250219230034.png]]


![[Pasted image 20250219230120.png]]

![[Pasted image 20250219231105.png]]

in POV of servlets

![[Pasted image 20250211064140.png]]


![[Pasted image 20250211064455.png]]

![[Pasted image 20250211064519.png]]




IOC(Inversion of control) :

**Inversion of Control (IoC)** is a design principle where **the control of object creation and dependency management is transferred from the developer to a framework or container**.

->IOC is known as Implementation of DI(dependency Injection).
-> IOC container will create the objects at the first runtime instance of the java application.
![[Pasted image 20250211065149.png]]
->Internally the IOC container follows Dependency injection.


***Spring IOC Container :*** 

  The **Spring IoC (Inversion of Control) Container** is the **core of the Spring Framework**. It **manages the lifecycle** and **dependencies of objects (beans)** in a Spring application.

🔹 **What does it do?**  
✔ **Creates objects (beans)**  
✔ **Manages dependencies** (Dependency Injection - DI)  
✔ **Controls the lifecycle** of beans (initialization, destruction)  
✔ **Promotes loose coupling** by handling object dependencies externally
Bean wiring:
	**Bean wiring** is the process of configuring dependencies between Spring beans so that the Spring container knows how to manage and inject them. It helps in creating relationships between objects using **dependency injection (DI)**.


![[Pasted image 20250221070727.png]]

![[Pasted image 20250221070908.png]]



### **Autowiring in Spring**

**Autowiring** is a feature in Spring that allows the Spring container to **automatically inject** dependencies into beans without needing explicit configuration. It helps reduce boilerplate code and simplifies dependency injection.

Ways to create ioc container:
->BeanFacotry: org.springframework.beans.factory
->ApplicationContext: org.springframework.context.ApplicationContext.
	applicationcontext is the child interface of BeanFactory interfacen.
		BeanFactory interface is the root interface.

**BeanFactory is deprecated from spring 3**

![[Pasted image 20250221071911.png]]


->@component : In Java, `@Component` is an annotation used in **Spring Framework** to indicate that a class is a Spring-managed component. It is a **stereotype annotation**, meaning that it marks a class as a candidate for **Spring's dependency injection** mechanism.

### **Usage of `@Component`**

When a class is annotated with `@Component`, Spring automatically detects and registers it as a **bean** in the **Spring application context** during component scanning.

### **Injecting `@Component` Bean**

You can **inject** this component into another class using `@Autowired`

![[Pasted image 20250226225953.png]]
-> the product2 is returned using the name of the bean which is passed through the @Component("id");


->When there are multiple beans,then passing ClassName.class is not a good approach. Due to ambiguoty issue.
->If only one bean object is enough then @component is a good choice.
->More than one bean object for same class., Then @Config (manual configuration ) is better.

-> @ComponentScan(basePackages={package list.....} );
![[Pasted image 20250226231947.png]]
same, but approach is different.





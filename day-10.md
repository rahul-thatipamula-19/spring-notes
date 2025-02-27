Constructor injection:
Constructor: In java, it is a block which will be executed at object creation.
->It it used to initialize default values to instance variables.
-> Based on beans configuration: Is we are using 

->in constructor injection the injection happens while object creation with constructor execution.
-> while writing the constructor arg.. the order should be preserved.


![[Pasted image 20250220182627.png]]



->If default constructor is not defined then it supports only constructor injection.
->If default constructor is there along with parameterized constructor.. then both setter injection and constructor injection is possible.
![[Pasted image 20250220183733.png]]

**setter and constructor injection**
```
<bean id="student" class="com.example.Student">
    <!-- Constructor Injection -->
    <constructor-arg value="Rahul"/>
    <constructor-arg value="22"/>
    
    <!-- Setter Injection -->
    <property name="grade" value="A"/>
</bean>
```

![[Pasted image 20250221064338.png]]

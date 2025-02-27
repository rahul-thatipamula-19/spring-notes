![[Pasted image 20250221210438.png]]

In **Spring Framework**, **bean scope** defines the **lifecycle and visibility** of a bean (i.e., how and when a bean is created, shared, or disposed of in the Spring container).

#beanscope
### **Types of Bean Scopes in Spring**

Spring provides the following bean scopes:

#### **1. Singleton (Default)**

- **Only one instance** of the bean is created for the entire Spring container.
    
- All requests for the bean return the same instance.
    
- Used for stateless beans.
- 
    `@Bean @Scope("singleton")  // or @Scope(ConfigurableBeanFactory.SCOPE_SINGLETON) public MyBean myBean() {     return new MyBean(); }`
    
![[Pasted image 20250226182352.png]]

#### **2. Prototype**

- A **new instance** is created every time the bean is requested.
    
- Used for stateful beans where separate instances are needed.

    `@Bean @Scope("prototype")  // or @Scope(ConfigurableBeanFactory.SCOPE_PROTOTYPE) public MyBean myBean() {     return new MyBean(); }`
    
![[Pasted image 20250226182930.png]]

#### **3. Request (Web Applications)**

- A **new bean instance is created per HTTP request**.
    
- Used in **Spring MVC** applications.

    `@Bean @Scope("request")  // or @Scope(WebApplicationContext.SCOPE_REQUEST) public MyBean myBean() {     return new MyBean(); }`
    

#### **4. Session (Web Applications)**

- A **single bean instance is created per user session**.
    
- Used for storing user-specific data.
    
    `@Bean @Scope("session")  // or @Scope(WebApplicationContext.SCOPE_SESSION) public MyBean myBean() {     return new MyBean(); }`
    

#### **5. Application (Web Applications)**

- A **single instance of the bean is created per ServletContext**.
    
- Useful for application-wide shared beans.

    `@Bean @Scope("application")  // or @Scope(WebApplicationContext.SCOPE_APPLICATION) public MyBean myBean() {     return new MyBean(); }`
    

#### **6. WebSocket (Web Applications)**

- A **single instance is created per WebSocket session**.
    
- Used for **real-time applications** with WebSockets.
    
    `@Bean @Scope("websocket")  // or @Scope(WebApplicationContext.SCOPE_WEBSOCKET) public MyBean myBean() {     return new MyBean(); }`
    

### **Which Scope to Use?**

- **Singleton**: When you need shared resources (e.g., service classes, DAOs).
- **Prototype**: When you need new objects every time (e.g., form data objects).
- **Request/Session**: For web applications to handle request- or session-specific data.
- **Application**: For global resources like caches.
- **WebSocket**: For real-time communication. 



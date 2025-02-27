->we can pass the beanconfiguration class name through constructor of AnnotationConfigApplicationContext() and through register() method of that class.

->if we use register() method.. then in the next step we have to use refresh() method.
->we can also pass as many configurations classes as possible by seperating using comma.  
->we can call register() method as many times as possible.
->When using `context.register()`, you must call `context.refresh()` to initialize the Spring context. `register()` only registers configuration classes but does not create or wire beans. `refresh()` completes the initialization by scanning for beans, resolving dependencies, and starting lifecycle components. If you pass the configuration class to the `AnnotationConfigApplicationContext` constructor, `refresh()` is called automatically.


->we completed
![[Pasted image 20250226225042.png]]

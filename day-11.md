|Feature|Constructor Injection|Setter Injection|
|---|---|---|

|   |   |   |
|---|---|---|
|**Definition**|Dependencies are passed via the constructor.|Dependencies are passed via setter methods.|

|   |   |   |
|---|---|---|
|**Mutability**|Creates an immutable object; dependencies are set at the time of object creation.|Creates a mutable object; dependencies can be changed anytime.|

|   |   |   |
|---|---|---|
|**Required Dependencies**|Best for mandatory dependencies, as they must be provided at object creation.|Best for optional dependencies, as they can be set later.|

|   |   |   |
|---|---|---|
|**Testability**|Easier to test with immutable dependencies.|Can be tested, but dependency changes might affect test consistency.|

|   |   |   |
|---|---|---|
|**Boilerplate Code**|Less code since dependencies are injected directly.|More boilerplate due to setter methods.|

|   |   |   |
|---|---|---|
|**Circular Dependency Handling**|Can cause circular dependency issues, which may require `@Lazy` or breaking the cycle.|Less prone to circular dependency issues.|

|   |   |   |
|---|---|---|
|**Use Case**|Preferred when all dependencies are mandatory and known at object creation.|Preferred when dependencies are optional or may change over time.|


### **What is a POJO?**

A **POJO (Plain Old Java Object)** is a simple Java class that does not depend on any specific framework or library. It is used to represent data and typically consists of fields (variables), getters, setters, constructors, and sometimes `toString()`, `equals()`, and `hashCode()` methods.

### **Characteristics of a POJO**

1. **No Special Restrictions** – A POJO is a normal Java object without special requirements like extending a class or implementing an interface.
2. **Encapsulation** – Fields are private, and access is provided through getters and setters.
3. **No Heavy Framework Dependencies** – Unlike Java Beans, POJOs do not require annotations or configurations.
4. **Serializable (Optional)** – Can implement `Serializable` for object serialization.


| Feature | POJO | JavaBean | DTO (Data Transfer Object) |
| ------- | ---- | -------- | -------------------------- |
|         |      |          |                            |

|   |   |   |   |
|---|---|---|---|
|**Encapsulation**|Yes|Yes|Yes|

|   |   |   |   |
|---|---|---|---|
|**Getters/Setters**|Optional|Mandatory|Mandatory|

|   |   |   |   |
|---|---|---|---|
|**No-arg Constructor**|Optional|Required|Required|

|   |   |   |   |
|---|---|---|---|
|**Serializable**|Optional|Yes|Yes|

|   |   |   |   |
|---|---|---|---|
|**Framework Independent**|Yes|No (follows JavaBean spec)|No (used for data transfer)|

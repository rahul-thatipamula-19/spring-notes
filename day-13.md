![[Pasted image 20250221195234.png]]

**autowiring** does not support for primitives and string data.. and can only for reference objects.

Auto wiring can be enabled in four ways
1. by defualt autowiring in spring  wrto XML config. We need to use an attribute called as autowire as part of //bean.
2. autowire attribute support 4 values. 
	1. no: No Autowiring. This is default value.
	2. ![[Pasted image 20250221195832.png]]
	3. 
3.
	1. byName: Informing to spf, please inject dependecy object which matches with bean id and property name of class.
	2. ![[Pasted image 20250221200319.png]]
	3.  byType: same datatype object
	4. ![[Pasted image 20250221201235.png]]
	5.
	1. if more than one bean id types are there.. then there will be ambigous effect and it does not work and throw an error. In case of this change the byType to another.(ex: byName).
4: byName and byType are done through setter injection.
5: constructor : in constructor autowire.. if there are multiple beans of same type.. then internally it follows **byName** .


	   
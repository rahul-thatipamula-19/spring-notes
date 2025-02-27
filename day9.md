The spring framework will create each object and pass the properties described in the xml file.
xml file configuration is not using in modern days.

The spring framework will call the setter methods when the values are passed as properties.
for map data types the values are passed as decribed in the image
![[Pasted image 20250220171409.png]]
injection of types can be of 4 into the objects.
![[Pasted image 20250220171556.png]]


->The class that going to be injected should be declared first, than the root class.
->ref attribute in xml is used to include the another class as injection. ref stands for object reference.

![[Pasted image 20250220172053.png]]


example:
![[Pasted image 20250220172433.png]]


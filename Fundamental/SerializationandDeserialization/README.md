## Serialization and Deserialization

Serialization is a mechanism of converting the state of an object into a byte stream.  
Deserialization is the reverse process where the byte stream is used to recreate the actual Java object in memory.   
This mechanism is used to persist the object.  

![](http://www.geeksforgeeks.org/wp-content/uploads/gq/2016/01/serialize-deserialize-java.png)  

To make a Java object serializable we implement the java.io.Serializable interface.  

**Advantages of Serialization**:  
1. To save/persist state of an object.  
2. To travel an object across a network.  

![](http://contribute.geeksforgeeks.org/wp-content/uploads/serialization-4.jpg)  
Serializable is a marker interface (has no data member and method). It is used to “mark” java classes so that objects of these classes may get certain capability. Other examples of marker interfaces are:- Cloneable and Remote.  

**REMEMBER**  
1. If a parent class has implemented Serializable interface then child class doesn’t need to implement it but vice-versa is not true.  
2. Only non-static data members are saved via Serialization process.  
3. Static data members and transient data members are not saved via Serialization process.So, if you don’t want to save value of a non-static data member then make it transient.  
4. Constructor of object is never called when an object is deserialized.  
5. Associated objects must be implementing Serializable interface.  


### Understand the serialVersionUID

The serialVersionUID is used as a version control in a Serializable class. If you do not explicitly declare a serialVersionUID, JVM will do it for you automatically, based on various aspects of your Serializable class, as described in the Java(TM) Object Serialization Specification.  






## Reference:
1. [serialization in java - geeksforgeeks](http://www.geeksforgeeks.org/serialization-in-java/)

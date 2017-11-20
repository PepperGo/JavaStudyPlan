## Serialization and Deserialization

Serialization is a mechanism of converting the state of an object into a byte stream.  
Deserialization is the reverse process where the byte stream is used to recreate the actual Java object in memory.   
This mechanism is used to persist the object.  

![](http://www.geeksforgeeks.org/wp-content/uploads/gq/2016/01/serialize-deserialize-java.png)  

To make a Java object serializable we implement the java.io.Serializable interface.  

**Advantages of Serialization**:  
1. To save/persist state of an object.  
2. To travel an object across a network.  



## Understand the serialVersionUID

The serialVersionUID is used as a version control in a Serializable class. If you do not explicitly declare a serialVersionUID, JVM will do it for you automatically, based on various aspects of your Serializable class, as described in the Java(TM) Object Serialization Specification.  


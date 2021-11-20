# Java Collections Framework Questions


## 1- What is the Collection framework in Java?
Collection Framework is a combination of classes and interface, which is used to store and manipulate the data in the form of objects. It provides various classes such as ArrayList, Vector, Stack, and HashSet, etc. and interfaces such as List, Queue, Set, etc. for this purpose.

## 2- What are the main differences between array and collection?
Array and Collection are somewhat similar regarding storing the references of objects and manipulating the data, but they differ in many ways. The main differences between the array and Collection are defined below:

- Arrays are always of fixed size, i.e., a user can not increase or decrease the length of the array according to their requirement or at runtime, but In Collection, size can be changed dynamically as per need.
- Arrays can only store homogeneous or similar type objects, but in Collection, heterogeneous objects can be stored.
- Arrays cannot provide the ?ready-made? methods for user requirements as sorting, searching, etc. but Collection includes readymade methods to use.

## 3- Explain various interfaces used in Collection framework?
Collection framework implements various interfaces, Collection interface and Map interface (java.util.Map) are the mainly used interfaces of Java Collection Framework. List of interfaces of Collection Framework is given below:

**1. Collection interface:** Collection (java.util.Collection) is the primary interface, and every collection must implement this interface.

**Syntax:**
```
public interface Collection<E>extends Iterable  
Where <E> represents that this interface is of Generic type
```
**2. List interface:** List interface extends the Collection interface, and it is an ordered collection of objects. It contains duplicate elements. It also allows random access of elements.

**Syntax:**
```
public interface List<E> extends Collection<E>
```  
**3. Set interface:** Set (java.util.Set) interface is a collection which cannot contain duplicate elements. It can only include inherited methods of Collection interface

**Syntax:**
```
public interface Set<E> extends Collection<E>
```  
Queue interface: Queue (java.util.Queue) interface defines queue data structure, which stores the elements in the form FIFO (first in first out).

**Syntax:**
```
public interface Queue<E> extends Collection<E> 
```
**4. Dequeue interface:** it is a double-ended-queue. It allows the insertion and removal of elements from both ends. It implants the properties of both Stack and queue so it can perform LIFO (Last in first out) stack and FIFO (first in first out) queue, operations.

**Syntax:**
```
public interface Dequeue<E> extends Queue<E>
```  
**5. Map interface:** A Map (java.util.Map) represents a key, value pair storage of elements. Map interface does not implement the Collection interface. It can only contain a unique key but can have duplicate elements. There are two interfaces which implement Map in java that are Map interface and Sorted Map.

## 4) What is the difference between ArrayList and Vector?
| ArrayList  |  Vector  |
| ------------------- | ------------------- |
|  ArrayList is not synchronized.	|  Vector is synchronized. |
|  ArrayList is not a legacy class.	|  Vector is a legacy class. |
|  ArrayList increases its size by 50% of the array size.	|  Vector increases its size by doubling the array size. |
|  ArrayList is not ?thread-safe? as it is not synchronized.	|  Vector list is ?thread-safe? as it?s every method is synchronized. |

## 5- What is the difference between ArrayList and LinkedList?
| ArrayList  |  LinkedList |
| ------------------- | ------------------- |
| ArrayList uses a dynamic array. | LinkedList uses a doubly linked list. |
| ArrayList is not efficient for manipulation because too much is required.	 | LinkedList is efficient for manipulation. |
| ArrayList is better to store and fetch data. | LinkedList is better to manipulate data. |
| ArrayList provides random access.	| LinkedList does not provide random access. |
| ArrayList takes less memory overhead as it stores only object	| LinkedList takes more memory overhead, as it stores the object as well as the address of that object. |

## 6- What is the difference between Iterator and ListIterator?
Iterator traverses the elements in the forward direction only whereas ListIterator traverses the elements into forward and backward direction.
| Iterator  |  ListIterator |
| ------------------- | ------------------- |
| The Iterator traverses the elements in the forward direction only. | ListIterator traverses the elements in backward and forward directions both. |
| The Iterator can be used in List, Set, and Queue. | ListIterator can be used in List only. |
| The Iterator can only perform remove operation while traversing the collection. | ListIterator can perform ?add,? ?remove,? and ?set? operation while traversing the collection. |

## 7- What is the difference between Iterator and Enumeration?
| Iterator  |  Enumeration |
| ------------------- | ------------------- |
| The Iterator can traverse legacy and non-legacy elements. | Enumeration can traverse only legacy elements. |
| The Iterator is fail-fast. | Enumeration is not fail-fast. |
| The Iterator is slower than Enumeration. | Enumeration is faster than Iterator. |
| The Iterator can perform remove operation while traversing the collection. | The Enumeration can perform only traverse operation on the collection. |

## 8- What is the difference between List and Set?
The List and Set both extend the collection interface. However, there are some differences between the both which are listed below.

- The List can contain duplicate elements whereas Set includes unique items.
- The List is an ordered collection which maintains the insertion order whereas Set is an unordered collection which does not preserve the insertion order.
- The List interface contains a single legacy class which is Vector class whereas Set interface does not have any legacy class.
- The List interface can allow n number of null values whereas Set interface only allows a single null value.

## 9- What is the difference between HashSet and TreeSet?
The HashSet and TreeSet, both classes, implement Set interface. The differences between the both are listed below.

- HashSet maintains no order whereas TreeSet maintains ascending order.
- HashSet impended by hash table whereas TreeSet implemented by a Tree structure.
- HashSet performs faster than TreeSet.
- HashSet is backed by HashMap whereas TreeSet is backed by TreeMap.

## 10- What is the difference between Set and Map?
The differences between the Set and Map are given below.

- Set contains values only whereas Map contains key and values both.
- Set contains unique values whereas Map can contain unique Keys with duplicate values.
- Set holds a single number of null value whereas Map can include a single null key with n number of null values.

## 11- What is the difference between HashSet and HashMap?
The differences between the HashSet and HashMap are listed below.

- HashSet contains only values whereas HashMap includes the entry (key, value). HashSet can be iterated, but HashMap needs to convert into Set to be iterated.
- HashSet implements Set interface whereas HashMap implements the Map interface
- HashSet cannot have any duplicate value whereas HashMap can contain duplicate values with unique keys.
- HashSet contains the only single number of null value whereas HashMap can hold a single null key with n number of null values.

## 12- What is the difference between HashMap and TreeMap?
The differences between the HashMap and TreeMap are given below.

- HashMap maintains no order, but TreeMap maintains ascending order.
- HashMap is implemented by hash table whereas TreeMap is implemented by a Tree structure.
- HashMap can be sorted by Key or value whereas TreeMap can be sorted by Key.
- HashMap may contain a null key with multiple null values whereas TreeMap cannot hold a null key but can have multiple null values.

## 13- What is the difference between HashMap and Hashtable?
| HashMap  |  Hashtable |
| ------------------- | ------------------- |
| HashMap is not synchronized.	| Hashtable is synchronized. |
| HashMap can contain one null key and multiple null values. | Hashtable cannot contain any null key or null value. |
| HashMap is not ?thread-safe,? so it is useful for non-threaded applications. | Hashtable is thread-safe, and it can be shared between various threads. |
| HashMap inherits the AbstractMap class | Hashtable inherits the Dictionary class. |

## 14- What is the difference between Collection and Collections?
The differences between the Collection and Collections are given below.

- The Collection is an interface whereas Collections is a class.
- The Collection interface provides the standard functionality of data structure to List, Set, and Queue. However, Collections class is to sort and synchronize the collection elements.
- The Collection interface provides the methods that can be used for data structure whereas Collections class provides the static methods which can be used for various operation on a collection.

## 15- What is the difference between Comparable and Comparator?
| Comparable  |  Comparator |
| ------------------- | ------------------- |
| Comparable provides only one sort of sequence. | The Comparator provides multiple sorts of sequences. |
| It provides one method named compareTo().	| It provides one method named compare(). |
| It is found in java.lang package.	| It is located in java.util package. |
| If we implement the Comparable interface, The actual class is modified.	| The actual class is not changed. |

## 16- What do you understand by BlockingQueue?
BlockingQueue is an interface which extends the Queue interface. It provides concurrency in the operations like retrieval, insertion, deletion. While retrieval of any element, it waits for the queue to be non-empty. While storing the elements, it waits for the available space. BlockingQueue cannot contain null elements, and implementation of BlockingQueue is thread-safe.

**Syntax:**
```
public interface BlockingQueue<E> extends Queue <E>
```

## 17- What is the advantage of Properties file?
If you change the value in the properties file, you don't need to recompile the java class. So, it makes the application easy to manage. It is used to store information which is to be changed frequently. Consider the following example.

```
import java.util.*;  
import java.io.*;  
public class Test {  
public static void main(String[] args)throws Exception{  
    FileReader reader=new FileReader("db.properties");  
      
    Properties p=new Properties();  
    p.load(reader);  
      
    System.out.println(p.getProperty("user"));  
    System.out.println(p.getProperty("password"));  
}  
}
```

**Output:**

```
system
oracle
```

## 18- What does the hashCode() method?
The hashCode() method returns a hash code value (an integer number).

The hashCode() method returns the same integer number if two keys (by calling equals() method) are identical.

However, it is possible that two hash code numbers can have different or the same keys.

If two objects do not produce an equal result by using the equals() method, then the hashcode() method will provide the different integer result for both the objects.

## 19- Why we override equals() method?
The equals method is used to check whether two objects are the same or not. It needs to be overridden if we want to check the objects based on the property.

For example, Employee is a class that has 3 data members: id, name, and salary. However, we want to check the equality of employee object by the salary. Then, we need to override the equals() method.

## 20- How to synchronize List, Set and Map elements?
Yes, Collections class provides methods to make List, Set or Map elements as synchronized:

|  `public static List synchronizedList(List l){}` | 
| ------------------- |
|  `public static Set synchronizedSet(Set s){}` |
|  `public static SortedSet synchronizedSortedSet(SortedSet s){}` |
|  `public static Map synchronizedMap(Map m){}` |
|  `public static SortedMap synchronizedSortedMap(SortedMap m){}` |





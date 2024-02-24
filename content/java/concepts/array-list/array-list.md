---
Title: 'ArrayList'
Description: 'The ArrayList class uses dynamic arrays for storing elements. Conceptually, it is like an array but with no size limit.'
Subjects:
  - 'Code Foundations'
  - 'Computer Science'
Tags:
  - 'Arrays'
  - 'Classes'
  - 'Data Structures'
CatalogContent:
  - 'learn-java'
  - 'paths/computer-science'
---

The `ArrayList` class uses dynamic arrays that are resizable, unlike traditional fixed [arrays](https://www.codecademy.com/resources/docs/java/arrays). However, each element must still be of the same type. Elements can be added or removed at any time, making the `ArrayList` more flexible.

Some other important points about the `ArrayList` class include:

- It has the ability to contain duplicate elements.
- It maintains insertion order.
- It is non-synchronized and, therefore, not safe for multiple threading.
- It allows random access since arrays work on an index basis.
- The space/time complexity is a bit slower than a LinkedList due to the nature of adding/removing elements.

## Syntax

To use the ArrayList class, you need to import it from the java.util package:

```java
import java.util.ArrayList;
```

To define an instance of ArrayList, you can use the following syntax, replacing DataType with the desired data type:

```pseudo
ArrayList<DataType> arrayListInstance = new ArrayList<DataType>();
```

## Example

Here's an example that demonstrates the usage of ArrayList. In this example, we create a new ArrayList instance called arr and perform various operations on it, including adding and removing elements:

```java
// Import from the java.util package
import java.util.ArrayList;

public class Example {
  public static void main(String []args) {
    ArrayList<String> arr = new ArrayList<>();

    System.out.println(arr);  // Currently empty

    arr.add("hello");
    arr.add("India");

    System.out.println(arr);

    arr.remove("hello");

    System.out.println(arr.size());  // Prints size of ArrayList

    arr.clear();

    System.out.println(arr); // Empty again
  }
}
```

The output of this example would be:

```shell
[]
[hello, India]
1
[]
```

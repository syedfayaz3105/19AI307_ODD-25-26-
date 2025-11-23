# Ex.No:2(B) METHODS

## QUESTION:
Write a class with one static method and one non-static method. Call both from the main() method. When staticMethod() is called, it should print "I am static". When nonStaticMethod() is called, it should print "I am non-static".

#### Example:
```
Result:
I am static
I am non-static
```



## AIM:

To understand how to define and use static and non-static methods in Java and call them from the main method.


## ALGORITHM :
*	Start the program.
*	Create a class containing:
   -> one static method
   -> one non-static method
* Static method prints: "I am static".
* Non-static method prints: "I am non-static".
* Call the static method directly from main().
* Create an object to call the non-static method.
* End the program.	





## PROGRAM:
 ```
Program to implement a Methods using Java
Developed by: Farhana H
RegisterNumber: 212223230057
```

## SOURCE CODE:
```
public class Test {
    static void staticMethod() {
        System.out.println("I am static");
    }

    void nonStaticMethod() {
        System.out.println("I am non-static");
    }

    public static void main(String[] args) {
        staticMethod();
        Test obj = new Test();
        obj.nonStaticMethod();
    }
}




```


## OUTPUT:
<img width="1181" height="340" alt="image" src="https://github.com/user-attachments/assets/94449343-3486-4baf-9e35-d12bce8149b3" />



## RESULT:
Thus, the Java program demonstrating static and non-static methods was executed successfully.


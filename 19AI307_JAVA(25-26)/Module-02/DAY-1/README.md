# Ex.No:2(A) CLASS AND OBJECT

## QUESTION:
Create a class Vehicle with attributes as number, type and owner.


## AIM:
To Create a class Vehicle with attributes as number, type and owner.

## ALGORITHM :
* Start the program.
* Import the necessary package 'java.util'
* Import the package java.util.Scanner to read user input.
* Create a class Vehicle with data members: (number, type, owner).
* In the main() method, create a Scanner object.
* Create two objects of the Vehicle class.
* Read the details (number, type, owner) for both objects from user input.
* Display the details of both vehicles.




## PROGRAM:
 ```
Program to implement a Class and Objects using Java
Developed by: Farhana H
RegisterNumber: 212223230057

```

## SOURCE CODE:

```
import java.util.Scanner;
class Vehicle
{
    String number;
    String type;
    String owner;
}
public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        Vehicle v1 = new Vehicle();
        v1.number = sc.next();
        v1.type = sc.next();
        v1.owner = sc.next();

        Vehicle v2 = new Vehicle();
        v2.number = sc.next();
        v2.type = sc.next();
        v2.owner = sc.next();

        System.out.println(v1.number + " | " + v1.type + " | " + v1.owner);
        System.out.println(v2.number + " | " + v2.type + " | " + v2.owner);
    }
}



```





## OUTPUT:
<img width="900" height="270" alt="image" src="https://github.com/user-attachments/assets/8961b564-8cae-466a-97ac-b178bb664893" />



## RESULT:
Thus, a Java program to create a class Vehicle with attributes number, type, and owner was successfully implemented and executed.



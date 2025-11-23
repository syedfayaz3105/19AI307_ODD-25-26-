# Ex.No:2(E) ACCESS MODIFIERS

## QUESTION:
Create a class Calculator with: One non-static method add(int a, int b) that returns the sum, One static method info() that says "Calculator is ready".

## AIM:
To write a Java program that defines a class Calculator with one non-static method for addition and one static method for displaying information.

## ALGORITHM :
* Create a class named Calculator.
* Define a non-static method add(int a, int b) that returns the sum.
* Define a static method info() that prints "Calculator is ready".
* In main(), call the static method directly and the non-static method using an object.
* Display the result.

## PROGRAM:
 ```
Program to implement a Access Modifiers using Java
Developed by:  Farhana H
RegisterNumber:  212223230057
```

## SOURCE CODE:
```
import java.util.Scanner;

class Calculator {

    int add(int a, int b) {
        return a + b;
    }

    static void info() {
        System.out.println("Calculator is ready");
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int num1 = sc.nextInt();
        int num2 = sc.nextInt();

        Calculator.info();

        Calculator calc = new Calculator();
        int sum = calc.add(num1, num2);

        System.out.println("Sum: " + sum);

    }
}


```

## OUTPUT:
<img width="1242" height="363" alt="image" src="https://github.com/user-attachments/assets/92958cc7-d0b9-4f25-8d8d-89a6f868dd06" />


## RESULT:
The program successfully demonstrates the use of static and non-static methods in a class.



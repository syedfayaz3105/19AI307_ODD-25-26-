# Ex.No:3(b) POLYMORPHISM

## QUESTION:
Write a Java program using method overriding. Create a superclass Bank with a method getInterestRate() returning 0. Create subclasses SBI, ICICI, and HDFC that override the method.


## AIM:
To write a Java program demonstrating runtime polymorphism using method overriding, where subclasses override a method of the superclass to provide specific implementation.


## ALGORITHM :
* Start the program.
* Import the necessary package 'java.util'
* Create a superclass Bank with a method getInterestRate() returning 0.
* Create subclasses SBI, ICICI, and HDFC that override the method to return different interest rates.
* In the main() method, accept bank name at runtime.
* Create an object of the appropriate subclass based on the input.
* Call the overridden method using a reference of type Bank.
* Display the interest rate.
* End the program.




## PROGRAM:
 ```
Program to implement a Polymorphism using Java
Developed by: Farhana H
RegisterNumber: 212223230057
```

## SOURCE CODE:
```
import java.util.*;
class Bank {
    double getInterestRate() {
        return 0;
    }
}

class SBI extends Bank {
    @Override
    double getInterestRate() {
        return 6.5;
    }
}

class ICICI extends Bank {
    @Override
    double getInterestRate() {
        return 7.0;
    }
}

class HDFC extends Bank {
    @Override
    double getInterestRate() {
        return 7.5;
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String bankName = sc.nextLine().trim();
        Bank bank;
        if (bankName.equalsIgnoreCase("SBI")) {
            bank = new SBI();
            System.out.println("SBI Rate: " + bank.getInterestRate() + "%");
        } else if (bankName.equalsIgnoreCase("ICICI")) {
            bank = new ICICI();
            System.out.println("ICICI Rate: " + bank.getInterestRate() + "%");
        } else if (bankName.equalsIgnoreCase("HDFC")) {
            bank = new HDFC();
            System.out.println("HDFC Rate: " + bank.getInterestRate() + "%");
        } else {
            System.out.println("Invalid bank name.");
        }
    }
}

```


## OUTPUT:
<img width="505" height="256" alt="image" src="https://github.com/user-attachments/assets/283a1f31-7896-48d6-bf0e-40f6abfcbb8a" />

## RESULT:
Thus, the Java program demonstrating Polymorphism using Method Overriding was successfully executed.
Thus, the Java program demonstrating Polymorphism using Method Overriding was successfully executed.


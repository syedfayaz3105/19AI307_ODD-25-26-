# Ex.No:1(E) STRINGS AND MATH FUNCTION

## QUESTION:
Write a Java program to reverse a given string.

## AIM:
To write a Java program that accepts a string from the user and prints the reversed string.

## ALGORITHM :
* Start the program.
* Import the package java.util.Scanner.
* Create a Scanner object to read input from the user.
* Read the input string.
* Initialize an empty string variable rev to store the reversed string.
* Use a loop to traverse the string from the last character to the first:
* Append each character to rev.
* After the loop ends, display the reversed string.
* End the program.

## PROGRAM:
 ```
Program to implement a Strings and Math Function using Java
Developed by: Farhana H
RegisterNumber: 212223230057

```

## SOURCE CODE:
```
import java.util.Scanner;

public class ReverseString {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        String str = sc.nextLine();
        String rev = "";
        for (int i = str.length() - 1; i >= 0; i--) {
            rev = rev + str.charAt(i);
        }


        System.out.println("Reversed string: " + rev);

        sc.close();
    }
}



```

## OUTPUT:
<img width="1283" height="346" alt="image" src="https://github.com/user-attachments/assets/d7815bd2-0da3-4c09-80e2-5364fcac4cef" />



## RESULT:
Thus, the Java program to reverse a given string was executed successfully and the reversed output was obtained.



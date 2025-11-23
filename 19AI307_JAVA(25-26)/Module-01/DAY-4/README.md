# Ex.No:1(D) ARRAYS

## QUESTION:
Write a Java program to reverse an array


## AIM:
To write a Java program to reverse the elements of an array and display the reversed array.

## ALGORITHM :
* Start the program.
* Import the package java.util.Scanner.
* Create a Scanner object to read input from the user.
* Read the size of the array n.
* Create an integer array of size n.
* Read all n elements from the user and store them in the array.
* Use a loop to print the elements of the array in reverse order:
* Start from the last index and move towards the first index.
* Display the reversed array.
* End the program.


## PROGRAM:
 ```
/*
Program to implement a Array concept using Java
Developed by: Preethi J
RegisterNumber: 212223220080
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

public class ReverseArray {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        
        int n = sc.nextInt();
        int[] arr = new int[n];

        
        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }

        
        for (int i = n - 1; i >= 0; i--) {
            System.out.print(arr[i] + " ");
        }

        sc.close();
    }
}

```


## OUTPUT:
<img width="1280" height="633" alt="image" src="https://github.com/user-attachments/assets/d04f02a0-05f6-4125-bce2-948f71266ec2" />



## RESULT:
Thus, the Java program to reverse the elements of an array was executed successfully and the expected output was obtained.



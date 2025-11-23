# Ex.No:3(C) ABSTRACTION

## QUESTION:
A group of researchers receives mysterious numerical sequences believed to be sent by intelligent alien life. To decode them, scientists have built intelligent SignalAgents that follow abstract processing rules. Each agent listens to the numbers differently.


## AIM:
To implement Abstraction in Java by defining an abstract class with abstract methods and providing different implementations in derived subclasses.


## ALGORITHM :
* Start the program.
* Import the necessary package 'java.util'
* Create an abstract class SignalAgent with an abstract method processNumbers(int[]).
* Create subclasses SumAgent and AverageAgent that extend the base class and provide method implementations.
* Accept a numerical sequence from the user and store it in an array.
* Allow the user to select which type of agent to use for processing.
* Display the processed result.
* End the program.


## PROGRAM:
 ```
Program to implement a Abstraction using Java
Developed by: Farhana H
RegisterNumber: 212223230057
```

## SOURCE CODE:
```
import java.util.*;

abstract class SignalAgent {
    abstract int decodeSignal(int[] signal);
}

class PrimeAgent extends SignalAgent {
    boolean isPrime(int n) {
        if (n <= 1) return false;
        for (int i = 2; i * i <= n; i++) {
            if (n % i == 0)
                return false;
        }
        return true;
    }

    @Override
    int decodeSignal(int[] signal) {
        int sum = 0;
        for (int num : signal) {
            if (isPrime(num))
                sum += num;
        }
        return sum;
    }
}

class MirrorAgent extends SignalAgent {
    @Override
    int decodeSignal(int[] signal) {
        int n = signal.length;
        for (int i = 0; i < n / 2; i++) {
            if (signal[i] != signal[n - 1 - i]) {
             
                return -1;
            }
        }
        return 1;
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int[] signal = new int[n];
        for (int i = 0; i < n; i++)
            signal[i] = sc.nextInt();
        int type = sc.nextInt();
        
        SignalAgent agent;
        
        if (type == 1) {
            agent = new PrimeAgent();
            System.out.println(agent.decodeSignal(signal));
        } else if (type == 2) {
            agent = new MirrorAgent();
            int result = agent.decodeSignal(signal);
            if (result == 1)
                System.out.println("BALANCED");
            else
                System.out.println("BROKEN");
        }
    }
}


```

## OUTPUT:
<img width="409" height="296" alt="image" src="https://github.com/user-attachments/assets/6347d668-c686-4449-b258-180efe5582e4" />



## RESULT:
Thus, the Java program demonstrating Abstraction using an abstract class and derived classes was executed successfully.



no free flotaing function. that means everything is inside a class in java.. 

you dont manage pointers or maually free memory in java.

java code is compiled into bytecode .class which allows it to run anywhere and compiles in java virtual machine (JVM)


```
public class Main{
	public static void main(String[] args){
	System.out.println("Welcome to java");
	}
}
```

static : Runs without needing to instantiate an object of `Main` first.

always important to use 
```
import java.util.Scanner;

Scanner scanner = new Scanner(System.in);

long variable - scanner.nextLong();

```
this is used to take inputs in java



if statements work in similar fashion to c
```
If(){}
```

```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        long score = scanner.nextLong();
        System.out.println("Wendy's high score: " + score);
        scanner.close();
    }
}



import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        long a = scanner.nextLong();
        long b = scanner.nextLong();

// In Java, booleans must be converted to integers using arithmetic tricks with relational operators
        int aIsGreater = (a >= b) ? 1 : 0; 
        
        // Pure relational operator logic:
        long maxVal = a * (a >= b ? 1 : 0) + b * (b > a ? 1 : 0);

        System.out.println(maxVal);
        scanner.close();
    }
}

import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        String modelName = scanner.nextLine();
        int epochs = scanner.nextInt();
        int batchSize = scanner.nextInt();
        double learningRate = scanner.nextDouble();
        boolean isSuccessful = scanner.nextBoolean();

        System.out.println("Model Name: " + modelName);
        System.out.println("Training Epochs: " + epochs);
        System.out.println("Batch Size: " + batchSize);
        System.out.printf("Learning Rate: %.2f\n", learningRate);
        System.out.println("Training Successful: " + isSuccessful);

        scanner.close();
    }
}


```

## Impt while using Print

using "printf" u use " "", variable  "
ex :         System.out.printf("Learning Rate: %.2f\n", learningRate);

using println
System.out.println("Training Successful: " + isSuccessful);

import java.util.Scanner;

## using float double int in functions
```
// You are using Java-21version 
import java.util.Scanner;

public class Main{
    public static void main(String[] args){
        Scanner scanner = new Scanner(System.in);
        
        int principal = scanner.nextInt();
        float rate = scanner.nextFloat();
        int time = scanner.nextInt();
        
        float interest = (principal * rate * time) / 100.0f;
        float total = principal + interest;
        
        System.out.printf("Simple Interest: %.2f\n", interest);
        System.out.printf("Total Amount: %.2f\n", total);
        
        scanner.close();
    }
}
```

in interest line dividing with just 100.0 will not work cuz 100.0 is a double and not a float. hence f is used after 100.0 so that you can noramally divide


## IMPT in java ^ represents XOR


HARD LAB 1
```
q1
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        int input = scanner.nextInt();

        // Bitwise XOR with mask to toggle 2nd and 3rd bits
        // 2nd bit (bit index 1) = 2^1 = 2
        // 3rd bit (bit index 2) = 2^2 = 4
        // Mask = 2 + 4 = 6 (binary 110)
        int result = input ^ 6;

        System.out.println("Result: " + result);

        scanner.close();
    }
}
------------------------------------

q2

import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        int X = scanner.nextInt();
        int N = scanner.nextInt();

        // Create a mask with N ones: (1 << N) - 1
        int mask = (1 << N) - 1;

        // Perform bitwise AND to extract lowest N bits
        int result = X & mask;

        System.out.println("Result: " + result);

        scanner.close();
    }
}

```


---

## Using Switch
```
        char grade = scanner.next().charAt(0);
        String remark;

        switch (grade) {
            case 'A':
                remark = "Excellent";
                break;
            case 'B':
                remark = "Very Good";
                break;
            case 'C':
                remark = "Good";
                break;
            case 'D':
                remark = "Satisfactory";
                break;
            case 'F':
                remark = "Fail";
                break;
            default:
                remark = "Invalid Grade";
                break;
        }
```



import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        double electricityUnits = scanner.nextDouble();
        double waterUnits = scanner.nextDouble();
        double gasUnits = scanner.nextDouble();

        // Rates
        double electricityCost = electricityUnits * 0.12;
        double waterCost = waterUnits * 0.05;
        double gasCost = gasUnits * 0.08;

        double totalCost = electricityCost + waterCost + gasCost;

        // Apply discount rules
        double finalBill;
        if (totalCost >= 100.0) {
            finalBill = totalCost * 0.90; // 10% discount
        } else if (totalCost >= 50.0) {
            finalBill = totalCost * 0.95; // 5% discount
        } else {
            finalBill = totalCost;        // No discount
        }

        System.out.printf("%.2f\n", finalBill);

        scanner.close();
    }
}

import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        int grade = scanner.nextInt();
        char letterGrade;

        if (grade >= 90) {
            letterGrade = 'A';
        } else if (grade >= 80) {
            letterGrade = 'B';
        } else if (grade >= 70) {
            letterGrade = 'C';
        } else if (grade >= 60) {
            letterGrade = 'D';
        } else {
            letterGrade = 'F';
        }

        System.out.println("Letter Grade: " + letterGrade);

        scanner.close();
    }
}


import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        int N = scanner.nextInt();
        int temp = N;

        long oddDigitsNum = 0;   // Stores odd digits extracted right-to-left
        long reversedOdd = 0;    // Stores the reverse of oddDigitsNum

        // Extract odd digits right-to-left using a do-while loop
        do {
            int digit = temp % 10;
            if (digit % 2 != 0) {
                oddDigitsNum = oddDigitsNum * 10 + digit;
            }
            temp /= 10;
        } while (temp > 0);

        // Print the extracted odd digits (which are naturally in reverse order)
        System.out.println("Odd digits: " + oddDigitsNum);

        // Reverse oddDigitsNum using a do-while loop to verify palindrome
        long tempOdd = oddDigitsNum;
        do {
            int digit = (int)(tempOdd % 10);
            reversedOdd = reversedOdd * 10 + digit;
            tempOdd /= 10;
        } while (tempOdd > 0);

        // Palindrome check
        if (oddDigitsNum == reversedOdd) {
            System.out.println("The odd digits form a palindrome.");
        } else {
            System.out.println("The odd digits do not form a palindrome.");
        }

        scanner.close();
    }
}
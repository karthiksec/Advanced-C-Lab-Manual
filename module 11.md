```
NAME:KARTHIK G.
REG NO:212223220043
```
EXP NO:21 C PROGRAM TO CREATE A FUNCTION TO FIND THE GREATEST NUMBER
Aim:
To write a C program to create a function to find the greatest number

Algorithm:
1.	Include the necessary header #include <stdio.h>.
2.	Use a series of if and else if statements to compare the values and return the maximum among them.
3.	Declare variables n1, n2, n3, n4, and greater to store user input and the result.
4.	Use scanf to take four integers as input.
5.	Call the max_of_four function with the input integers and store the result in the greater variable
 
Program:
```
#include <stdio.h>

// Function to find greatest number in array
int findGreatest(int arr[], int n) {
    int max = arr[0];
    for (int i = 1; i < n; i++) {
        if (arr[i] > max) {
            max = arr[i];
        }
    }
    return max;
}

int main() {
    int n;
    printf("Enter how many numbers: ");
    scanf("%d", &n);

    int arr[n];
    printf("Enter %d numbers: ", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    int greatest = findGreatest(arr, n);
    printf("Greatest number = %d\n", greatest);

    return 0;
}
```

Output:
<img width="1915" height="826" alt="image" src="https://github.com/user-attachments/assets/3d8c6738-94ea-40e9-bf01-c7579cf6fd2b" />

Result:
Thus, the program  that create a function to find the greatest number is verified successfully.


 
EXP NO:22 C PROGRAM TO PRINT THE MAXIMUM VALUES FOR THE AND, OR AND  XOR COMPARISONS
Aim:
To write a C program to print the maximum values for the AND, OR and XOR comparisons

Algorithm:
1.	Define a function calculate_the_max that takes two integers n and k as parameters.
2.	Declare variables a, o, and x to store the maximum values for AND, OR, and XOR operations, respectively.
3.	Use nested loops to iterate through pairs of integers (i, j) from 1 to n.
4.	Within the loops, check conditions for AND, OR, and XOR operations and update the corresponding maximum values (a, o, x).
5.	Declare variables n and k to store user input.
6.	Use scanf to take two integers as input.
7.	Call the calculate_the_max function with input values.
 
Program:
```
#include <stdio.h>

int main() {
    int n;
    printf("Enter the value of n: ");
    scanf("%d", &n);

    int maxAND = 0, maxOR = 0, maxXOR = 0;

    for (int i = 1; i <= n; i++) {
        for (int j = i + 1; j <= n; j++) {
            if ((i & j) > maxAND) maxAND = i & j;
            if ((i | j) > maxOR)  maxOR  = i | j;
            if ((i ^ j) > maxXOR) maxXOR = i ^ j;
        }
    }

    printf("Maximum AND = %d\n", maxAND);
    printf("Maximum OR  = %d\n", maxOR);
    printf("Maximum XOR = %d\n", maxXOR);

    return 0;
}
```

Output:
<img width="1702" height="811" alt="image" src="https://github.com/user-attachments/assets/c5cc6929-18c2-44dd-90cd-d225c7d6822f" />

Result:
Thus, the program to print the maximum values for the AND, OR and XOR comparisons
is verified successfully.


 
EXP NO:23 C PROGRAM TO WRITE THE LOGIC FOR THE REQUESTS
Aim:
To write a C program to write the logic for the requests

Algorithm:
1.	Declare variables noshel and noque to store the number of shelves and the number of queries, respectively.
2.	Use scanf to take two integers as input for the number of shelves and queries.
3.	Declare a 2D array shelarr to represent shelves and books, and an array nobookarr to store the number of books on each shelf.
4.	Declare variables k and c to keep track of the book index and the total number of books.
5.	Use a for loop to iterate over the queries.
 
Program:
```
#include <stdio.h>

int main() {
    int n;
    printf("Enter the value of n: ");
    scanf("%d", &n);

    int maxAND = 0, maxOR = 0, maxXOR = 0;

    for (int i = 1; i <= n; i++) {
        for (int j = i + 1; j <= n; j++) {
            if ((i & j) > maxAND) maxAND = i & j;
            if ((i | j) > maxOR)  maxOR  = i | j;
            if ((i ^ j) > maxXOR) maxXOR = i ^ j;
        }
    }

    printf("Maximum AND = %d\n", maxAND);
    printf("Maximum OR  = %d\n", maxOR);
    printf("Maximum XOR = %d\n", maxXOR);

    return 0;
}
```

Output:
<img width="1751" height="863" alt="image" src="https://github.com/user-attachments/assets/75447491-e954-4cf6-8fd0-62f4031462fc" />

Result:
Thus, the program to write the logic for the requests is verified successfully.


 
EXP NO:24 C PROGRAM PRINT THE SUM OF THE INTEGERS IN THE ARRAY.
Aim:
To write a C program print the sum of the integers in the array.

Algorithm:
1.	Declare a variable n to store the number of integers.
2.	Use scanf to take an integer n as input.
3.	Declare an array a of size n to store the integers.
4.	Declare a variable sum and initialize it to zero.
5.	Use a for loop to iterate n times:
6.	Use scanf to input each integer and add it to the sum.
7.	Print the final sum using printf.



Program:
```
#include <stdio.h>

int main() {
    int n, i, sum = 0;
    printf("Enter number of elements: ");
    scanf("%d", &n);

    int arr[n];  // array declaration

    printf("Enter %d integers:\n", n);
    for (i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
        sum += arr[i];  // accumulate sum
    }

    printf("Sum of array elements = %d\n", sum);

    return 0;
}
```

Output:
<img width="1890" height="861" alt="image" src="https://github.com/user-attachments/assets/a6c6ac05-e455-4b6b-8fea-16f56d3ea981" />


Result:
Thus, the program prints the sum of the integers in the array is verified successfully.


 
EXP NO 25: C PROGRAM TO COUNT THE NUMBER OF WORDS IN A      SENTENCE



Aim:

To write a C program that counts the number of words in a given sentence.

Algorithm:

1.	Input the sentence: Take a sentence from the user.
2.	Initialize a counter variable: This will keep track of the number of words.
3.	Process each character of the sentence:
o	Iterate through the sentence, checking each character.
o	If a character is not a space, it may belong to a word. If it's the first non-space character after a space or at the start, increment the word count.
4.	Handle spaces and punctuation: Skip over spaces, punctuation marks, and consider each word as a sequence of characters separated by spaces.
5.	Display the result: After processing the sentence, output the total word count.



Program:
 ```
#include <stdio.h>
#include <string.h>
#include <ctype.h>

int main() {
    char str[200];
    int count = 0, i;

    printf("Enter a sentence: ");
    fgets(str, sizeof(str), stdin);  // read full line

    int len = strlen(str);

    for (i = 0; i < len; i++) {
        // Check if current char is not space and previous is space or start
        if ((i == 0 && !isspace(str[i])) || 
            (!isspace(str[i]) && isspace(str[i - 1]))) {
            count++;
        }
    }

    printf("Number of words = %d\n", count);

    return 0;
}
```

Output:
<img width="1836" height="862" alt="image" src="https://github.com/user-attachments/assets/0ca262e5-3251-4428-88e1-243d5a2d5e4d" />




Result:

Thus, the program that counts the number of words in a given sentence is verified 
successfully.

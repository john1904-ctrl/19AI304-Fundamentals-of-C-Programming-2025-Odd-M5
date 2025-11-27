EX-21-POINTERS
# AIM:
Write a C program to convert a 23.65 into 25 using pointer

## ALGORITHM:
1.	Declare a double variable to hold the floating-point number (23.65).
2.	Declare a pointer to double to point to the address of the variable.
3.	Use the pointer to modify the value to 25.0.
4.	Print the modified value.

## PROGRAM:

```
#include <stdio.h>

int main() {
    double num = 23.65;
    double *ptr = &num;
    *ptr = 25.0;
    printf("Modified value: %.2f\n", num);

    return 0;
}
```

## OUTPUT:
 	



![445978705-69d31b81-432a-456e-8b4b-cf4da277d9d6](https://github.com/user-attachments/assets/e2cdb3d2-58f9-4b38-a5b8-96eee72e3c11)


## RESULT:
Thus the program to convert a 23.65 into 25 using pointer has been executed successfully.

# EX-22-FUNCTIONS AND STORAGE CLASS

## AIM:

Write a C program to calculate the Product of first 12 natural numbers using Recursion

## ALGORITHM:

1.	Define a recursive function calculateProduct that takes an integer parameter n.
2.	Return n multiplied by the result of the calculateProduct function called with n - 1.
3.	Declare an integer variable n and an unsigned long long variable product.
4.	Initialize n with the value 12 (for the first 12 natural numbers).
5.	Call the calculateProduct function with n and store the result in the product variable.
6.	Print the result, indicating it is the product of the first 12 natural numbers.

## PROGRAM:

```
#include <stdio.h>

int product(int n)
{
    if (n == 1)
        return 1;
    else
        return n * product(n - 1);
}

int main()
{
    int n;
    scanf("%d", &n);

    if (n <= 0) {
        printf("Input must be a natural number\n");
        return 1;
    }

    int result = product(n);
    printf("Product is = %d\n", result);
    return 0;
}

```


## OUTPUT:


![445979231-2586a095-974f-4c49-b01c-bf78a0593201](https://github.com/user-attachments/assets/05acca35-47bd-4902-8729-2ff4f1b891bd)

Thus the program has been executed successfully.


# EX-23-ARRAYS AND ITS OPERATIONS

## AIM:

Write C Program to find Sum of each row of a Matrix

## ALGORITHM:

1.	Declare and initialize the matrix with the desired values.
2.	Create a loop to iterate through each row of the matrix.
3.	Inside the loop, calculate the sum of the elements in each row.
4.	Print the sum for each row.

## PROGRAM:

```
#include <stdio.h>

int main() {
    int rows, cols;
    scanf("%d %d", &rows, &cols);

    int matrix[rows][cols];
    for (int i = 0; i < rows; i++) {
        for (int j = 0; j < cols; j++) {
            scanf("%d", &matrix[i][j]);
        }
    }
    for (int i = 0; i < rows; i++) {
        int rowSum = 0;
        for (int j = 0; j < cols; j++) {
            rowSum += matrix[i][j];
        }
        printf("The Sum of Elements of a Rows in a Matrix:  %d\n", rowSum);
    }

    return 0;
}

```
## OUTPUT



![445979725-4cd464fa-8924-4071-a59d-a21373144c40](https://github.com/user-attachments/assets/8fddd62c-e98c-4041-a0ea-87befe27a525)

 
 

 ## RESULT

Write C Program to find Sum of each row of a Matrix


# EX -25 –DISPLAYING ARRAYS USING POINTERS
## AIM

Write a c program to read and display an array of any 6 integer elements using pointer

## ALGORITHM
Step 1: Start the program.
Step 2: Declare the following:
•	Integer variable i for iteration.
•	Integer variable n to store the number of elements.
•	Integer array arr[10] to hold up to 10 elements.
•	Integer pointer parr and initialize it to point to the array arr.
Step 3: Read the value of n (number of elements) from the user.
Step 4: Loop from i = 0 to i < n:
•	Read an integer value and store it in the address parr + i using pointer arithmetic.
Step 5: Loop from i = 0 to i < n:
•	Print the element at *(parr + i) using pointer dereferencing.
Step 6: End the program.

## PROGRAM


```
#include <stdio.h>

int main() {
    int arr[10], i, n;
    int *parr;

    // Step 3: Set number of elements to 6
    n = 6;

    // Step 2: Initialize pointer to point to array
    parr = arr;

    // Step 4: Read elements using pointer
    printf("Enter %d integer elements:\n", n);
    for (i = 0; i < n; i++) {
        scanf("%d", (parr + i));
    }

    // Step 5: Display elements using pointer
    printf("The array elements are:\n");
    for (i = 0; i < n; i++) {
        printf("%d ", *(parr + i));
    }
```

## OUTPUT


![445981700-dd9740a2-562b-4940-a9ae-f470667f4d1f](https://github.com/user-attachments/assets/4ea9c8e2-31c3-42a4-9308-75a05429f29e)

 

## RESULT


Thus the C program to read and display an array of any 6 integer elements using pointer has been executed




## RESULT:
Thus the program to convert a 23.65 into 25 using pointer has been executed successfully.

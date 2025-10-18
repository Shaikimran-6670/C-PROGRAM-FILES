## 1.program in C to store elements in an array and print them.
```c
#include<stdio.h>

int main()
{
        int arr[10];
        int n,i;

        printf("enter the number of the elements:");
        scanf("%d",&n);

        printf("enter %d elements:",n);

        for(i=0;i<n;i++) {

                scanf("%d",&arr[i]);
        }

        printf("the elements of the array are:\n");

        for(i=0;i<n;i++) {
                printf("%d\n",arr[i]);
        }

        return 0;
}
```
## 2.program in C to read n number of values in an array and display them in reverse order.
```c
include<stdio.h>

int main()
{
        int arr[100];
        int n,i;

        printf("enter the number of the elements:");
        scanf("%d",&n);

        printf("enter %d elements:",n);

        for(i=0;i<n;i++) {

                scanf("%d",&arr[i]);
        }

        printf("after reversing numbers:\n");

        for(i=n-1;i>=0;i--) {

                printf("%d\n",arr[i]);
        }

        return 0;
}
```
## 3. Write a program in C to find the sum of all elements of the array.
```c
#include<stdio.h>

int main()
{
        int arr[100];
        int i,n,sum=0;

        printf("enetr the number of the elements:");
        scanf("%d",&n);

        printf("enter %d elements:\n",n);

        for(i=0;i<n;i++) {
                scanf("%d",&arr[i]);
        }

        printf("sum of the all elements is:");

        for(i=0;i<n;i++) {

                sum = sum+arr[i];
        }
        printf("%d\n",sum);

        return 0;
}
```
## 4. program in C to copy the elements of one array into another array.
```c

5. Write a program in C to count the total number of duplicate elements in an array.
6. Write a program in C to print all unique elements in an array.
7. Write a program in C to merge two arrays of the same size sorted in descending order.
8. Write a program in C to count the frequency of each element of an array.
9. Write a program in C to find the maximum and minimum elements in an array
10. Write a program in C to separate odd and even integers into separate arrays.
11. Write a program in C to sort elements of an array in ascending order
12. Write a program in C to sort the elements of the array in descending order
13. Write a program in C to delete an element at a desired position from an array.
14. Write a program in C to find the second largest element in an array
15. Write a program in C to find the second smallest element in an array.
16. Write a program in C for a 2D array of size 3x3 and print the matrix.
17. Write a program in C for adding two matrices of the same size.
18. Write a program in C for the subtraction of two matrices.
19. Write a program in C for the multiplication of two square matrices.
20. Write a program in C to find the transpose of a given matrix.
21. Write a program in C to find the sum of the right diagonals of a matrix.
22. Write a program in C to find the sum of the left diagonals of a matrix.
23. Write a program in C to find the sum of rows and columns of a matrix.
24. Write a program in C to print or display the lower triangular of a given matrix.
25. Write a program in C to print or display an upper triangular matrix.
26. Write a program in C to calculate the determinant of a 3 x 3 matrix

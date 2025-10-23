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
nclude<stdio.h>

int main()
{
        int a[100],b[100];
        int i,n;

        printf("enter the number of elements:");
        scanf("%d",&n);

        printf("enter %d elements:\n",n);

        for(i=0;i<n;i++) {
                scanf("%d",&a[i]);
        }

        printf("-----after copying elements-----\n");

        for(i=0;i<n;i++) {

                b[i] = a[i];

                printf("%d\t",b[i]);
        }

        return 0;
}

```

## 5.Program in C to count the total number of duplicate elements in an array.
```c
include<stdio.h>

int main()
{
        int arr[100],visit[100]={0};

        int i,j,count=0,n;

        printf("enter the number of the elements:");
        scanf("%d",&n);

        printf("enter %d elements:",n);

        for(i=0;i<n;i++) {
                scanf("%d",&arr[i]);
                for(j=0;j<n;j++) {
                        }
        }

        for(i=0;i<n;i++) {
                if(visit[i]==0) {
                        for(j=i+1;j<n;j++) {
                                if(arr[i]==arr[j]) {

                                        count++;

                                        visit[j]=1;

                                }
                        }

                }
        }
          printf("\n Number of Duplicates are=%d\n",count);

        return 0;
}
```
## 6. Program in C to print all unique elements in an array.
```c
#include<stdio.h>

int main()
{
        int arr[100];
        int i,j,n,count;

        printf("enter the number of the elements:");
        scanf("%d",&n);

        printf("enter %d elemnets:",n);

        for(i=0;i<n;i++) {
                 scanf("%d",&arr[i]);
                for(j=0;j<n;j++) {

                }
        }

        printf("-----the unique elements are-----\n");

        for(i=0;i<n;i++) {

                count=0;

                for(j=0;j<n;j++) {

                        if(arr[i] == arr[j] && i!=j)

                        count++;

                }
                if(count ==0)
        printf("%d\n",arr[i]);

           }

        return 0;
        }
```
## 7. Program in C to merge two arrays of the same size sorted in descending order.
```c
#include<stdio.h>

int main()
{
        int a[100],b[100],merge[200];

        int i,j,n,temp;

        printf("enter the size of each array elements:");
        scanf("%d",&n);

        printf("enter %d elements of first array:",n);
        for(i=0;i<n;i++) {
                scanf("%d",&a[i]);
        }

        printf("enter %d elements of second array:",n);
        for(i=0;i<n;i++) {
                scanf("%d",&b[i]);
        }

        for(i=0;i<n;i++) {
                merge[i] = a[i];
        }
        for(i=0;i<n;i++) {
                merge[n+i] = b[i];
        }

        for(i=0;i<2*n-1;i++) {
                for(j=i+1;j<2*n;j++) {
                        if(merge[i] < merge[j]) {

                                temp = merge[i];
                                merge[i] = merge[j];
                                merge[j] = temp;
                        }
                }
        }
        printf("Descending order after merging\n");
        for(i=0;i<2*n;i++) {
                printf("%d\n",merge[i]);
        }
        return 0;
}
```
## 8.Program in C to count the frequency of each element of an array.
```c
#include<stdio.h>

int main()
{
        int arr[100],visited[100]={0};
        int i,j,n,count;

        printf("enter the size of an array:");
        scanf("%d",&n);

        printf("enter the %d elements:",n);

        for(i=0;i<n;i++) {
                scanf("%d",&arr[i]);
        }

        for(i=0;i<n;i++) {

                if(visited[i]==1)

                continue;

                        count=1;

                for(j=i+1;j<n;j++) {
                        if(arr[i] == arr[j]) {

                                 count++;

                                 visited[j]=1;
                        }
                }


                printf("%d->%d\n",arr[i],count);
        }
                return 0;
        }
```
## 9.Program in C to find the maximum and minimum elements in an array.
```c
#include<stdio.h>

int main()
{
        int arr[100];
        int max,min,i,j,n;

        printf("enter the size of the array:");
        scanf("%d",&n);

        printf("enter the %d elements:",n);

        for(i=0;i<n;i++) {
                scanf("%d",&arr[i]);
        }

         max=arr[0];
         min=arr[0];

        for(i=1;i<n;i++) {

                if(arr[i] > max) {

                         max=arr[i];

                }if(arr[i] < min){

                         min =arr[i];

                }
        }

        printf("maximum=%d\n",max);
        printf("minmum=%d\n",min);

        return 0;
}
```
## 10.Program in C to separate odd and even integers into separate arrays.
```c
#include<stdio.h>

int main()
{
        int arr[100],even[100],odd[100];
        int i,j,n,evencount,oddcount;

        printf("enter the size of the array elements:");
        scanf("%d",&n);

        printf("enter the %d elements:",n);

        for(i=0;i<n;i++) {
                scanf("%d",&arr[i]);
        }

        for(i=0;i<n;i++) {
                if(arr[i]%2==0) {

                   even[evencount]=arr[i];

                   evencount++;
                }
                else{
                        odd[oddcount]=arr[i];

                        oddcount++;
                }
        }

                printf("even numbers are:");

                for(i=0;i<evencount;i++) {

                        printf("\n%d",even[i]);
                }

                printf("\nodd numbers are:");

                for(i=0;i<oddcount;i++) {

                        printf("\n%d",odd[i]);
                }

        return 0;
}
```
## 11.Program in C to sort elements of an array in ascending order.
```c
#include<stdio.h>

int main()
{
        int arr[100];
        int i,j,temp,n;

        printf("enter the size of array elements:");
        scanf("%d",&n);

        printf("enter the %d elements:",n);

        for(i=0;i<n;i++) {
                scanf("%d",&arr[i]);
        }

        for(i=0;i<n-1;i++) {
                for(j=i+1;j<n;j++) {

                        if(arr[i] > arr[j]) {

                                temp = arr[i];
                                arr[i] = arr[j];
                                arr[j] = temp;
                        }
                }
        }

        printf("-----Ascending order is-----");

        for(i=0;i<n;i++) {
                printf(" %d  ",arr[i]);
        }
        printf("\n");
        return 0;
}
```
## 12.Program in C to sort the elements of the array in descending order.
```c
#include<stdio.h>

int main()
{
        int arr[100];
        int i,j,n,temp;

        printf("enter the size of the array elements:");
        scanf("%d",&n);

        printf("enter %d elements:",n);

        for(i=0;i<n;i++) {

                scanf("%d",&arr[i]);
        }

        for(i=0;i<n-1;i++) {

                for(j=i+1;j<n;j++) {

                        if(arr[i] < arr[j]) {

                                temp = arr[i];
                                arr[i] = arr[j];
                                arr[j] =temp;
                        }
                }
        }

        printf("-----Descending order is-----");

        for(i=0;i<n;i++) {

                printf(" %d  ",arr[i]);
        }
        printf("\n");
        return 0;
}
```
## 13.Program in C to delete an element at a desired position from an array.
```c
#include<stdio.h>

int main()
{
        int arr[100];
        int i,j,n,pos,num;

        printf("enter the size of the array element:");
        scanf("%d",&n);

        printf("enter the %d elements:",n);

        for(i=0;i<n;i++) {
                scanf("%d",&arr[i]);
        }

        printf("enter the deleting position from 1 to %d:",n);
        scanf("%d",&pos);

        if(pos < 1 || pos > n) {

                printf("invalid position");
        }else {

        for(i=pos-1;i<n-1;i++) {

                arr[i] = arr[i+1];

        }
                n--;

        printf("-----After deletion-----\n");

        for(i=0;i<n;i++) {
                printf("%d ",arr[i]);
        }
        }
        printf("\n");

        return 0;
}
```
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

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
## 14.Program in C to find the second largest element in an array.
```c
#include<stdio.h>

int main()
{
        int arr[100],second,big;

        int i,n;

        printf("enter the size of the array elements:");
        scanf("%d",&n);

        printf("enter the %d elements:",n);

        for(i=0;i<n;i++) {

                scanf("%d",&arr[i]);
        }

        big=0;
        second=0;

        for(i=0;i<n;i++) {

          if(arr[i] > big) {

                second = big;

                big = arr[i];

        }else if(arr[i] > second) {

                 second = arr[i];
        }
        }

        printf("The second largest number is:%d\n",second);

        return 0;
}
```
## 15.Program in C to find the second smallest element in an array.
```c
#include<stdio.h>

int main()
{
        int arr[100],small,second;

        int i,n;

        printf("enter the size of the array elements:");
        scanf("%d",&n);

        printf("enter %d elements:",n);

        for(i=0;i<n;i++) {
                scanf("%d",&arr[i]);
        }

        if(arr[0] < arr[1]) {

                small=arr[0];
                second=arr[1];
        }else {
                small=arr[1];
                second=arr[0];
        }
        for(i=2;i<n;i++) {

                if(arr[i] < small) {

                        second = small;
                        small = arr[i];
                } else if(arr[i] < second && arr[i] > small) {

                        second = arr[i];
                }
        }
        printf("The second smallest number is:%d\n",second);
        return 0;
}
```
## 16.Program in C for a 2D array of size 3x3 and print the matrix.
```c
#include<stdio.h>

int main()
{
        int arr[3][3];
        int i,j;

        printf("Enter the 3x3 matrix elements\n");

        for(i=0;i<3;i++) {
                for(j=0;j<3;j++) {

                        printf("Enter the number at position [%d][%d]:",i,j);

                        scanf("%d",&arr[i][j]);
                }
        }

        printf("The 3x3 matrix is:\n");

        for(i=0;i<3;i++) {
                for(j=0;j<3;j++) {

                        printf("%d\t",arr[i][j]);
                }

        printf("\n");
      }

        return 0;
}
```
## 17.Program in C for adding two matrices of the same size.
```c
#include<stdio.h>

int main()
{
        int a[100][100],b[100][100],sum[100][100];
        int i,j,row,col;

        printf("Enter the numbers of the rows and columns:");
        scanf("%d %d",&row,&col);

        printf("Enter the first matrix elements\n");

        for(i=0;i<row;i++) {
                for(j=0;j<col;j++) {

                        scanf("%d",&a[i][j]);
                }
        }

        printf("Enter the second matrix elements\n");

        for(i=0;i<row;i++) {
                for(j=0;j<col;j++) {

                        scanf("%d",&b[i][j]);
                }
        }

        for(i=0;i<row;i++) {
                for(j=0;j<col;j++) {

                        sum[i][j] = a[i][j] + b[i][j];
                }
        }

        printf("The resultant matrix is:\n");

        for(i=0;i<row;i++) {
                for(j=0;j<col;j++) {

                        printf("%d\t",sum[i][j]);
                }
                printf("\n");
        }
        return 0;
}
```
## 18.Program in C for the subtraction of two matrices.
```c
#include<stdio.h>

int main()
{
        int a[100][100],b[100][100],sub[100][100];
        int i,j,row,col;

        printf("Enter the size of the rows and columns:\n");
        scanf("%d %d",&row,&col);

        printf("Enter the first matrix elements:\n");

        for(i=0;i<row;i++) {
                for(j=0;j<col;j++) {

                        scanf("%d",&a[i][j]);
                }
        }

        printf("Enter the second matrix elements:\n");

        for(i=0;i<row;i++) {
                for(j=0;j<col;j++) {

                        scanf("%d",&b[i][j]);
                }
        }

        for(i=0;i<row;i++) {
                for(j=0;j<col;j++) {

                     sub[i][j] = a[i][j] - b[i][j];
                }
        }

        printf("-----After subtraction of the matrices-----\n");

        for(i=0;i<row;i++) {
                for(j=0;j<col;j++) {

                        printf("%d\t",sub[i][j]);
                }
                printf("\n");
        }
        return 0;
}
```
## 19.Program in C for the multiplication of two square matrices.
```c
#include<stdio.h>

int main()
{
        int a[10][10],b[10][10],multi[10][10];
        int i,j,row,col;

        printf("Enter the rows and column size\n");
        scanf("%d %d",&row,&col);

        printf("Enter the first matrix elements:\n");

        for(i=0;i<row;i++) {
                for(j=0;j<col;j++) {

                        scanf("%d",&a[i][j]);
                }
        }

        printf("Enter the second matrix elements\n");

        for(i=0;i<row;i++) {
                for(j=0;j<col;j++) {

                        scanf("%d",&b[i][j]);
                }
        }

        for(i=0;i<row;i++) {
                for(j=0;j<col;j++) {

                        multi[i][j] = a[i][j] * b[i][j];
                }
        }

        printf("The resultant matrix is:\n");

        for(i=0;i<row;i++) {
                for(j=0;j<col;j++) {

                        printf("%d\t",multi[i][j]);
                }
                printf("\n");
        }

                return 0;
        }
```
## 20.Program in C to find the transpose of a given matrix.
```c
#include<stdio.h>

int main()
{
        int a[100][100],trans[100][100];
        int i,j,row,col;

        printf("Enter the rows and columns size:");
        scanf("%d %d",&row,&col);

        printf("Enter the matrix elements:\n");

        for(i=0;i<row;i++) {
                for(j=0;j<col;j++) {

                        scanf("%d",&a[i][j]);
                }
        }

        printf("-----The original matrix-----\n");

        for(i=0;i<row;i++) {
                for(j=0;j<col;j++) {

                        printf("%d\t",a[i][j]);
                }
                printf("\n");
        }
        printf("----- After Transposing the matrix-----\n");

        for(i=0;i<col;i++) {
                for(j=0;j<row;j++) {

                        trans[i][j] = a[j][i];

        printf("%d\t",trans[i][j]);
                }

        printf("\n");
        }

        return 0;
}
```
## 21.Program in C to find the sum of the right diagonals of a matrix.
```c
#include<stdio.h>

int main()
{
        int arr[100][100];

        int i,j,n,sum=0;

        printf("Enter the array size");
        scanf("%d",&n);

        printf("Enter the %d x %d matrix\n",n,n);

        for(i=0;i<n;i++) {
                for(j=0;j<n;j++) {

                        scanf("%d",&arr[i][j]);
                }
        }

        printf("The matrix is\n");

        for(i=0;i<n;i++) {
                for(j=0;j<n;j++) {

                        printf("%d\t",arr[i][j]);
                }
                printf("\n");
        }

        printf("The right daigonal is:\n");

        for(i=0;i<n;i++) {
                for(j=0;j<n;j++) {

                        if(i+j == n-1) {

                        printf("%d\n",arr[i][j]);
                        }
                }
        }

        for(i=0;i<n;i++) {
                for(j=0;j<n;j++) {

                        if(i+j == n-1) {

                                sum = sum + arr[i][j];
                        }
                }
        }
        printf("The sum of right diagonal is:%d\n",sum);

        return 0;
}
```
## 22.Program in C to find the sum of the left diagonals of a matrix.
```c
#include<stdio.h>

int main()
{
        int arr[100][100];

        int i,j,n,sum=0;

        printf("Enter the array size:");
        scanf("%d",&n);

        printf("Enter %d x %d matrix\n",n,n);

        for(i=0;i<n;i++) {
                for(j=0;j<n;j++) {

                        scanf("%d",&arr[i][j]);
                }
        }

        printf("The matrix is:\n");

        for(i=0;i<n;i++) {
                for(j=0;j<n;j++) {

                        printf("%d\t",arr[i][j]);
                }
                printf("\n");
        }

        printf("The left diagonal is:\n");

        for(i=0;i<n;i++) {
                for(j=0;j<n;j++) {

                        if(i == j) {

                                printf("%d\n",arr[i][j]);

                        }
                }
        }

         for(i=0;i<n;i++) {
                for(j=0;j<n;j++) {

                        if(i == j) {

                            sum = sum + arr[i][j];

                        }
                }
        }
         printf("The sum of the left diagonal is:%d\n",sum);

         return 0;
}
```
## 23.Program in C to find the sum of rows and columns of a matrix.
```c
#include<stdio.h>

int main()
{
        int arr[100][100];

        int i,j,n,sum=0;

        printf("Enter the array size:");
        scanf("%d",&n);

        printf("Enter %d x %d matrix\n",n,n);

        for(i=0;i<n;i++) {
                for(j=0;j<n;j++) {

                        scanf("%d",&arr[i][j]);
                }
        }

        printf("The matrix is:\n");

        for(i=0;i<n;i++) {
                for(j=0;j<n;j++) {

                        printf("%d\t",arr[i][j]);
                }
                printf("\n");
        }

        printf("The left diagonal is:\n");

        for(i=0;i<n;i++) {
                for(j=0;j<n;j++) {

                        if(i == j) {

                                printf("%d\n",arr[i][j]);

                        }
                }
        }

         for(i=0;i<n;i++) {
                for(j=0;j<n;j++) {

                        if(i == j) {

                            sum = sum + arr[i][j];

                        }
                }
        }
         printf("The sum of the left diagonal is:%d\n",sum);

         return 0;
}
```
## 24.Program in C to print or display the lower triangular of a given matrix.
```c
#include<stdio.h>

int main()
{
        int arr[100][100];
        int i,j,n;

        printf("Enter the array size:");
        scanf("%d",&n);

        printf("Enter the %d x %d matrix\n",n,n);

        for(i=0;i<n;i++) {
                for(j=0;j<n;j++) {

                        scanf("%d",&arr[i][j]);
                }
        }

        printf("The matrix is\n");

        for(i=0;i<n;i++) {
                for(j=0;j<n;j++) {

                        printf("%d\t",arr[i][j]);
                }
                printf("\n");
        }

        printf("The lower matrix is\n");

        for(i=0;i<n;i++) {
                for(j=0;j<n;j++) {

                        if(i>=j)
                                printf("%d\t",arr[i][j]);
                        else
                                printf("\t");

                }
                        printf("\n");
        }
        return 0;
}
```
## 25.Program in C to print or display an upper triangular matrix.
```c
#include<stdio.h>

int main()
{
        int arr[100][100];
        int i,j,n;

        printf("Eter the matrix size:");
        scanf("%d",&n);

        printf("Enter the %d x %d matrix\n",n,n);

        for(i=0;i<n;i++) {
                for(j=0;j<n;j++) {
                        scanf("%d",&arr[i][j]);
                }
        }

        printf("The matrix is\n");

        for(i=0;i<n;i++) {
                for(j=0;j<n;j++) {

                        printf("%d\t",arr[i][j]);
                }
                printf("\n");
        }

        printf("The upper matrix is\n");

        for(i=0;i<n;i++) {
                for(j=0;j<n;j++) {

                        if(i<=j)
                printf("%d\t",arr[i][j]);
        else

                printf("\t");
                }
               printf("\n");
        }

       return 0;
}
```
## 26.Program in C to calculate the determinant of a 3 x 3 matrix.
```c
#include<stdio.h>

int main()
{

        int a[3][3];
        int i,j,det;

        printf("Etnter the 3 x 3 matrix\n");



        for(i=0;i<3;i++) {
                for(j=0;j<3;j++) {

                        scanf("%d",&a[i][j]);
                }
        }

         printf("The 3 x 3 matrix is\n");

         for(i=0;i<3;i++) {
                 for(j=0;j<3;j++) {

                         printf("%d\t",a[i][j]);
                 }
                 printf("\n");
         }

                          det = a[0][0]*(a[1][1]*a[2][2] - a[1][2]*a[2][1])
                               -a[0][1]*(a[1][0]*a[2][2] - a[1][2]*a[2][0])
                               +a[0][2]*(a[1][0]*a[2][1] - a[1][1]*a[2][0]);



           printf("Determinat is=%d\n",det);

           return 0;
}
```
## 27.Program in C to accept two matrices and check whether they are equal.
```c
#include<stdio.h>

int main()
{
        int a[100][100],b[100][100];
        int i,j,row,col,flag=1;

        printf("Enter the row and column size\n");
        scanf("%d %d",&row,&col);

        printf("Enter the first matrix elements\n");
        for(i=0;i<row;i++) {
                for(j=0;j<col;j++) {

                        scanf("%d",&a[i][j]);
                }
        }

        printf("Enter the second matrix elements\n");

        for(i=0;i<row;i++) {
                for(j=0;j<col;j++) {

                        scanf("%d",&b[i][j]);
                }
        }

        printf("The first matrix is\n");

        for(i=0;i<row;i++) {
                for(j=0;j<col;j++) {

                        printf("%d\t",a[i][j]);
                }
                printf("\n");
        }

        printf("The second matrix is\n");

        for(i=0;i<row;i++) {
                for(j=0;j<col;j++) {

                        printf("%d\t",b[i][j]);
                }
                printf("\n");
        }

        for(i=0;i<row;i++) {
                for(j=0;j<col;j++) {

                        if(a[i][j] != b[i][j]) {

                                flag=0;
                                break;
                        }
                }

                if(flag==0)
                        break;
        }

                        if(flag==1) {

                        printf("Both matrices are equal\n");

                        }else{
                                printf("Both matrices are not equal\n");
                        }

        return 0;
}
```
## 28.Program in C to find the majority element of an array.(A majority element in an array A[] of size n is an element that appears more than n/2 times (and hence there is at most one such element).
```c
#include<stdio.h>

int main()
{
        int arr[100];
        int i,j,n,count,found;

        printf("enter the array size:");
        scanf("%d",&n);

        printf("Enter the %d elements\n",n);

        for(i=0;i<n;i++) {
                        scanf("%d",&arr[i]);
                }

        printf("The elements are:\n");

        for(i=0;i<n;i++) {

                        printf("%d\n",arr[i]);
                }

        found=0;

        for(i=0;i<n;i++) {
                count=0;
                for(j=0;j<n;j++) {

                        if(arr[i] == arr[j]) {

                                count++;

                        }
                }

        if(count > n/2) {

                printf("The majority element is:%d\n",arr[i]);

                found=1;
                break;
        }
        }

        if(!found) {

                printf("No majority elemnet is found\n");
        }

        return 0;
}
```
## 29.Program in C to find the missing number in a given array. There are no duplicates in the list.
```c
#include<stdio.h>

int main()
{
        int arr[100],sum=0,missing;
        int i,n,total;

        printf("Enter the n number");
        scanf("%d",&n);

        printf("Enter the %d number from 1 to %d",n-1,n);

        for(i=0;i<n-1;i++) {
                scanf("%d",&arr[i]);

                 sum+=arr[i];
        }

        total = n*(n+1)/2;
        missing = total - sum;

        printf("The missing number is:%d",missing);

        return 0;
}
```
## 30.Program in C to find the two repeating elements in a given array.
```c
#include<stdio.h>

int main()
{
        int arr[100];
        int i,j,n;

        printf("Enter the array size:");

        scanf("%d",&n);

        printf("Enter %d elements\n",n);

        for(i=0;i<n;i++) {
                scanf("%d",&arr[i]);
        }

        printf("The repeated  elements are\n");

        for(i=0;i<n;i++) {
                for(j=i+1;j<n;j++) {

                        if(arr[i]==arr[j]) {
                                printf("%d\n",arr[i]);
                        }
                }
        }
        return 0;
}
```
## 31.Program to check if a given element is present in an array.
```c
#include<stdio.h>

int main()
{
        int arr[100];

        int i,j,n,search,found=0;

        printf("Enter the array size\n");
        scanf("%d",&n);

        printf("Enter %d  elements\n",n);

        for(i=0;i<n;i++) {
                scanf("%d",&arr[i]);
        }

        printf("Enter the number for searching\n");
        scanf("%d",&search);

        for(i=0;i<n;i++) {

                if( arr[i] == search) {

                        found =1;
                }
        }

        if(found==1) {
                printf("Number is present in an array\n");
        }
        else {
                printf("Nuber is not present in an array\n");
        }
        return 0;
}

```
## 32.Function to calculate the average of elements in an array.
```c
#include<stdio.h>


        float findaverage( int arr[],int n)
        {
        int sum=0;
        for(int i=0;i<n;i++) {

                sum+=arr[i];
        }

        return (float)sum/n;
        }

int main()
{
        int arr[100],i,n;
        float avg;

        printf("Enter the array size:");
        scanf("%d",&n);

        printf("Enter %d elements\n",n);

        for(i=0;i<n;i++) {

                scanf("%d",&arr[i]);
        }
        avg = findaverage(arr,n);

        printf("The average of array is :%.2f\n",avg);

        return 0;
}

```
## 33.Program to count the number of even and odd elements in an array.
```c
#include<stdio.h>

int main()
{
        int arr[100],even=0,odd=0;
        int i,n,count;

        printf("Enter the array size:");
        scanf("%d",&n);

        printf("Enter %d elements\n",n);

        for(i=0;i<n;i++) {

                scanf("%d",&arr[i]);
        }

        for(i=0;i<n;i++) {

                if(arr[i]%2==0) {

                        even++;
                }
                else{
                        odd++;
                }
        }

                printf("The number of even numbers are:%d\n",even);
                printf("the number of odd numbers are:%d\n",odd);
        return 0;
}
```
## 34. Implement a function to reverse the elements of an array.
```c
#include<stdio.h>

    void reverse (int arr[],int n)
{

        int start=0,end=n-1;
        int temp;

        while(start<end) {

                temp = arr[start];

                arr[start] = arr[end];

                arr[end] = temp;

                start++;
                end--;
        }
}

int main()
{
        int arr[100];
        int i,n;

        printf("Enter the array size:");
        scanf("%d",&n);

        printf("Enter %d elements\n",n);

        for(i=0;i<n;i++) {
                scanf("%d",&arr[i]);
        }

        reverse(arr,n);

        printf("After reversing the array\n");

        for(i=0;i<n;i++) {

                printf("%d\t",arr[i]);
        }
        printf("\n");
        return 0;
}
```
## 35. Implement a function to delete an element at a specific position in an array.
```c
#include<stdio.h>

void deleteElement(int arr[],int *n,int pos)
{
        int i;

        if(pos<1 || pos>*n) {
                printf("Invalid position\n");

                return ;
        }

       for(i=pos-1;i<*n-1;i++) {

               arr[i] = arr[i+1];
       }(*n)--;
}

int main()
{
        int arr[100];
        int i,n,pos;

        printf("Enter the array size:");
        scanf("%d",&n);

        printf("Enter %d elements\n",n);

        for(i=0;i<n;i++) {
                scanf("%d",&arr[i]);
        }

        printf("Enter the position of deletion from 1 to %d\n",n);
        scanf("%d",&pos);

        deleteElement(arr,&n,pos);

        printf("-----After deletion-----\n");

        for(i=0;i<n;i++) {
                printf("%d\n",arr[i]);
        }

        return 0;
}
```
## 36.Function to find the product of all elements in an array.
```c
#include<stdio.h>

int findproduct(int arr[],int n)
{
        int i,product=1;

        for(i=0;i<n;i++) {

                product = product * arr[i];
        }
        return product;
}

int main()
{
        int i,n,arr[200];
        int result;

        printf("Enter the array size:");
        scanf("%d",&n);

        printf("Enter %d elements\n",n);

        for(i=0;i<n;i++) {

                scanf("%d",&arr[i]);
        }

        result =findproduct(arr,n);

        for(i=0;i<n;i++) {


        }printf("The product of elements of an array is:%d\n",result);


        return 0;
}
```
## 37. Print Square of Array Elements in C.
```c
#include<stdio.h>

int main()
{
        int arr[100];
        int i,n,square[100];

        printf("Enter the array size:");
        scanf("%d",&n);

        printf("Enter %d elements\n",n);

        for(i=0;i<n;i++) {

                scanf("%d",&arr[i]);
        }

        printf("The square of an array is\n");

        for(i=0;i<n;i++) {

                square[i] = arr[i] * arr[i];
                 printf("%d\n",square[i]);
        }
        return 0;
}
```
## 38. Print Ascii Values using Array in C.
```c
#include<stdio.h>

int main()
{
        int str[100];
        int i;

        printf("Enter the string\n");
        scanf("%ls",str);

        for(i=0;str[i]!='\0';i++) {
                printf("The ASCII value of %c is %d\n",str[i],str[i]);
        }

        return 0;
}
```
## 39.Program To Find Two Elements whose Sum is Closest to Zero.
```c
#include<stdio.h>
#include<stdlib.h>

int compare(const void *a,const void *b) {

        return(*(int*)a - *(int*)b);
}

int main()
{
        int arr[100];
        int i,left,right;
        int min_left,min_right,min_sum;
        int sum,n;

        printf("Enter the number of elements:");
        scanf("%d",&n);

        printf("Enter %d elements\n",n);

        for(i=0;i<n;i++) {

                scanf("%d",&arr[i]);
        }

        qsort(arr,n,sizeof(int),compare);

        left=0;
        right=n-1;

        while(left < right) {

                sum = arr[left] +arr[right];

                if(sum <min_sum) {

                min_sum = sum;
                min_left = left;
                min_right = right;
                }

                if(sum < 0)

                        left++;
                        else
                                right--;
        }

        printf("The two elements closest to zero are : %d and %d\n",arr[min_left],arr[min_right]);

        return 0;
}
```
## 40.Program to Find Union and Intersection of Two Arrays.
```c
#include<stdio.h>

int main()
{
        int a[100],b[100],uni[100],inter[100];

        int m,n,i,j,k=0,l=0,found;

        printf("Enter the first array size:");
        scanf("%d",&m);

        printf("Enter %d elements\n",m);

        for(i=0;i<m;i++) {

                scanf("%d",&a[i]);
        }

        printf("Enter the second array size:");
        scanf("%d",&n);

        printf("Enter %d elements\n",n);

        for(i=0;i<n;i++) {

                scanf("%d",&b[i]);
        }

        for(i=0;i<m;i++)

                uni[k++] = a[i];

        for(i=0;i<n;i++) {
                found=0;

                for(j=0;j<m;j++){

                if(b[i] == a[j]) {
                        found=1;
                        break;
                }
                }

                if(found==0)

                        uni[k++]=b[i];
                }

                for(i=0;i<m;i++) {
                        for(j=0;j<n;j++) {

                                if(a[i] == b[j]) {

                                        inter[l++] = a[i];
                                        break;

                                }
                        }
                }

                printf("The union is\n");

                for(i=0;i<k;i++) {

                        printf(" %d \n",uni[i]);
                }

                printf("The intersection is:");
                for(i=0;i<l;i++) {
                        printf("%d\n",inter[i]);
                }


                return 0;
}
```
## 41.Program to Print all Non Repeated Elements in an Array.
```c
#include<stdio.h>

int main()
{
        int arr[100];
        int i,j,n,found=0;

        printf("Enter the array size:");

        scanf("%d",&n);

        printf("Enter %d elements\n",n);

        for(i=0;i<n;i++) {
                scanf("%d",&arr[i]);
        }

        for(i=0;i<n;i++) {
                for(j=i+1;j<n;j++) {

                        if(arr[i]==arr[j]) {

                                if(found==0) {
                                printf("The repeated elements are\n");

                                }

                                printf("%d\n",arr[i]);
                                found=1;
                                break;
                        }
                }
        }

        if(found==0) {

                printf("There are no repeated elements\n");
}

        return 0;
}
```
## 42.Program to write all the elements of 2-D Array into !-D Array in row wise.
43. Write a program to write whether a matrix is symmetric or not
44. Write a program to check if elements of an array are distinct or not.
 45.Write a program to remove duplicate elements from a sorted array.
37. Write a program to find out whether a square matrix is symmetric or not. A square matrix is 
symmetric if the transpose of the matrix is equal to the matrix.
38. Write a recursive function to find the sum of all even numbers in an array.
39. Write a recursive function that finds the sum of all elements of an array by repeatedly 
partitioning it into two almost equal parts.
40. Write a recursive function to reverse the elements of an array..
41. Write a recursive function to find whether the elements of an array are in strict ascending 
order or not.
42. Write a program to find the sum of rows and columns of a 2-d array and store the sums in 
the same array

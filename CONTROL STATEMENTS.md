## 1.C PROGRAM TO ACCEPT TWO INTEGERS AND CHECK WHETHER THEY ARE EQUAL OR NOT
```c
#include<stdio.h>
int main() {
        int a,b;
        printf("enter the numbers:");
        scanf("%d %d",&a,&b);
        if(a==b)
                printf("both are equal\n");
        else
                printf("both are not equal\n");
        return 0;
}
```
## C PROGRAM TO PRINT 
```c
#include<stdio.h>
int main()
{
        int a;
        printf("enter the number:");
        scanf("%d",&a);
        if(a%2==0){
                printf("even number\n");
        }       else{
                        printf("odd number\n");
        }
        return 0;
}
```

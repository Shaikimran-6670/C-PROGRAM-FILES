## 1.C PROGRAM TO ACCEPT TWO INTEGERS AND CHECK WHETHER THEY ARE EQUAL OR
NOT
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

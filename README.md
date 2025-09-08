## 1.hello world program.
```c
#include<stdio.h>
int main() {
        printf("hello world\n");
        return 0;
}
```
## 2. equal numbers or not program.
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

## 3. even or odd number program.
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


## 1. equal numbers or not program.
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

## 2. even or odd number program.
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
## 3. positive and negative numbers program.
```c
#include<stdio.h>
int main() {
        int a;
        printf("enter the number:");
        scanf("%d",&a);
        if(a>0)
                printf("positive number\n");
        else
                printf("negative number\n");
        return 0;
}
```
## 4. Leap year program.
```c
#include<stdio.h>
int main()
{
        int year;
        printf("enter the year:");
        scanf("%d",&year);
        if(year%4==0)
                printf("Leap year\n");
        else
                printf("Not a leap year\n");
        return 0;
}
```
## 5.C PROGRAM TO READ THE AGE OF A CANDIDATE AND DETERMINE WHETHER HE/SHE IS
ELIGIBLE TO CAST HIS/HER OWN VOTE
```c
#include<stdio.h>
int main()
{
        int age;
        printf("enter the age:");
        scanf("%d",&age);
        if(age>=18)
                printf("Eligible for vote\n");
        else
                printf("Not eligible for vote\n");
        return 0;
}
```

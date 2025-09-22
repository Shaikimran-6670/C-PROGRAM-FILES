
## 1. C PROGRAM WHETHER NUMBERS EQUAL OR NOT.
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

## 2. C PROGRAM TO PRINT EVEN OR ODD.
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
## 5.C PROGRAM TO READ THE AGE OF A CANDIDATE AND DETERMINE WHETHER HE/SHE IS ELIGIBLE TO CAST HIS/HER OWN VOTE
```c
#include<stdio.h>
```
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
## 6.C PROGRAM TO READ THE VALUE OF AN INTEGER M AND DISPLAY THE VALUE OF N IS 1 WHEN M IS LARGER THAN 0, 0 WHEN M IS 0 AND -1 WHEN M IS LESS THAN 0.
```c
#include<stdio.h>
int main() {

        int m,n;

        scanf("%d",&m);
        if (m>0)
                n=1;

           else if  (m<0)
                n=-1;

        else
                n=0;

        printf("%d",n);
        return 0;
}
```
## 7.C PROGRAM TO FIND THE LARGEST OF THREE NUMBERS
```c
#include<stdio.h>
int main() {

        int a,b,c;

        printf("enter the number:");
        scanf("%d %d %d",&a,&b,&c);

        if(a>=b && a>=c){
                printf("%d is the big number\n",a);

        }else if (b>=a && b>=c){
                printf("%d is the big number\n",b);

        }else{
                printf("%d is the big number\n",c);
        }

        return 0;
}
```
## 8.C PROGRAM TO CHECK WHETHER A CHARACTER IS A VOWEL OR CONSONANT
```c
#include<stdio.h>
int main() {

        char ch;

        printf("enter the cheacter:");
        scanf("%c",&ch);

         if((ch=='A' || ch=='E' || ch=='I' || ch=='O' || ch=='U')||
           (ch=='a' || ch=='e' || ch=='i' || ch=='o' || ch=='u')){

                printf(" is the vowel");

        }else{
                printf(" is the consonant");
        }
        return 0;
}
```
## 9.C PROGRAM TO CHECK WHETHER A CHARACTER IS AN ALPHABET OR NOT
```c
#include<stdio.h>
int main () {

        char ch;
        scanf("%c",&ch);

        if((ch>='A' && ch<='Z') ||
                (ch>='a' && ch<='z')){

                printf("character");
        }else
                printf("not a character");
                return 0;
        }
```
## 10.C PROGRAM TO FIND MINIMUM OR MAXIMUM BETWEEN TWO NUMBERS
```c
#include<stdio.h>
int main() {

        int a,b;

        printf("enter the numbers:");
        scanf("%d %d",&a,&b);

        if(a>b) {

                printf("%d is the maximum\n",a);
                printf("%d is the minimum\n",b);
        }

        else if (b>a) {

                printf("%d is the maximum\n",b);
                printf("%d is the minimum\n",a);
        }

         else {
                printf("both are equal\n");
         }
                return 0;
}
```
## 11.C PROGRAM TO ENTER WEEK NUMBER AND PRINT DAY OF WEEK
```c
#include<stdio.h>
int main() {

        int day;

        printf("enter the week:");
        scanf("%d",&day);

        switch(day) {
                case 1:
                         printf("sunday\n");
                        break;
                case 2:
                        printf("monday\n");
                        break;
                case 3:
                         printf("tuesday\n");
                        break;
                case 4:
                         printf("wedensday\n");
                        break;
                case 5:
                         printf("thursday\n");
                        break;
                case 6:
                         printf("friday\n");
                        break;
                case 7:
                         printf("saturday\n");
                        break;

        default:
        printf("invalid week number");

        break;
        }
        return 0;
}
```
## 12.C PROGRAM TO CHECK WHETHER A CHARACTER IS UPPERCASE OR LOWERCASE
```c
#include<stdio.h>
int main() {

        char ch;

        printf("enter the charcter:");
        scanf("%c",&ch);

        if(ch>='A' && ch<='Z') {
                printf("UPPER CASE\n");
        }else{
                printf("LOWER CASE\n");
        }
        return 0;
}
```
## 13.C PROGRAM TO FIND NUMBER OF DAYS IN MONTH
```c
#include<stdio.h>
int main()
{
        int month;

        printf("enter the month number:");
        scanf("%d",&month);

        switch(month) {

                case 1:
                case 3:
                case 5:
                case 7:
                case 8:
                case 10:
                case 12:
                        printf("31 days\n");
                        break;

                case 4:
                case 6:
                case 9:
                case 11:
                        printf("30 days\n");
                        break;
                case 2:
                        printf("28 or 29 days\n");
                        break;

                default:
                        printf("invalid month\n");
                        break;
        }
        return 0;
}
```
## 14.C PROGRAM TO FIND MAXIMUM BETWEEN TWO NUMBERS USING SWITCH CASE
```c
#include<stdio.h>
int main() {

        int a,b;

        printf("enter the numbers:");
        scanf("%d %d",&a,&b);

        switch(a>b) {
        case 1:
                printf("%d is maximum\n",a);
                printf("%d is minimum\n",b);
        break;

        case 0:

        switch(a<b) {
        case 1:
                printf("%d is maximum\n",b);
                printf("%d is minimum\n",a);

                break;

        case 0:
                printf("both are equal\n");
                break;
        }

        break;

        }
        return 0;
}
```
## 15.C PROGRAM TO PRINT EVEN NUMBERS BETWEEN 1 TO 20 USING A FOR LOOP
```c
#include<stdio.h>
int main() {

        int i;
        for(i=1;i<=20;i++) {

             if(i%2==0)
             printf("%d\n",i);

        }
        return 0;
}
```
## 16.PROGRAM TO CALCULATE THE SUM OF NUMBERS FROM 1 TO 100 USING A WHILE LOOP

```c

#include<stdio.h>
int main()
{
        int i,n=100,sum=0;

        i=0;
        while(i<=n) {
                sum=sum + i;
                i++;
        }
        printf("%d\n",sum);

        return 0;
}
```
## 17.C PROGRAM TO FIND THE FACTORIAL OF A GIVEN NUMBER USING A FOR LOOP
```c
#include<stdio.h>
int main() {

        int i,n;
        int fact=1;

        printf("enter the number:");
        scanf("%d",&n);

        for(i=1;i<=n;i++){
                fact=fact*i;

        }

        printf("%d",fact);
        return 0;

}
```
## 18.C PROGRAM TO CHECK WHETHER A GIVEN NUMBER IS PRIME OR NOT USING A WHILE LOOP.
```c
#include<stdio.h>
int main() {
        int i=1,n;
        int count=0;

        printf("enter the number:");
        scanf("%d",&n);

                while(i<=n) {
                if(n%i==0)
                count++;
                i++;
                }

        if(count==2)
        printf("prime\n");

        else

        printf("not prime\n");

                return 0;
}
```


## 19.C PROGRAM TO PRINT SUM OF DIGITS.
```C

#include<stdio.h>
int main()
{
         long long  int i,sum=0,digit,n;

        printf("enter the digit:");
        scanf("%lld",&n);

        i=1;
        while(n>0) {
                digit = n % 10;
                sum = sum + digit;
                n = n/10;
                i++;
        }

        printf("%lld",sum);

        return 0;
}
```


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
## 20.C PROGRAM TO PRINT FIBONACCI SERIES UP TO N TERMS USING A FOR LOOP
```c
#include<stdio.h>
int main() {
        int count=2,n;
        int i,a=0,b=1,next;
        printf("enter the terms:");
        scanf("%d",&n);

        printf("fibanocci series:\n");

        if(n>=1)
                printf("%d\n",a);
        if(n>=2)
                printf("%d\n",b);
        while(count<n) {
                next=a+b;
        printf("%d\n",next);
         a=b;
         b=next;
         count++;
        }
        return next;
}
```
## 21.C PROGRAM TO REVERSE A GIVEN NUMBER USING A WHILE LOOP
```c
#include<stdio.h>
int main()
{
        long long int i,num,reverse=0,original;

        printf("enter the number:");
        scanf("%lld",&num);

        i=0;
        while(num>0) {

           original = num % 10;

           reverse = reverse * 10 + original;

           num = num / 10;
        }
        printf("%lld",reverse);

        return 0;
}
```
## 22.C PROGRAM TO FIND THE LARGEST ELEMENT IN AN ARRAY USING A FOR LOOP
```c
#include<stdio.h>
int main()
{
        int i;
       int arr[10],large;

        printf("enter the values:");
        for(i=0;i<5;i++)
        scanf("%d",&arr[i]);

        large=arr[5];

        for(i=0;i<5;i++)

                if(arr[i]>large)

                        large=arr[i];

        printf("the largest element is:%d\n",large);

        return 0;
}
```
## 23.C PROGRAM TO FIND THE SMALLEST ELEMENT IN AN ARRAY USING A WHILE LOOP
```c
#include<stdio.h>
int main()
{
        int arr[10];
        int i,small;
        printf("enter the values:");
        for(i=0;i<5;i++) {
                scanf("%d",&arr[i]);
        }
        small=arr[0];
        for(i=0;i<5;i++) {
                if(arr[i]<small)
                        small=arr[i];
        }
        printf("the smallest element is:%d\n",small);
        return 0;
}
```
## 24.C PROGRAM TO PRINT ALL THE ELEMENTS OF AN ARRAY USING A FOR LOOP
```c
#include<stdio.h>
int main()
{
        int arr[10];
        int i;

        printf("enter the element:");

        for(i=0;i<10;i++){
                scanf("%d",&arr[i]);
        }
        for(i=0;i<10;i++)
                        printf("%d\n",arr[i]);

        return 0;
}
```
## 25.C PROGRAM TO FIND THE SUM OF ELEMENTS IN AN ARRAY USING A WHILE LOOP
```c
#include<stdio.h>
int main() {
        int arr[5],i,sum=0;
        printf("enter the array:");
        for(i=0;i<5;i++){
                scanf("%d",&arr[i]);
        }
        for(i=0;i<5;i++)

        while(i<5){
                sum=sum+arr[i];
                i++;

        }
        printf("the sum of all elements is:%d\n",sum);

}
```
## 26.C PROGRAM TO COUNT THE NUMBER OF VOWELS IN A GIVEN STRING USING A FOR LOOP.
```c
#include<stdio.h>
#include<string.h>
int main() {

        char str[100];
        int i,count=0;

        printf("enter the string:");

        fgets(str,100,stdin);

        str[strcspn(str,"\n")]='\0';

        for(i=0;str[i]!='\0';i++){

        if((str[i]=='a' || str[i]=='e' || str[i]=='i' || str[i]=='o' || str[i]=='u') ||
            (str[i]=='A' || str[i]=='E' || str[i]=='I' || str[i]=='O' || str[i]=='U'))
                count++;
        }


        printf("the number of vowels are:%d\n",count);
        return 0;
}
```
## 27.C PROGRAM TO COUNT THE NUMBER OF WORDS IN A GIVEN STRING USING A WHILE LOOP
```c
#include<stdio.h>
#include<string.h>

int main() {
        char str[100];
        int i=0,count=1;
        printf("enter the string:");
        fgets(str,sizeof(str),stdin);
        str[strcspn(str,"\n")]='\0';

        while(str[i]!='\0'){
                if(str[i]==' '||str[i]=='\n'&& str[i]!='\0')

                        count++;
                        i++;
        }

                     printf("the number of words are:%d\n",count);

        return 0;
}
```
## 28.C PROGRAM TO CHECK WHETHER A GIVEN STRING IS A PALINDROME OR NOT USING A FOR LOOP.
```c

#include <stdio.h>
#include<string.h>

int main() {
        char str[100];
        int i,len,flag=1;

        printf("enter the  string:");
        scanf("%s",str);

        len= strlen(str);

        for(i=0;i < len/2;i++) {
        if(str[i] != str[len-1-i]) {
                        flag=0;
                        break;
                }
        }
        if(flag)
                printf("palindrome\n");
        else
                printf("not palindrome\n");
        return 0;
}
```
## 29.A C PROGRAM TO CONCATENATE TWO STRINGS WITHOUT USING LIBRARY FUNCTIONS USING A WHILE LOOP.
```c

#include <stdio.h>
#include<string.h>

int main() {
        char str[100];
        int i,len,flag=1;

        printf("enter the  string:");
        scanf("%s",str);

        len= strlen(str);

        for(i=0;i < len/2;i++) {
        if(str[i] != str[len-1-i]) {

                        flag=0;
                        break;
                }
        }
        if(flag)
                printf("palindrome\n");
        else
                printf("not palindrome\n");
        return 0;
}
```
## 30.C PROGRAM TO FIND THE LENGTH OF A STRING USING A FOR LOOP
```c
#include<stdio.h>
#include<string.h>

int main() {

        char str[100];
        int i=0,count=1;

        printf("enter the string:");
        fgets(str,sizeof(str),stdin);
        str[strcspn(str,"\n")]='\0';

        while(str[i]!='\0'){
                if(str[i]==' '||str[i]=='\n'&& str[i]!='\0')

                        count++;
                        i++;
        }

                     printf("the number of words are:%d\n",count);

        return 0;
}

```
## 31.C PROGRAM TO CONVERT A STRING TO UPPERCASE USING A WHILE LOOP.
```c
#include<stdio.h>
#include<string.h>

int main() {
        char str[100];
        int i=0;

        printf("enter the string:");

        fgets(str,sizeof(str),stdin);

        str[strcspn(str,"\n")] ='\0';

        while(str[i] != '\0') {

                if(str[i]>= 'a' && str[i]<= 'z')

                str[i] = str[i] - 32;
                i++;
        }

        printf("%s",str);
        return 0;
}
```
## 32.C PROGRAM TO FIND THE POWER OF A NUMBER USING A FOR LOOP
```c
#include<stdio.h>
#include<string.h>

int main() {

        long long int i,base;
        long long int result=1,exponent;

        printf("enter the base:");
        scanf("%lld",&base);

        printf("enter the exponent:");
        scanf("%lld",&exponent);

        for(i=1;i<=exponent;i++) {
                result = result * base;

        }

        printf("%lld^%lld = %lld\n",base,exponent,result);
        return 0;
}
```
## 33.C PROGRAM TO FIND THE FACTORIAL OF A NUMBER USING A WHILE LOOP.
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
## 34.C PROGRAM TO FIND THE GCD OF TWO NUMBERS USING A WHILE LOOP.
```c
#include<stdio.h>

int main()
{
        int a,b;

        printf("enter two numbers:");
        scanf("%d %d",&a,&b);

        while(a != b) {
          if(a>b)
                a=a-b;
        else
                b=b-a;
        }
        printf("GCD is:%d\n",a);
        return 0;
}
```
## 35.A C PROGRAM TO FIND THE LCM OF TWO NUMBERS USING A FOR LOOP.
```c
#include<stdio.h>

void  main()
{
        int a,b,i=2,lcm;

        printf("enter the two numbers:");
        scanf("%d %d",&a,&b);

        for((a>b ? a:b); ;i++) {

                if(i % a==0 && i % b==0) {

                        lcm = i;
                        break;

                }
        }


        printf("LCM of %d and %d is:%d\n",a,b,lcm);


}
```
## 36.C PROGRAM TO PRINT THE MULTIPLICATION TABLE OF A GIVEN NUMBER USING A FOR LOOP.
```c
#include<stdio.h>

int main()
{
        int i,n,table;

        printf("enter the number:");
        scanf("%d",&n);

        for(i=1;i<=10;i++) {

                table =n * i;

        printf("%d x %d = %d\n",n,i,table);
        }

        return 0;
}
```
## 37.PROGRAM IN C TO PRINT THE ARMSTRONG NUMBERS BETWEEN 1 AND 1000 USING A FOR LOOP.
```c
#include<stdio.h>

int main()
{
        int i,temp,sum=0,digit;

        printf("the armstrong numbers are:\n");


        for(i=1;i<=1000;i++) {

                sum = 0;
                temp = i;


                while(temp > 0) {

                        digit = temp % 10;

                        sum = sum + (digit *digit * digit);

                        temp = temp / 10;
        }

        if(sum == i) {

                printf("%d\n",i);
        }
        }

        return 0;
}
```
## 38.A PROGRAM IN C TO IMPLEMENT A SIMPLE CALCULATOR USING SWITCH-CASE STATEMENTS.
```c
#include<stdio.h>
int main()

{
        int a,b;
        char op;

        printf("enter the numbers:");


        scanf("%d %d",&a,&b);

        printf("enter the oeprator:+,-,*,/,%%:");

        scanf(" %c",&op);

        switch(op) {

                case '+':
                        printf("%d",a+b);
                        break;

                case '-':
                         printf("%d",a-b);
                        break;

                case '*':
                         printf("%d",a*b);
                        break;

                case '/':
                         printf("%d",a/b);
                        break;

                case '%':
                         printf("%d",a%b);
                         break;
        default:
printf("invlaid operator\n");
}

return 0;
}
```
## 39.PROGRAM IN C TO CHECK WHETHER A GIVEN NUMBER IS A PALINDROME OR NOT USING WHILE LOOPS AND IF-ELSE STATEMENTS.
```c
#include<stdio.h>

int main() {

        int num,reverse=0,digit;

        int original;

        printf("enter the number:");
        scanf("%d",&num);

        original = num;

        for( ;num >0;) {

                digit=num%10;

                reverse = reverse*10+digit;

                num= num/10;
        }
        if(original == reverse)

                printf("%d is palindrome\n",original);

        else

                printf("%d is not palindrome\n",original);


        return 0;
}
```
## 40.PROGRAM IN C TO FIND THE SUM OF ELEMENTS IN THE LOWER TRIANGULAR  MATRIX USING LOOPS AND IF-ELSE STATEMENTS.
```c
#include<stdio.h>

int main()
{
        int arr[3][3];

        int i,j,sum=0;

        printf("enter the array elements:");

        for(i=0;i<3;i++) {

                for(j=0;j<3;j++) {

                        scanf("%d",&arr[i][j]);

                }
        }

        printf("the matrix is\n");

        for(i=0;i<3;i++) {

                for(j=0;j<3;j++) {

                        printf("%d\t",arr[i][j]);

                }


        printf("\n");
        }

        printf("the lower traingular is:\n");

        for(i=0;i<3;i++) {

                for(j=0;j<3;j++) {

                        if(i>=j) {

                                printf("%d\t",arr[i][j]);

                                sum+=arr[i][j];
                        }

                }
                        printf("\n");
        }

        printf("%d",sum);

        return 0;
}

```
## 41.PROGRAM IN C TO FIND THE SUM OF ELEMENTS IN THE UPPER TRIANGULAR  MATRIX USING LOOPS AND IF-ELSE STATEMENTS.
```c
#include<stdio.h>

int main()
{
        int arr[3][3];

        int i,j,sum=0;

        printf("enter the array elements:");

        for(i=0;i<3;i++) {

                for(j=0;j<3;j++) {

                        scanf("%d",&arr[i][j]);

                }
        }

        printf("the matrix is\n");

        for(i=0;i<3;i++) {

                for(j=0;j<3;j++) {

                        printf("%d\t",arr[i][j]);

                }


        printf("\n");
        }

        printf("the lower traingular is:\n");

        for(i=0;i<3;i++) {

                for(j=0;j<3;j++) {

                        if(i<=j) {

                                printf("%d\t",arr[i][j]);

                                sum+=arr[i][j];
                        }

                }
                        printf("\n");
        }

        printf("%d",sum);

        return 0;
}

```
## 42.PROGRAM IN C TO REMOVE DUPLICATE ELEMENTS FROM AN ARRAY USING LOOPS AND IF-ELSE STATEMENTS.
```c
#include<stdio.h>

int main()
{
        int arr[100],visited[100]={0};
        int i,j,count;

        printf("enter the numbers:");
        for(i=0;i<5;i++) {

                scanf("%d",&arr[i]);
        }

        for(i=0;i<5;i++) {

                if(visited[i]==0)

                        count=1;
                for(j=i+1;j<5;j++) {

                        if(arr[i]==arr[j]) {

                                count++;
                                visited[j]=1;
                        }
                }

                if(count==1)

                        printf("%d\n",arr[i]);
        }
        return 0;
}
```
## 43.PROGRAM IN C TO SORT AN ARRAY OF INTEGERS IN ASCENDING ORDER USING LOOPS AND IF-ELSE STATEMENTS.
```c
#include<stdio.h>

int main()
{
        int i,j,n,temp;
        int arr[100];

        printf("enter the number of the elements:");
        scanf("%d",&n);



                printf("enter %d integers\n",n);

                                 for(i=0;i<n;i++) {

                                         scanf("%d",&arr[i]);
                                 }

                                         for(i=0;i<n;i++) {

                                                 for(j=i+1;j<n;j++) {

                                                         if(arr[i] > arr[j]) {

                                                                  temp = arr[i];

                                                                  arr[i] = arr[j];

                                                                  arr[j] = temp;
                                                         }
                                                 }
                                         }

                                                 printf("ascending order is\n");

                                                 for(i=0;i<n;i++) {

                                                         printf("%d\n",arr[i]);
                                                 }


                                         return 0;
}
                    
```
## 44..WRITE A PROGRAM IN C TO SORT AN ARRAY OF INTEGERS IN DESCENDING ORDER USING LOOPS AND IF-ELSE STATEMENTS.
```c
#include<stdio.h>

int main()
{
        int i,j,n,temp;
        int arr[100];

        printf("enter the number of the elements:");
        scanf("%d",&n);



                printf("enter %d integers\n",n);

                                 for(i=0;i<n;i++) {

                                         scanf("%d",&arr[i]);
                                 }

                                         for(i=0;i<n;i++) {

                                                 for(j=i+1;j<n;j++) {

                                                         if(arr[i] < arr[j]) {

                                                                  temp = arr[i];

                                                                  arr[i] = arr[j];

                                                                  arr[j] = temp;
                                                         }
                                                 }
                                         }

                                                 printf("Descending order is\n");

                                                 for(i=0;i<n;i++) {

                                                         printf("%d\n",arr[i]);
                                                 }


                                         return 0;
}
```
## 45.A PROGRAM IN C TO FIND THE SECOND LARGEST ELEMENT IN AN ARRAY USING LOOPS AND IF-ELSE STATEMENTS.
```c
#include<stdio.h>

int main()
{
        int arr[100];
        int i,big,n,second;

        printf("enter the number of elements:\n");

        scanf("%d",&n);

        printf("enter %d elemnets:",n);

        for(i=0;i<n;i++) {

                scanf("%d",&arr[i]);
        }

        big= 0;

        second = 0;

         for (i=0;i<n;i++) {

                    if(arr[i] > big)  {


                            second = big;

                            big = arr[i];

                    } else if(arr[i] > second && arr[i] !=big ) {

                            second = arr[i];

                    }
            }

        printf("the second largest element is:%d",second);

          printf("\n");

        return 0;


}
```
## 46.PROGRAM IN C TO FIND THE FREQUENCY OF EACH ELEMENT IN AN ARRAY USING LOOPS AND IF-ELSE STATEMENTS.
```c
#include<stdio.h>

int main ()
{
        int arr[100],visited[10]={0};

        int i,n,count,j;

        printf("enter the number of the elements:");

        scanf("%d",&n);

        printf("enter the elemnets:");

        for(i=0;i<n;i++) {

                scanf("%d",&arr[i]);

        }

        for(i=0;i<n;i++) {

                if(visited[i] == 1)

           continue ;
                 count =1;

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
## 48.C PROGRAM TO PRINT ALL THE ODD NUMBERS BETWEEN 1 TO 50 USING A FOR LOOP.
```c
#include<stdio.h>

int main()
{
        int i;

                printf("the odd numbers from 1 to 50 are:\n");

        for(i=1;i<=50;i++) {

                if(i%2!=0)

                printf("%d\n",i);


        }
        return 0;
}
```
## 49.PROGRAM IN C TO FIND THE SUM OF ELEMENTS IN EACH COLUMN OF A MATRIX USING LOOPS AND IF-ELSE STATEMENTS.
```c
#include<stdio.h>


int main()
{
        int arr[10][10];

        int i,j,sc,rows,cols;

        printf("enter the row:");
        scanf("%d",&rows);

        printf("enter the columns:");
        scanf("%d",&cols);

        printf("enter the array elemnets:\n");

        for(i=0;i<rows;i++) {

                for(j=0;j<cols;j++) {

                        scanf("%d",&arr[i][j]);

                }
        }

        printf("the matrix is:\n");

        for(i=0;i<rows;i++) {

                for(j=0;j<cols;j++) {

                        printf("%d\t",arr[i][j]);
                }

                printf("\n");
        }

        for(i=0;i<rows;i++) {
                sc=0;

                for(j=0;j<cols;j++) {


                        sc+=arr[i][j];

                }

        printf("the sum of column %d:%d \n",i+1,sc);
        }

        return 0;
}

```
## 50.PROGRAM IN C TO FIND THE SUM OF ELEMENTS IN EACH ROW OF A MATRIX USING LOOPS AND IF-ELSE STATEMENTS.
```c
#include<stdio.h>

int main()
{
        int arr[10][10];

        int i,j,sum,sr,rows,cols,sc;

        printf("enter the row:");
        scanf("%d",&rows);

        printf("enter the colums:");
        scanf("%d",&cols);

        printf("enter the array elements:\n");

        for(i=0;i<rows;i++) {

                for(j=0;j<cols;j++) {

                        scanf("%d",&arr[i][j]);

                }

        }
        printf("the matrix is:\n");

        for(i=0;i<rows;i++) {

                for(j=0;j<cols;j++) {

                        printf("%d\t",arr[i][j]);
                }
                printf("\n");
        }

        for(i=0;i<rows;i++) {


                sum=0;
                sr=0;

                for(j=0;j<cols;j++) {

                        sum+=arr[j][i];


                }

                   printf("sum of row %d is:%d\n",i+1,sum);

                }

        return 0;
}
```
## 51.PROGRAM IN C TO ADD TWO MATRICES USING LOOPS AND IF-ELSE STATEMENTS.
```c
#include<stdio.h>

int main()
{
        int sum[10][10],a[10][10],b[10][10];

        int i,j,row,col;

        printf("enter the row size and column  size:");
        scanf("%d %d",&row,&col);

        printf("enter the first matrice elements:");

        for(i=0;i<row;i++) {
                for(j=0;j<col;j++) {
        scanf("%d",&a[i][j]);
                }
        }

        printf("enter the second matrice elements:");

        for(i=0;i<row;i++) {
                for(j=0;j<col;j++) {
        scanf("%d",&b[i][j]);
                }
        }



        printf("the two matrices are:\n");


        for(i=0;i<row;i++) {

                for(j=0;j<col;j++) {

                        printf("%d\t",a[i][j]);

                }

        printf("\n");
        }

        printf("-----------------------\n");

        for(i=0;i<row;i++) {
                for(j=0;j<col;j++) {
                        printf("%d\t",b[i][j]);
                }
                printf("\n");
        }
        printf("-----after adding matrices-----\n");

        for(i=0;i<row;i++) {
                for(j=0;j<col;j++) {

                        sum[i][j] = a[i][j] + b[i][j];

                printf("%d\t",sum[i][j]);
           }
                printf("\n");
        }



        return 0;
}
```
## 52.PROGRAM IN C TO SUBTRACT TWO MATRICES USING LOOPS AND IF-ELSE STATEMENTS.
```c
#include<stdio.h>

int main()
{
        int sub[10][10],a[10][10],b[10][10];

        int row,col,i,j;

        printf("enter the row and column size:");
        scanf("%d %d",&row,&col);

          printf("enter the first matrice:\n");

        for(i=0;i<row;i++) {
                for(j=0;j<col;j++) {

                  scanf("%d",&a[i][j]);

                }
        }

        printf("enter the second matrice:\n");
            for(i=0;i<row;i++) {
                for(j=0;j<col;j++) {

                        scanf("%d",&b[i][j]);
                }

        }

        printf("the two matrices are\n");

        for(i=0;i<row;i++) {
                for(j=0;j<col;j++) {

                        printf("%d\t",a[i][j]);
                }
                printf("\n");
        }


           printf("--------------------\n");

        for(i=0;i<row;i++) {
                for(j=0;j<col;j++) {

                        printf("%d\t",b[i][j]);
                }
                printf("\n");
        }

        printf("-----after the subtraction the matrices-----\n");

        for(i=0;i<row;i++) {
                for(j=0;j<col;j++) {

                        sub[i][j] = a[i][j] - b[i][j];

                        printf("%d\t",sub[i][j]);
                }
                printf("\n");
        }
        return 0;
}
```
## 53.PROGRAM IN C TO MULTIPLY TWO MATRICES USING LOOPS AND IF-ELSE STATEMENTS.
```c
#include<stdio.h>

int main()
{
        int mult[10][10],a[10][10],b[10][10];
        int i,j,row,col;

        printf("enter the size of row and column:");
        scanf("%d %d",&row,&col);

        printf("enter the first matrice:\n");

        for(i=0;i<row;i++) {
                for(j=0;j<col;j++) {

                        scanf("%d",&a[i][j]);
                }
        }
        printf("enter the second matrice:\n");

        for(i=0;i<row;i++) {
                for(j=0;j<col;j++) {
                        scanf("%d",&b[i][j]);
                }
        }
        printf("the matrices are\n");

        for(i=0;i<row;i++) {
                for(j=0;j<col;j++) {
                        printf("%d\t",a[i][j]);
                }
                printf("\n");
        }
        printf("-----------------\n");
        for(i=0;i<row;i++) {
                for(j=0;j<col;j++) {
                        printf("%d\t",b[i][j]);
                }
                printf("\n");
        }
        printf("-----after the multiplication of matrices-----\n");
        for(i=0;i<row;i++) {
                for(j=0;j<col;j++) {

                        mult[i][j] = a[i][j] * b[i][j];

                        printf("%d\t",mult[i][j]);
                }
                printf("\n");
        }
        return 0;
}
```
## 54.A PROGRAM IN C TO PRINT THE ELEMENTS OF AN ARRAY IN REVERSE ORDER USING LOOPS AND IF-ELSE STATEMENTS.
```c
#include<stdio.h>

int main()
{
        int arr[100];

        int i,n;

        printf("enter the number of elements:");

        scanf("%d",&n);

        printf("enter the %d elements:",n);

        for(i=0;i<n;i++) {

                scanf("%d",&arr[i]);

        }

        printf("the reverse mode of elements are:\n");

        for(i=n-1;i>=0;i--) {


                        printf("%d\n",arr[i]);

        }

        return 0;
}
```
## 55.PROGRAM IN C TO CHECK WHETHER TWO ARRAYS ARE EQUAL OR NOT USING LOOPS AND IF-ELSE STATEMENTS.
```c
#include<stdio.h>

int main()
{

        int arr1[100],arr2[100];

        int i,n;

        printf("enter the number of elements:");

        scanf("%d",&n);

        printf("enter the %d elements of first array:",n);

        for(i=0;i<n;i++) {

                scanf("%d",&arr1[i]);
        }

        printf("enter the %d elements of second array:",n);

        for(i=0;i<n;i++) {

                scanf("%d",&arr2[i]);
        }

        for(i=0;i<n;i++) {

                if(arr1[i] != arr2[i]) {

                        printf("the elements are not equal\n");

                return 0;

                }
        }

                       printf("the elememnts are equal\n");

      return 0;

}
```

# Bibi_w1
INFINITIX 
-------------------------------------------------------------------------
PROGRAM 1:
#include<stdio.h>
void main()
{
    int a,b;
    printf("Enter the number:");
    scanf("%d",&a);
    b=a+2;
    printf("Added value:%d",b);
}
--------------------------------------------------------------------------
PROGRAM 2:

#include<stdio.h>
void main()
{
    int a,b;
    printf("Enter the number:");
    scanf("%d",&a);
    b=a-5;
    printf("Subtracted value:%d",b);
--------------------------------------------------------------------------
PROGRAM 3:

#include<stdio.h>
void main()
{
    int a,b;
    printf("Enter the number:");
    scanf("%d",&a);
    b=a*3;
    printf("Multiplied value:%d",b);
}
--------------------------------------------------------------------------
PROGRAM 4:

#include<stdio.h>
void main()
{
    int a,b;
    printf("Enter the number:");
    scanf("%d",&a);
    b=a/6;
    printf("Quotient value:%d",b);
}
--------------------------------------------------------------------------
PROGRAM 5:


#include<stdio.h>
void main()
{
    int a,b;
    printf("Enter the number:");
    scanf("%d",&a);
    b=a%8;
    printf("Remainder value:%d",b);
}
--------------------------------------------------------------------------
PROGRAM 6:

#include<stdio.h>
int main()
{
    int number;
    printf("Enter a two-digit number:");
    scanf("%d",&number);
    if(number >= 10 && number <=99){
        int ones_digit = number % 10;
        printf("The one's digit of %d is: %d\n",number,ones_digit);
    }else{
        printf("Error:Please enter a valid two-digit number.\n");
    }
    return 0;
}
--------------------------------------------------------------------------
PROGRAM 7:
#include<stdio.h>
int main()
{
    int number;
    printf("Enter a two-digit number:");
    scanf("%d",&number);
    if(number >= 10 && number <=99){
        int tens_digit = number / 10;
        printf("The ten's digit of %d is: %d\n",number,tens_digit);
    }else{
        printf("Error:Please enter a valid two-digit number.\n");
    }
    return 0;
}
--------------------------------------------------------------------------
PROGRAM 8:

#include<stdio.h>
int main()
{
    int number;
    printf("Enter a two-digit number:");
    scanf("%d",&number);
    if(number >= 10 && number <=99){
        int tens_digit = number / 10;
        printf("The ten's digit of %d is: %d\n",number,tens_digit);
    }else{
        printf("Error:Please enter a valid two-digit number.\n");
    }
    return 0;
}
-----------------------------------------------------------------------------
PROGRAM 9:


#include<stdio.h>
int main()
{
    int number;
    printf("Enter a three-digit number:");
    scanf("%d",&number);
    if(number >= 100 && number <=999){
        int hundreds_digit = number / 100;
        printf("The hundreds's digit of %d is: %d\n",number,hundreds_digit);
    }else{
        printf("Error:Please enter a valid three-digit number.\n");
    }
    return 0;
}
-------------------------------------------------------------------
PROGRAM 10:

#include<stdio.h>
int main()
{
    int number;
    printf("Enter a three-digit number:");
    scanf("%d",&number);
    if(number >= 100 && number <=999){
        int hundreds = number / 100;
        int tens_digit = (number/10) % 10;    
        printf("The ten's digit of %d is: %d\n",number,tens_digit);
    }else{
        printf("Error:Please enter a valid three-digit number.\n");
    }
    return 0;
}
-------------------------------------------------------------------------
PROGRAM 11:

#include<stdio.h>
int main()
{
    int number,tens_digit,ones_digit,sum;
    printf("Enter a two-digit number:");
    scanf("%d",&number);
    if(number >= 10 && number <=99){
       tens_digit = number / 10;
       ones_digit = number % 10;
       sum = tens_digit + ones_digit;
        printf("The sum of the digits of %d is: %d\n",number,sum);
    }else{
        printf("Error:Please enter a valid two-digit number.\n");
    }
    return 0;
}
------------------------------------------------------------------------------
PROGRAM 12:

#include<stdio.h>
int main()
{
    int number,originalNumber,sum = 0;
    printf("Enter a three-digit number:");
    scanf("%d",&number);
    originalNumber = number;
    if(number >= 100 && number <=999){
    while(number!=0){
        int digit = number % 10;
        sum += digit;
        number /= 10;
    }
    printf("The sum of the digits of %d is: %d\n",originalNumber,sum);
    }else{
        printf("Error:Please enter a valid three-digit number.\n");
    }
    return 0;
}
------------------------------------------------------------------------
PROGRAM 13:

#include<stdio.h>
int main()
{
    int number,originalNumber,onesDigit,tensDigit;
    printf("Enter a two-digit number:");
    scanf("%d",&number);
    if(number >= 10 && number <=99){
        originalNumber = number;
        onesDigit = number % 10;
        number /= 10;
        tensDigit = number % 10;
        int reversedNumber = onesDigit*10 +tensDigit;
    printf("The reverse of %d is: %d\n",originalNumber,reversedNumber);
    }else{
        printf("Error:Please enter a valid two-digit number.\n");
    }
-------------------------------------------------------------------------
PROGRAM 14:

#include<stdio.h>
int main(){
    int number,originalNumber,reverseNumber = 0;
    printf("Enter a three-digit number:");
    scanf("%d",&number);
    if(number >= 100 && number <= 999){
        originalNumber = number;
        while(number !=0){
            int remainder = number % 10;
            reverseNumber = reverseNumber * 10 + remainder;
            number /= 10;
        }
        printf("The reverse of %d is: %d\n",originalNumber,reverseNumber);
    }else{
        printf("Error:Please enter a valid three-digit number.\n");
    }
    return 0;
}
----------------------------------------------------------------------------
PROGRAM 15:

#include<stdio.h>
int main(){
    int number,originalNumber,reversedFirstTwo;
    printf("Enter a four-digit number:");
    scanf("%d",&number);
    if(number >= 1000 && number <= 9999){
        originalNumber = number;
        int firstTwoDigits = number / 100;
        int lastTwoDigits = number % 100;
        int reversedTensUnits = (firstTwoDigits % 10)*10+(firstTwoDigits/10);
        reversedFirstTwo = reversedTensUnits * 100 +
        lastTwoDigits;
        printf("The number with reversed first two digits is:%d\n",reversedFirstTwo);
    }else{
        printf("Error:Please enter a valid four-digit number.\n");
    }
    return 0;
}
---------------------------------------------------------------------------------------------

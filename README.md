# space12
#include<stdio.h>
#include<conio.h>
void main()
{
long int decimal,remainder,quotient;
int binary[100],i=1,j;
clrscr();
printf("Enter any decimal number: ");
scanf("%ld",&decimal);
quotient = decimal;
while(quotient!=0){
binary[i++]= quotient % 2;
quotient = quotient / 2;
}
printf("Equivalent binary value of decimal number %d: ",decimal);
for(j = i -1 ;j> 0;j--)
printf("%d",binary[j]);
getch();
}

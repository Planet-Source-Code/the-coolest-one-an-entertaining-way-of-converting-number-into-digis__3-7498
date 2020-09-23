<div align="center">

## An entertaining way of converting number into digis


</div>

### Description

An entertaining way of converting number into digis
 
### More Info
 
just follow the comments placed along with the code

none so far


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[The Coolest one\.\.\.](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/the-coolest-one.md)
**Level**          |Beginner
**User Rating**    |4.3 (13 globes from 3 users)
**Compatibility**  |C, C\+\+ \(general\), Borland C\+\+
**Category**       |[Miscellaneous](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/miscellaneous__3-1.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/the-coolest-one-an-entertaining-way-of-converting-number-into-digis__3-7498/archive/master.zip)

### API Declarations

```
#include<stdlib.h>
#include<stdio.h>
#include<conio.h>
#include<dos.h>
#include<math.h>
```


### Source Code

```
/********An entertaining way of converting number into digis**********/
/*********************Tried and tested by-****************************/
/************************SUMIT THAWRANI*******************************/
/**********************sumit0001@yahoo.com****************************/
#include<stdlib.h>
#include<stdio.h>
#include<conio.h>
#include<dos.h>
#include<math.h>
void main()
{
unsigned long dig,temp; //I prefer unsigned int as their range is much larger
unsigned long div;   //Just make sure that the number u enter is
int num,i;       // lesser than 4294977295 or be prepared to get an
int count=0,c;     // awkward answer
void word(int);
clrscr();
printf("Enter the digit to be converted into words :");
scanf("%lu",&dig);
printf("\nThe number you entered is : %lu\n",dig);
printf("\nAnd this can be written in words as ..");
temp=dig;
while (temp!=0)
{ temp=temp/10;
 count++;       //counts the number of digits in the given number
 }
temp=dig;
for(i=count-1;i>=0;i--)
{ c=temp/pow(10,i);
  div=pow(10,i);
  temp=temp%div;
  sound(random(9999)); //plays different sound
  delay(400);   //introduces some delay
  word(c);     //call to function word() to print word
  nosound();
  c=0;
}
getch();
}
void word(int i)
{
switch(i){
case 1: printf(" One ");
	break;
case 2: printf(" Two ");
	break;
case 3: printf(" Three ");
	break;
case 4: printf(" Four ");
	break;
case 5: printf(" Five ");
	break;
case 6: printf(" Six ");
	break;
case 7: printf(" Seven ");
	break;
case 8: printf(" Eight ");
	break;
case 9: printf(" Nine ");
	break;
case 0: printf(" Zero ");
	break;
				}
return;
}
```


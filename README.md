# EX-16-LEFT-SHIFT-OPERATION
## AIM
To write a C Program to perform the basic left shift operation for 44 integer number with 3 shifts.

## ALGORITHM
1.	Start the program.
2.	Assign values of a and b as 44 and 3.
3.	Use left shift operator (<<) and shift the value of a three times.
4.	Display the result.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>
int main() {
    unsigned int a=44 ;	
      int c = 0; 
    c = a << 3;    
   printf("After Left Shift Operation value of a is:%d\n", c );
}
```
## OUTPUT

<img width="1038" height="185" alt="image" src="https://github.com/user-attachments/assets/2cc26194-8b31-480d-a334-d5fab11b4d83" />








## RESULT
Thus the program to perform the basic left shift operation for 44 integer number with 3 shifts has been executed successfully.




 
 


# EX-17-TWO-NUMBERS-ARE-EQUAL-OR-NOT


## AIM

Write a C Program to check whether the two numbers are equal or not using simple if statement.

## ALGORITHM

1.	Start the program.
2.	Read two numbers.
3.	If first number is equal to second number, display both are equal.
4.	Otherwise display both are not equal.
5.	Stop the program.

## PROGRAM
```
# include <stdio.h>
int main()
{
    int a,b;
    scanf("%d %d",&a,&b);
    if(a==b)
    {
        printf("Numbers are Equal");
    }
    else
    {
        printf("Numbers are not Equal");
    }
    return 0;
}
```

## OUTPUT
<img width="702" height="270" alt="image" src="https://github.com/user-attachments/assets/e9c1f24a-4184-4070-958b-8abc9a0fae82" />
           
## RESULT

Thus the program to check whether the two numbers are equal or not using simple if statement has been executed successfully
 
 


# EX-18-STRING-LOWERCASE-CONVERSION
## AIM
Write a C Program to convert the given string into lowercase.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using tolower( ) function convert the given string into its lowercase.
4.	Display the result.
5.	Stop the program.

## PROGRAM
```
#include<stdio.h>
#include<ctype.h>
#include<string.h>
int main()
{
    char str[100];
    scanf("%s",str);
    printf("Lower case String is:");
    for(int i=0;i<strlen(str);i++)
    {
        printf("%c",tolower(str[i]));
    }
}
```
## OUTPUT
<img width="782" height="227" alt="image" src="https://github.com/user-attachments/assets/166f7a6f-ade7-41f0-ae86-216f0065907a" />




## RESULT
Thus the program to convert the given string into lowercase has been executed successfully
 
 


# EX-19-COUNT-OF-WORDS-IN-A-STRING
## AIM
Write a C Program to count the total number of words in a given string using do While loop.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using for loop, inspect the string character by character.
4.	Whenever a space is encountered increment count by 1.
5.	Display the result.
6.	Stop the program.

## PROGRAM
```
#include<stdio.h>
#include<string.h>
#include<ctype.h>
int main()
{
    char str[1000];
    int i=0,count=0;
    scanf("%[^\n]s",str);
   do
   {
       if((str[i]!=' ' && str[i]!= '\t'&& str[i]!='\0') && (str[i+1]== ' ' || str[i+1]== '\t' || str[i+1]=='\0'))
       {
           count++;
       }
       i++;
   }while(str[i]!='\0');
   printf("%d\n",count);
}
```
## OUTPUT

<img width="612" height="215" alt="image" src="https://github.com/user-attachments/assets/90853e2c-64c3-49e0-9e5a-94df18879255" />




## RESULT
Thus the program to count the total number of words in a given string using do While loop has been executed successfully
 
 


# EX  -20 -COMPARING TWO STRINGS
## AIM
write a Program to compare two strings without using strcmp().
## ALGORITHM
Step 1: Start the program.
Step 2: Declare two character arrays c1 and c2 of size 100 to store the strings. Also, declare an integer variable
             flag and initialize it to 0, and i for indexing.      
Step 3: Read the first string c1 using scanf("%[^\n]", c1); — this reads input until a newline is encountered 
            (i.e., can include spaces).
Step 4: Read the second string c2 using scanf("%s", c2); — this reads input until a space or newline (i.e., no 
            spaces in the second string).
Step 5: Start comparing characters of both strings from index i = 0.
Step 6: Repeat the following while neither c1[i] nor c2[i] is '\0' (i.e., end of string):
•	If c1[i] is not equal to c2[i], set flag = 1.
•	Increment i by 1.
Step 7: After the loop, check the value of flag:
•	If flag == 0, print "strings are same".
•	Otherwise, print "strings are not same".
Step 8: End the program.

## PROGRAM
```
# include <stdio.h>
int main()
{
    char str1[100],str2[100];
    int i=0,str=1;
    scanf("%s",str1);
    scanf("%s",str2);
    while(str1[i]!='\0' || str2[i] != '\0')
    {
        if(str1[i]!=str2[i])
        {
            str=0;
            break;
        }
        i++;
    }
    if(str)
    {
        printf("strings are same\n");
    }
    else
    {
        printf("strings are not same\n");
    }
    return 0;
}
```

## OUTPUT
 <img width="684" height="259" alt="image" src="https://github.com/user-attachments/assets/447f812b-f7ea-4590-80a8-a72b900d3942" />


## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.


# EX-11-EMI-CALCULATOR

## AIM

To write a program to prepare EMI calculator using function without return type and with arguments.

## ALGORITHM

1.	Start the program.
2.	Read principal amount, rate of interest and months.
3.	Pass these values as arguments to function.
4.	Calculate EMI using the formula, amt=(prpow(1+r,t))/(pow(1+r,t)-1)
5.	Display the result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>
#include <math.h>
float emi(float amt, float rate, float year){
    float a;
    rate/=(12*100);
    year*=12;
    a = (amt * rate * pow((1+rate),year))/(pow((1+rate),year)-1);
    return a;
}
int main(){
    float a=251000, c=5;
    float b=8.5;
    printf("Monthly EMI is= %.3f",emi(a,b,c));
}
```
## OUTPUT
![image](https://github.com/user-attachments/assets/df54a03d-9574-4b73-a41d-4f0571c1d3e1)





## RESULT

Thus the program to prepare EMI calculator using function without return type with arguments has been executed successfully
 
 


# EX-12-FIBONACCI-SERIES
## AIM
To write a C program to generate the Fibonacci series for the value 6.

## ALGORITHM
1.	Start the program.
2.	Read number of terms to display.
3.	Add the previous two terms and store it in new term.
4.	Assign 2nd term to 1st term and 3rd term to 2nd term.
5.	Repeat steps 3 and 4 n number of times.
6.	Display the result.
7.	Stop the program.

## PROGRAM
```
#include <stdio.h>
int main(){
    int n=6,a=0,b=1,c=0;
    printf("%d ",a);
    printf("%d ",b);
    while(n>0){
        c=a+b;
        printf("%d ",c);
        a=b;
        b=c;
        n--;
    }
}
```
## OUTPUT
![image](https://github.com/user-attachments/assets/52e62852-450a-4dd1-b56e-0393cedca5fd)








## RESULT
Thus the program to generate the Fibonacci series for the value 6 has been executed successfully.
 
 


# EX-13-ONE-DIMENSIONAL-ARRAY
## AIM
To write a C program to read n elements as input and print the last element of the array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	Print the last element.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main()
{
    int n;
    scanf("%d",&n);
    int a[n];
    for(int i=0;i<n;i++)
    {
        scanf("%d",&a[i]);
}
        printf("%d ",a[n-1]);

    return 0;
}
```
## OUTPUT
![image](https://github.com/user-attachments/assets/10c360c5-3abc-49ed-8743-b868e600bd86)









## RESULT
Thus the program to read n elements as input and print the last element of the array has been executed successfully.
 
 


# EX-14-POSITIVE-ARRAY-ELEMENTS
## AIM
To write a C Program to count total number of positive elements in an array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	If the array value can be divided by 2 then increment count by 1.
5.	Display result.
6.	Stop the program.

## PROGRAM
```
#include<stdio.h>
int main()
{
    int n,i;
    scanf("%d",&n);
    int arr[n],p=0,n=0;
    for (i=0;i<n;i++)
    {
        scanf("%d",&arr[i]);
        if (arr[i]>0) p++;
        else n++;
    }
    printf("count  of positive numbers  in array: %d\n",p);
    printf("count  of negative numbers  in array: %d",n);
}
```

## OUTPUT
![image](https://github.com/user-attachments/assets/ced9f1e3-c3ad-402c-8d00-3d2991f235ab)




## RESULT
Thus the program to count total number of positive elements in an array has been executed successfully.





 
 


# EX -15 - Replace All Even Elements With 'E' In One Dimensional Array

## Aim:
To write a C program to replace all even elements with 'E' in one dimensional array

## Algorithm:
1.	Input the array:
  Read the size of the array.
  Input the elements of the array.
2.	Iterate through the array:
 	For each element of the array, check if the element is even (i.e., if the element modulo 2 equals 0).
3.	Replace even elements with 'E':
     If an element is even, replace that element with the character 'E'.
4.	Output the updated array:
 Print the updated array after replacements.

## Program:
```
#include <stdio.h>

int main() {
    int n;
    scanf("%d", &n);

    int arr[n];
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    for (int i = 0; i < n; i++) {
        if (arr[i] % 2 == 0) {
            arr[i] = 'E';
        }
    }

    for (int i = 0; i < n; i++) {
        if (arr[i] == 'E') {
            printf("E ");
        } else {
            printf("%d ", arr[i]);
        }
    }

    return 0;
}
```
## Output:
![image](https://github.com/user-attachments/assets/8f236879-870c-496e-af9e-209acd090f8e)



## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.




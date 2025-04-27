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
void calculateEMI(float principal, float annualRate, int months) {
    float monthlyRate = annualRate / (12 * 100); 
    float emi;
    emi = (principal * monthlyRate * pow(1 + monthlyRate, months)) / (pow(1 + monthlyRate, months) - 1);
    printf("Monthly EMI is: %.2f\n", emi);
}
int main() {
    float principal, rate;
    int months;
    printf("Enter loan amount (principal): ");
    scanf("%f", &principal);
    printf("Enter annual interest rate (in %%): ");
    scanf("%f", &rate);
    printf("Enter loan tenure (in months): ");
    scanf("%d", &months);
    calculateEMI(principal, rate, months);
    return 0;
}
```


## OUTPUT
![image](https://github.com/user-attachments/assets/8c01fd77-d839-472b-b11d-d825159a8732)






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
#include<stdio.h>
int main()
{
    int i,a=0,b=1,t,n;
    scanf("%d",&n);
    printf("%d %d ",a,b);
    for(i=2;i<n;i++)
    {
        t=a+b;
        printf("%d ",t);
        a=b;
        b=t;
    }
    
    
}
```

## OUTPUT
![image](https://github.com/user-attachments/assets/98198f0d-33b4-44a7-80ee-eb74d1c6d3d4)








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
#include<stdio.h>
int main()
{
    int n,i;
    scanf("%d",&n);
    int a[n];
    for(i=1;i<=n;i++)
    {
        scanf("%d",&a[i]);
    }
    printf("%d",a[n]);
    return 0;
}
```

## OUTPUT
![image](https://github.com/user-attachments/assets/2d3304a2-d120-480f-a941-1b14c6e83208)










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
#include <stdio.h>
int main() {
    int arr[100], n, count = 0;
    printf("Enter the number of elements in the array: ");
    scanf("%d", &n);
    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    for (int i = 0; i < n; i++) {
        if (arr[i] > 0) {
            count++;
        }
    }
    printf("Total number of positive elements = %d\n", count);
    return 0;
}
```


## OUTPUT
![image](https://github.com/user-attachments/assets/6ee67cdf-6e4e-4f54-9c86-d84eff8a3832)






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
    int arr[100], n;
    char result[100];
    printf("Enter number of elements: ");
    scanf("%d", &n);
    printf("Enter %d integer elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    for (int i = 0; i < n; i++) {
        if (arr[i] % 2 == 0) {
            result[i] = 'E';
        } else {
            result[i] = '-';  
        }
    }
    printf("Modified output (even elements replaced with 'E'):\n");
    for (int i = 0; i < n; i++) {
        if (result[i] == 'E') {
            printf("E ");
        } else {
            printf("%d ", arr[i]);
        }
    }
    return 0;
}
```

## Output:
![image](https://github.com/user-attachments/assets/e438a731-e613-4049-b154-655dc1a73fd6)

 


## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.




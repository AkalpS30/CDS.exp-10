# CDS.exp-10
## Aim:
**To study and implement Pointer Operations (Call by value and Call by reference)..**

## Software:
`Microsoft VSCode`

## Theory:
Pointers are symbolic representations of addresses.
We can pass arguments to funtions using different methods mainly call by value and call by reference.

Call by value
In the call-by-value method, function arguments are passed by copying the value of the actual parameter, ensuring the original values remain unchanged.
The value is copied to the formal parameter.
Any changes made to the parameters within the function do not change the original values outside the function.

Call by reference
In the call-by-reference method, the memory address (reference) of the actual parameter is passed to the function, allowing direct access and modification of the original values.
The actual and the formal parameters point to the same memory address.

Any changes made to the parameters within the function are directly reflected in the original values outside the function.
## Code: 10A
```
//AKALP SARKAR
//ENTC B2
//EXP 10A
//23070123116
// // Printing the values by using callby value 

#include<iostream> 
using namespace std; 
void swap(int x, int y) 
{
    int swap;
    swap=x;
    x=y;
    y=swap;
}

int main() 
{
    int a=4, b=7;
    swap(a,b);
    cout<<"Value of a is: "<<a<<"\n";
    cout<<"Value of b is: "<<b<<"\n";
    return 0;
}
```
## Output:
![10A](https://github.com/user-attachments/assets/208a5464-3356-4bf4-b059-94a82e313a13)

## Code: 10B
```
//AKALP SARKAR
//ENTC B2
//EXP 10B
//23070123116
// Swapping the values 

#include<iostream> 
using namespace std; 
void swap(int *x, int *y) 
{
    int *swap;
    swap=x;
    x=y;
    y=swap;
}

int main() 
{
    int a=4,b=7;
    swap(a,b);
    cout<<"Value of a is: "<<a<<"\n";
    cout<<"Value of b is: "<<b<<"\n";
    return 0;
} 
```
## Output:
![10b](https://github.com/user-attachments/assets/1e1417d5-5cb6-4305-a0fc-e45ae0da92ea)

## Code:10C
```
//AKALP SARKAR
//ENTC B2
//EXP 10C
//23070123116
// Swapping the values using call by reference  

#include<iostream> 
using namespace std; 
void swap(int *x, int *y) 
{
    int swap;
    swap=*x;
    *x=*y;
    *y=swap;
}

int main() 
{
    int a=4,b=7;
    swap(&a,&b);
    cout<<"Value of a is: "<<a<<"\n";
    cout<<"Value of b is: "<<b<<"\n";
    return 0;
}
```
## Output:
![Output3](https://github.com/user-attachments/assets/08480b79-b810-4ab2-b5a0-9ec6f9014e6b)!

### Conclusion:
I learnt about pointers and how to pass arguments to functions using call by value and call by reference methods. I also learnt how to swap values using call by reference.


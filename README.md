# AIM
To learn about exception handling in c++.

# Problem Statement

1.) Write a c++ program to get a customized error for entering a negative number.

2.) Write a c++ program to get a customized error for entering a year less than 2000.

# Theory

In C++, exceptions are runtime anomalies or abnormal conditions that a program encounters during its execution. The process of handling these exceptions is called exception handling. Using the exception handling mechanism, the control from one part of the program where the exception occurred can be transferred to another part of the code.

So basically using exception handling in C++, we can handle the exceptions so that our program keeps running.

# Problem Codes

```javascript

//NEGATIVE NUMBER ERROR
# include<iostream>
using namespace std;
 int main()
 {  float a;
    cout<< "Enter a positive  numbers: "<<endl;
    cin>>a;

try {
    if ( a<0)
    {
        throw a;
    }
else {
 cout<< "The number  is: "<<a<<endl;
 }
}
catch (const float n)
{
    cout<<"You entered " <<a<<" which is a negative number"<<n;
}
 }

//YEAR LESS THAN 2000
# include<iostream>
using namespace std;
 int main()
 { int year;
    cout << "Enter year greater than 2000: "<<endl;
    cin>>year;

    try{
if ( year<2000)
{
    throw "You entered a year less than 2000";

}
else{
    cout<< "Entered year is: "<<year<<endl;
}
    }

    catch ( const char*msg)

    { 
        cout << msg;

    }
 }

```
# Output
## Negative Number Error
![Exp 16-positive number](https://github.com/user-attachments/assets/8e09e0bc-b984-4f5c-8f22-35c67a9f7643)
![Exp 16 - positive num](https://github.com/user-attachments/assets/d7a886f4-3f75-4bd0-add9-95670f95bea1)

## Year Exception
![exp 16 - Year 2](https://github.com/user-attachments/assets/9cc0a146-8665-4cd0-b27b-12ef43840a7c)
![Exp 16 - Year 1](https://github.com/user-attachments/assets/553c7f2c-2290-4c91-91ae-4c7f9bd68ab4)

# Conclusion

We learnt to use exception handling in c++.

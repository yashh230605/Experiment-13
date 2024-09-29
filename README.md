# Experiment 13



## Aim:
To study and implement constructor overloading


## Apparatus:
Vs Code, Github


## Theory:

### How Constructor Overloading Works in C++:

1:When an object is created, the C++ compiler checks the arguments provided and chooses the constructor that matches the argument list.

2:If no arguments are passed, the default constructor is called.

3:If arguments are passed, the constructor with the matching parameters is called.

### Rules for Constructor Overloading in C++:

1:Different Signatures: Each overloaded constructor must have a different signature (i.e., a different set of parameters).

2:No Return Type: Like all constructors, overloaded constructors do not have a return type, not even void.

3:Same Name: All constructors must have the same name as the class name.

### Characteristics of constructor overloading:

Sure, here is the definition of Constructor Overloading broken down into points:

1:Multiple Constructors: Constructor overloading allows a class to have more than one constructor, each with a different set of parameters.

2:Different Parameter Lists: The constructors must have different parameter lists, which can vary by the number, type, or order of parameters.

3:Automatic Selection: When an object is instantiated, the compiler automatically selects the appropriate constructor based on the arguments provided.

4:Flexible Initialization: Overloaded constructors allow for different ways to initialize an object, depending on the data available at the time of creation.

5:Same Name: All overloaded constructors must share the same name as the class, just like any other constructor.

6:No Return Type: Like all constructors, overloaded constructors do not have a return type.

7:Enhanced Versatility: Constructor overloading makes the class more versatile, allowing for more flexible object creation.

### Advantages of Constructor Overloading in C++:

1: Flexibility: Allows the class to be instantiated in multiple ways, depending on the available data.

2: Ease of Use: Users can initialize objects with different sets of data conveniently.

3: Improved Readability: Makes the code more readable by clearly defining how objects can be created.


## Code:

```
# include<iostream>
using namespace std;

class room
{
    private:
    double l,b;

    public:
    room()
    {
        l = 1.2;
        b = 2.3;
    }
    room(double len, double bre)
    {
        l = len;
        b = bre;
    }
    room(double len)
    {
        l = len;
        b = 4.5;
    }
    double area()
    {
        return l*b;
    }

};
int main()
{
    room r1,r2(6.7,7.8),r3(9.1);
    cout<<"No parameter passed: "<<endl;
    cout<<"Area: "<<r1.area()<<endl;
    cout<<"Two parameters passed: "<<endl;
    cout<<"Area: "<<r2.area()<<endl;
    cout<<"One parameter passed: "<<endl;
    cout<<"Area: "<<r3.area()<<endl;
}
```
### Output:
No parameter passed: 
Area: 2.76
Two parameters passed: 
Area: 52.26
One parameter passed: 
Area: 40.95


## Conclusion:
This program helps us understand how constructor overloading.# Experiment-13

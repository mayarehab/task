# **The Usage of Const keyword and & operator**
##**A. The use of const keyword** 

###_1. Variables:_ 
constant variable means that you can not change its value and it must be initialized while declaration. When const is used it tells the compiler to prevent the programmer from modifying it.

_Example:_
~~~cpp
int main(){
    const float pi = 3.14;
    const float e = 2.71;
    pi= 4; //error
    e++; //error
}
~~~
###_2. Pointers with const keyword:_
We can declare pointers using const keyword in two ways:

**1st way** is to declare pointer to a constant variable. As a result, we can make any array or string unchangeable.

_Example 1_ 
~~~cpp
int main(){
    const float *u = 11.5;  //pointer u points to const float variable
    const char *z = 'a' ;  //pointer z points to const char variable
    *u = 4.9; // error
 }
~~~
**2nd way** is to make the pointer itself constant which means that the pointer will always point to the same memory address no matter what is the value.

_Example 2_
~~~cpp
int n = 10;
int *ptr1;
int *const ptr = &n; // pointer ptr will always point to the location of variable n
*ptr = 6; //accepted
ptr=ptr1; //error
~~~
###_3. Constant Function arguments and return types:_
We can make the function arguments and return types constant.

Example
~~~cpp
void f(const int i)
{
    i++;    // error
}

const int g()
{
    return 1;
}
~~~
### _4. Constant Class Data members:_
We can define some data members as const. They are not initialized during declaration. Their initialization is done in the constructor.

_Example_
~~~cpp
class Trial
{
    const int i;
    public:
    Test(int x):i(x)
    {
        cout << "\ni value set: " << i;
    }
};

int main()
{
    Test t(10);
    Test s(20);
}
~~~
###_5. Class Member functions:_
A const member functions never modifies data members in an object.

Example
~~~cpp
// constant_member_function.cpp
class Date
{
public:
Date( int mn, int dy, int yr );
int getMonth() const;     // A read-only function
void setMonth( int mn );   // A write function; can't be const
private:
int month;
};

int Date::getMonth() const
{
return month;        // Doesn't modify anything
}
void Date::setMonth( int mn )
{
month = mn;          // Modifies data member
}
int main()
{
Date MyDate( 7, 4, 1998 );
const Date BirthDate( 1, 18, 1953 );
MyDate.setMonth( 4 );    // Okay
BirthDate.getMonth();    // Okay
BirthDate.setMonth( 4 ); // C2662 Error
}
~~~
###_6. Objects:_
The data members of the object can never be changed, during the object's lifetime, when the object is declares as const.

Example
~~~cpp
const class_name object;
~~~
      
      


##**B. The use of & operator**
###_1. Bitwise and opreator:_ 
It compares each bit of the first operand with each bit of the second operand.If both bits are 1, the bit is set to 1. If not the bet is set to zero.
_Example:_
~~~cpp
int main () {
  int a = 6; //6=110
  int b = 7; //7=111
  cout<<(a&b); //a&b=110 
}
~~~
###_2. Address of operator:_ 
It returns the address of the pointer (variable).
_Example:_
~~~cpp
int main(){
   int x;
   int *ptr;
   x=6;
   ptr=&x; // it will return the address of variable x
   cout<<ptr; 
}
~~~

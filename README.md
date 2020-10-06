#include <iostream>
#include <cmath>
using namespace std;

int main()
{
    int a, b, c, x, x1, x2, discriminant;
    cout<<"Please enter the quadratic coefficient: ";
    cin>>a;
    cout<<"Please enter the linear coefficient: ";
    cin>>b;
    cout<<"Please enter the constant: ";
    cin>>c;

    discriminant = (b*b - 4*a*c); /*Discriminant formula in quadratic equation*/

    if(discriminant<0)
    {
        cout<<"There are no real solutions of the equation."<<endl;
    }

    else if(discriminant==0)
    {
        x = ( -b ) / (2 * a);
        cout<<"There is only one real solution, which is equal to: "<<x<<endl;
    }

    else if(discriminant>0)
    {
        x1 = ((( -b ) + sqrt(discriminant)) / 2*a ); /*Quadratic formula for the first solution*/
        x2 = ((( -b ) - sqrt(discriminant)) / 2*a ); /*Quadratic formula for the second solution*/
        cout<<"The first real solution of the equation is: "<<x1<<endl;
        cout<<"The second real solution of the equation is: "<<x2<<endl;
    }

 return 0;
}


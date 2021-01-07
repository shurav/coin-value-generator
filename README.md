# coin-value-generator
This program will allow users to test if their number of coins equals their intended value

#include <iostream>
using namespace std;

int main()
{
    int pennies, nickels, dimes, quarters;
    float price;
    cout << "This program will allow you to see if the number of coins you have equals your desired price" << endl;
    cout << "What is your price?" << endl;
    cin >> price;
    cout << "Enter the number of pennies: " << endl;
    cin >> pennies;
    cout << "Enter the number of nickels: " << endl;
    cin >> nickels;
    cout << "Enter the number of dimes: " << endl;
    cin >> dimes;
    cout << "Enter the number of quarters: " << endl;
    cin >> quarters;
    float usertotal = .01*pennies+.05*nickels+.1*dimes+.25*quarters;
    if(usertotal==price)
    {
        cout << "congratulations, the value of your coins is " << usertotal << " and equals your intended amount" << endl;
    }
    else if (usertotal<price)
    {
        cout << "your amount is " << usertotal << " and is less than " << price << endl;
    }
    else
    {
        cout << "your amount is " << usertotal << " and is more than " << price << endl;
    }
    return 0;
}

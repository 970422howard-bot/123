 //Generating the Multiplication Table
#include <iostream>
#include <iomanip> //Header providing parametric manipulators
using namespace std;

int main(void)
{
    unsigned int i, j;
    cout << " X|";

    //Generation the top header line of the multiplication table
    for (j = 1; j <= 9; cout << setw(5) << j << "|", j++)
        ;

    cout << "\n------------------------------------------------";
    for (i = 1; i <= 9; i++)
    {
        cout << "\n " << i << "|";

        //Compute i*j and display in the form with the width of 5 characters
        for (j = 1; j <= 9; cout << setw(5) << i * j << "|", j++)
            ;
    }

    cout << "\n";
    return 0;
}

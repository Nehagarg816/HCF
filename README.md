# HCF
This is a program for finding hcf of two numbers in c++.


#include <stdio.h>
#include <iostream>
using namespace std;

int main()
{
    int n1, n2, hcf, t;
    std::cout << "Enter one number n1:";
    cin >> n1;
    std::cout << "Enter second number n2:";
    cin >> n2;
    if (n2 > n1)
    {
        t = n1;
        n1 = n2;
        n2 = t;
    }
    for (int i = 1; i <= n2; i++)
    {
        if (n1 % i == 0 && n2 % i == 0)
        {
            hcf = i;
        }
    }
    std::cout << "HCF is " << hcf << std::endl;

    return 0;
}

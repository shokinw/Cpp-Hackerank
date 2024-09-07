# Cpp-Hackerank
**1st code that I successfully run**
int main() {
    
    /* Enter your code here. Read input from STDIN. Print output to STDOUT */   
    int a;
    int b;
    int c;
    cin>>a>>b>>c;
    cout<<a+b+c<<endl;
    return 0;
}
+__________________________________________________________________________________
#include <iostream>
#include <cstdio>
#include<iomanip>
using namespace std;

int main() {
    // Complete the code.
    int n;
    long l;
    char ch;
    float f;
    double d;
    
    cin>> n >>l>>ch>>f>>d;
    cout<<n<<endl;
    cout<<l<<endl;
    cout<<ch<<endl;
    
    cout<<fixed<<setprecision(3)<<f<<endl;
    cout<<fixed<<setprecision(5)<<d<<endl;
    return 0;
}

+__________________________________________________________________________________
#include <bits/stdc++.h>

using namespace std;

string ltrim(const string &);
string rtrim(const string &);



int main()
{
    string n_temp;
    getline(cin, n_temp);

    int n = stoi(ltrim(rtrim(n_temp)));

        
    // Check if n is between 1 and 9 inclusive
    if (n >= 1 && n <= 9) {
        switch (n) {
            case 1: cout << "one" << endl; break;
            case 2: cout << "two" << endl; break;
            case 3: cout << "three" << endl; break;
            case 4: cout << "four" << endl; break;
            case 5: cout << "five" << endl; break;
            case 6: cout << "six" << endl; break;
            case 7: cout << "seven" << endl; break;
            case 8: cout << "eight" << endl; break;
            case 9: cout << "nine" << endl; break;
        }
    } else {
        cout << "Greater than 9" << endl;
    }

    return 0;**
}


string ltrim(const string &str) {
    string s(str);

    s.erase(
        s.begin(),
        find_if(s.begin(), s.end(), not1(ptr_fun<int, int>(isspace)))
    );

    return s;
}

string rtrim(const string &str) {
    string s(str);

    s.erase(
        find_if(s.rbegin(), s.rend(), not1(ptr_fun<int, int>(isspace))).base(),
        s.end()
    );

    return s;
}

+__________________________________________________________________________________


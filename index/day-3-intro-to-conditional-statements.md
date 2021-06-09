# Day 3: Intro to Conditional Statements

### Problem Link <a id="problem"></a>

* [x] [**HackerRank Problem Link**](https://www.hackerrank.com/challenges/30-conditional-statements/problem)\*\*\*\*

### Solution

* [x] **In C++ Language**

{% code title="Conditional\_Statements.cpp" %}
```cpp
#include <bits/stdc++.h>

using namespace std;

int main()
{
    int Num;
    cin >> Num;
    cin.ignore(numeric_limits<streamsize>::max(), '\n');
    
    // Complete the solve function below.
    
    if(Num%2 == 0)
    {
        if(Num>=2 && Num<=5)
        {
            cout<<"Not Weird";
        }
        else if(Num>=6 && Num<=20)
        {
            cout<<"Weird";
        }    
        else
        {
            cout<<"Not Weird";
        }
    }
    else
        cout<<"Weird";
    return 0;
}

```
{% endcode %}


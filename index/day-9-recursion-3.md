# Day 9: Recursion 3

### Problem Link <a id="problem"></a>

* [x] [**HackerRank Problem Link**](https://www.hackerrank.com/challenges/30-recursion/problem)\*\*\*\*

### Solution

* [x] **In C++ Language**

{% code title="Recursion.cpp" %}
```cpp
#include <bits/stdc++.h>

using namespace std;

int factorial(int num) ;

int main() 
{

    int n;
    cin >> n;
    cout << factorial(n) << endl;

    return 0;
}

int factorial(int num) 
{
    if(num == 1)
    {
        return 1;
    }
    else 
    {
    return (num * (factorial(num-1)));
    }
}

```
{% endcode %}


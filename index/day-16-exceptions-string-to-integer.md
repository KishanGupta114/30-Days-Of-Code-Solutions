# Day 16: Exceptions - String to Integer

### Problem Link <a id="problem"></a>

* [x] [**HackerRank Problem Link**](https://www.hackerrank.com/challenges/30-exceptions-string-to-integer/problem)\*\*\*\*

### Solution

* [x] **In C++ Language**

{% code title="StoI.cpp" %}
```cpp
#include <bits/stdc++.h>

using namespace std;

int main()
{
    string S;   
    cin >> S;
    
    int n;

    try
    {
        n=stoi(S);
        cout<<n<<endl;
    }
    catch(exception e)
    {
        cout<<"Bad String";
    }
    return 0;
}

```
{% endcode %}


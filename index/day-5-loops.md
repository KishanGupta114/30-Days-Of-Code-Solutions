# Day 5: Loops

### Problem Link <a id="problem"></a>

* [x] [**HackerRank Problem Link**](https://www.hackerrank.com/challenges/30-loops/problem)\*\*\*\*

### Solution

* [x] **In C++ Language**

{% code title="Loops.cpp" %}
```cpp
#include <bits/stdc++.h>

using namespace std;

int main()
{
    int num;
    cin >> num;
    cin.ignore(numeric_limits<streamsize>::max(), '\n');
    
    if(2<=num<=20)
    {
        for (int i = 1; i <= 10; i++) 
        {
            cout <<num<<" "<<"x"<<" "<<i<<" "<<"="<<" "<<(num*i)<< endl;
        }
    }
    return 0;
}

```
{% endcode %}


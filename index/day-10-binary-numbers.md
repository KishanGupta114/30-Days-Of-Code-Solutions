# Day 10: Binary Numbers

### Problem Link <a id="problem"></a>

* [x] [**HackerRank Problem Link**](https://www.hackerrank.com/challenges/30-binary-numbers/problem)\*\*\*\*

### Solution

* [x] **In C++ Language**

{% code title="Binary\_Num.cpp" %}
```cpp
#include <bits/stdc++.h>

using namespace std;

int main()
{
    int n,count=0,max=0;
    cin >> n;

    while(n)
    {
        if (n&1)
            count++;
        else 
            count = 0;
        if (max < count)
            max = count;
        n>>=1;
    }
    cout << max;

    return 0;
}

```
{% endcode %}


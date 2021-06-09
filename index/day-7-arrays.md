# Day 7: Arrays

### Problem Link <a id="problem"></a>

* [x] [**HackerRank Problem Link**](https://www.hackerrank.com/challenges/30-arrays/problem)\*\*\*\*

### Solution

* [x] **In C++ Language**

{% code title="Arrays.cpp" %}
```cpp
#include <bits/stdc++.h>

using namespace std;

int main()
{

 int n;
 cin >> n;

 vector<int> arr(n);

 for(int arr_i = 0;arr_i < n;arr_i++)
{
       cin >> arr[arr_i];
}

for(int arr_i = n-1;arr_i >= 0;arr_i--)
{
       cout << arr[arr_i]<<" ";
}
    return 0;
}

```
{% endcode %}


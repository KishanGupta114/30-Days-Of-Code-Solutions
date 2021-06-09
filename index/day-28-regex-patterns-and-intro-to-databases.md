# Day 28: RegEx, Patterns, and Intro to Databases

### Problem Link <a id="problem"></a>

* [x] [**HackerRank Problem Link**](https://www.hackerrank.com/challenges/30-regex-patterns/problem)\*\*\*\*

### Solution

* [x] **In C++ Language**

{% code title="RegEx\_Patterns\_Intro2Databse.cpp" %}
```cpp
#include <bits/stdc++.h>
using namespace std;

int main()
{
    int N, i;

    cin >> N;

    regex exp(".+@gmail\\.com$");

    vector<string> strarray;

    for(i = 0; i < N; i++)
 {
        string Fname;

        string Eid;

        cin >> Fname >> Eid;

        if(regex_match(Eid, exp))
 {
            strarray.push_back(Fname);
        }
    }

    sort(strarray.begin(), strarray.end()); 

    for(i = 0; i < strarray.size();i++) 
    { 
        cout << strarray[i] << endl; 
    }

    return 0;
}

```
{% endcode %}


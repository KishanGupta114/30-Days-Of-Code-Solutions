# Day 17: More Exceptions

### Problem Link <a id="problem"></a>

* [x] [**HackerRank Problem Link**](https://www.hackerrank.com/challenges/30-more-exceptions/problem)\*\*\*\*

### Solution

* [x] **In C++ Language**

{% code title="More\_Exceptions.cpp" %}
```cpp
#include <cmath>
#include <iostream>
#include <exception>
#include <stdexcept>
using namespace std;

class Calculator 
{
    public:
    int power(int first, int second) 
    {
        if(first < 0 || second < 0) 
        {
           throw runtime_error("n and p should be non-negative");
        }
        return pow(first, second);
    }
};

int main()
{
    Calculator myCalculator=Calculator();
    int T,n,p;
    cin>>T;
    while(T-->0){
      if(scanf("%d %d",&n,&p)==2){
         try{
               int ans=myCalculator.power(n,p);
               cout<<ans<<endl; 
         }
         catch(exception& e){
             cout<<e.what()<<endl;
         }
      }
    }
    
}
```
{% endcode %}


# Day 13: Abstract Classes

### Problem Link <a id="problem"></a>

* [x] [**HackerRank Problem Link**](https://www.hackerrank.com/challenges/30-abstract-classes/problem)\*\*\*\*

### Solution

* [x] **In C++ Language**

{% code title="Abstract\_cls.cpp" %}
```cpp
#include <cmath>
#include <cstdio>
#include <vector>
#include <iostream>
#include <algorithm>
#include <string>
using namespace std;
class Book{
    protected:
        string title;
        string author;
    public:
        Book(string t,string a){
            title=t;
            author=a;
        }
        virtual void display()=0;

};


//Write MyBook class
class MyBook : public Book {
  public:
    MyBook(
        string t,
        string a,
        int p
    ) :
        Book(t,a),
        price(p)
    {
        
    }
    
    virtual
    void
    display(
        void
    ) override {
        cout << "Title: " << title << endl;
        cout << "Author: " << author << endl;
        cout << "Price: " << price << endl;
    }
    
  private:
    int price;
};

int main() {
    string title,author;
    int price;
    getline(cin,title);
    getline(cin,author);
    cin>>price;
    MyBook novel(title,author,price);
    novel.display();
    return 0;
}

```
{% endcode %}


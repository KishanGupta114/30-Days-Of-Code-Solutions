# Day 14: Scope

### Problem Link <a id="problem"></a>

* [x] [**HackerRank Problem Link**](https://www.hackerrank.com/challenges/30-scope/problem)\*\*\*\*

### Solution

* [x] **In Python Language**

{% code title="Scope.py" %}
```python
class Difference:
    def __init__(self, a):
        self.__elements = a

	# Add your code here
    def computeDifference(self):
        maximum = 0

        for i in range(len(self.__elements)):
            for j in range(len(self.__elements)):
                absolute = abs(self.__elements[i] - self.__elements[j])
                if absolute > maximum:
                    maximum = absolute

        self.maximumDifference = maximum
# End of Difference class

_ = input()
a = [int(e) for e in input().split(' ')]

d = Difference(a)
d.computeDifference()

print(d.maximumDifference)
```
{% endcode %}


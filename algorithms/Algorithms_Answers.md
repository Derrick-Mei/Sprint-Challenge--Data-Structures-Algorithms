Add your answers to the Algorithms exercises here.

1. Exercise 1
    1. O(n)
    2. O(log n)
    3. O(log sqrt(n**2)) ???
        1. if n > 128, sum does not increase further
    4. O(n * log(n))
    5. O(n * n-1 * n-2 * n+7) = O(n^4)
    6. O(n)
    7. O(n)

2. Exercise 2
``` python
```

```python

will_it_break(floorLevels, criticalLevel):
    while floorLevels > criticalLevel:
        floorLevels / 2

Basically keep halving the floor levels.  This would be a log complexity.


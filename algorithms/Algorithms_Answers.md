Add your answers to the Algorithms exercises here.

1. Exercise 1
    1. O(n)
    2. O(log n)
    3. O(log sqrt(n**2)) ???
        1. if n > 128 128 aka 8^2/2, sum does not increase further
    4. O(n * log(n))
    5. O(n * n-1 * n-2 * n+7) = O(n^4)
    6. O(n)
    7. O(n)

2. Exercise 2
``` python
def biggest_difference(arr):
    max_diff = arr[1] - arr[0]
    min_element = arr[0]

    for i in range(i, len(arr)):
        if arr[i] - min_element > max_diff:
            max_diff = arr[i] - min_element
        if arr[i] < min_element:
            min_element = arr[i]
    return max_diff
```

```python
def will_it_break(floorLevels, criticalLevel):
    if floorLevels > criticalLevel:
        
    while floorLevels > criticalLevel:
        floorLevels / 2
```

Basically test the egg at top level.  If it breaks, test at middle.  This would elimintate half the choices. Then keep testing at the halfway points until you get 2 remaining.  Log time complexity


3. Excercise 3
    a) O(n^2) - quick sort is recursively called to all items in the array
    b) O(log (n^2)) - each iteration is splits the array evenly and fewer loops are called but each cycle is still a loop



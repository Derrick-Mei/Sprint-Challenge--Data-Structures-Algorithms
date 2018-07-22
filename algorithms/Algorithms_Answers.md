Add your answers to the Algorithms exercises here.

1. Exercise 1
    1. O(n)
    2. O(log n)
    3. O(sqrt(n)) ???
        1. if n > 128 128 aka 8^2/2, sum does not increase further
    4. O(n * log(n))
    5. O(n * n-1 * n-2) = O(n^3)
    6. O(n)
    7. O(n)

2. Exercise 2
``` python
def biggest_value(arr):
    max_value = arr[1] - arr[0]
    min_element = arr[0]

    for item in arr:
        if item - min_element > max_value:
            max_value = item - min_element
        if item < min_element:
            min_element = item
    return max_value
```
basically, cycle through the list once only.  instantiate the the first value as a the min value.
As you loop through list, if item is less than min value, update min value
as you go through the array, since you have a min value upto index, you can use that to calculate the value
if the value is greater, then replace it.

```python
def will_it_break(floorLevels, criticalLevel):
    brokenEggs = 0
    tries = 0
    if floorLevels > criticalLevel:
        brokenEggs += 1
        tries += 1

        will_it_break(floorLevels/2, criticalLevel)
    if floorLevels < criticalLevel:
        tries += 1
        will_it_break((floorLevels+(floorLevels/2))/2, criticalLevel)
    if floorLevels == criticalLevel:
        return brokenEggs

```

Basically test the egg at top level.  If it breaks, test at middle.  This would elimintate half the choices. Then keep testing at the halfway points until you get 2 remaining.  Log time complexity


3. Excercise 3
    a) O(n^2) - quick sort method would essentially be a loop within a loop.
        it would call a loop for each item on the original list on the remaining items
    b) O(n log(n)) - It's still like a loop within a loop, but the inner loop is now optimal and split into 2 each time and then the second n is a "log(n)"



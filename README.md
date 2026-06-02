# linked_list
# Count Positives, Sum Negatives

## Problem

Given an array of integers:

* Count the positive numbers.
* Sum the negative numbers.
* Ignore zeros.
* Return an empty list if the array is empty or `None`.

### Example

Input:

```python
[1, 2, 3, 4, 5, 6, 7, 8, 9, 10, -11, -12, -13, -14, -15]
```

Output:

```python
[10, -65]
```

## Solution

```python
def count_positives_sum_negatives(arr):
    if not arr:
        return []

    positive_count = 0
    negative_sum = 0

    for num in arr:
        if num > 0:
            positive_count += 1
        elif num < 0:
            negative_sum += num

    return [positive_count, negative_sum]
```

## Run the Program

```bash
python3 solution.py
```

## Author

Gregory Kip

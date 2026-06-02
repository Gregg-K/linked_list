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


# Merge Two Sorted Lists

## Description

This project solves the LeetCode problem **Merge Two Sorted Lists** using Python and Linked Lists.

Given the heads of two sorted linked lists, merge them into one sorted linked list and return the head of the merged list.

## Example

Input:

```python
list1 = [1,2,4]
list2 = [1,3,4]
```

Output:

```python
[1,1,2,3,4,4]
```

## Solution

The solution compares nodes from both linked lists and appends the smaller node to the merged list until all nodes have been processed.

## Run

Run it in a Python environment that supports the `ListNode` class.

## Author

Gregory Kip

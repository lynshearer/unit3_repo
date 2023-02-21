# Quiz 033

## Solution to Quiz #033

```.py
def mystery(list1:list, list2:list)->list:
    output = []
    for num in list1:
        for num2 in list2:
            if num == num2:
                output.append(num)
    return output
```

## Test of Solution

```.py
import pytest
from quiz033 import mystery

def test_empty_lists():
  assert mystery([], []) == []

def test_one_common_element():
  assert mystery([1, 2, 3], [3, 4, 5]) == [3]

def test_multiple_common_elements():
  assert mystery([1, 2, 3, 4], [3, 4, 5, 6]) == [3, 4]
  ```
  
  ## Proof of Working Solution 
  
  <img width="1112" alt="quiz033" src="https://user-images.githubusercontent.com/111893043/220255401-1ffc3cd6-4c21-4b6b-ac1c-eb1db8c37a65.png">

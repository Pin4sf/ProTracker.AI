# Two Sum Problem

**Link:** [https://leetcode.com/problems/two-sum](https://leetcode.com/problems/two-sum)

**Summary:**
This is a mock summary of the solution.

**Topics Covered:** Mock Topic 1, Mock Topic 2

**Solution:**
```python
def twoSum(nums, target):
    for i in range(len(nums)):
        for j in range(i + 1, len(nums)):
            if nums[i] + nums[j] == target:
                return [i, j]
```
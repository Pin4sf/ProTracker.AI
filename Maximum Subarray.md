# Maximum Subarray

**Link:** [https://leetcode.com/problems/maximum-subarray](https://leetcode.com/problems/maximum-subarray)

**Summary:**
This is a mock summary of the solution.

**Topics Covered:** Mock Topic 1, Mock Topic 2

**Solution:**
```python
def maxSubArray(nums):\n    max_sum = nums[0]\n    current_sum = nums[0]\n    for num in nums[1:]:\n        current_sum = max(num, current_sum + num)\n        max_sum = max(max_sum, current_sum)\n    return max_sum
```
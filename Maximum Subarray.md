# Maximum Subarray

**Link:** [https://leetcode.com/problems/maximum-subarray](https://leetcode.com/problems/maximum-subarray)

**Summary:**
This is a mock summary of the solution.

**Topics Covered:** Mock Topic 1, Mock Topic 2

**Solution:**
```python
class Solution:
    def maxSubArray(self, nums):
        ans = -inf
        for i in range(len(nums)):
            cur_sum = 0
            for j in range(i, len(nums)):
                cur_sum += nums[j]
                ans = max(ans, cur_sum)
        return ans
```
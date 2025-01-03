# Longest Substring Without Repeating Characters

**Link:** [https://leetcode.com/problems/longest-substring-without-repeating-characters](https://leetcode.com/problems/longest-substring-without-repeating-characters)

**Summary:**
This is a mock summary of the solution.

**Topics Covered:** Mock Topic 1, Mock Topic 2

**Solution:**
```python
def lengthOfLongestSubstring(s):
    charSet = set()
    l = 0
    res = 0

    for r in range(len(s)):
        while s[r] in charSet:
            charSet.remove(s[l])
            l += 1
        charSet.add(s[r])
        res = max(res, r - l + 1)

    return res
```
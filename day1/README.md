## Single Number
Given a **non-empty** array of integers, every element appears twice except for one. Find that single one.

**Note:**

* Your algorithm should have a linear runtime complexity. Could you implement it without using extra memory?

Example 1:
```
Input: [2,2,1]
Output: 1
```
Example 2:
```
Input: [4,1,2,1,2]
Output: 4
```

## Approach

The above uses the following properties of **Bitwise XOR**(^)
```
A ^ A = 0
0 ^ A = A
A ^ 0 = A
```

Since, there is only one element which is present once, all the other values will be reduced to 0. The single elment when XOR'ed to 0 would result in itself.

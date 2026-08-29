# LeetCode 73 – Set Matrix Zeroes

Given an `m × n` integer matrix, if an element is `0`, set its entire row and column to `0`.

The changes must be made **in-place**.

## Example

### Input

```text
matrix = [[1,1,1],
          [1,0,1],
          [1,1,1]]
```

### Output

```text
[[1,0,1],
 [0,0,0],
 [1,0,1]]
```

## Approach

I use the first row and first column of the matrix to store information about which rows and columns contain zeroes.

First, I check whether the first row or first column originally contains a zero.

Then I mark the corresponding rows and columns while scanning the rest of the matrix.

Finally, I set the required rows and columns to zero.

This avoids using an extra matrix.

## Complexity

* **Time Complexity:** `O(M × N)`
* **Space Complexity:** `O(1)`

## Language

**Python**

## LeetCode

**Problem:** 73. Set Matrix Zeroes
**Difficulty:** Medium
**Topic:** Array, Matrix

## Author

T.Nandhini

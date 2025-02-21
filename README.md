# Daily-Leetcode-problem-solution9
PROBLEM

Given a 2D grid of size m x n and an integer k. You need to shift the grid k times.

In one shift operation:

Element at grid[i][j] moves to grid[i][j + 1].
Element at grid[i][n - 1] moves to grid[i + 1][0].
Element at grid[m - 1][n - 1] moves to grid[0][0].
Return the 2D grid after applying shift operation k times.

Intuition

Using 1D tranformation technique

Approach

Flatten the 2D grid into a 1D array:
The 2D grid has m × n elements.
Store these elements in a 1D array to facilitate shifting.

Perform the shift operation efficiently:
Instead of shifting elements one by one (which would be inefficient), we calculate the new position using modulo arithmetic.
A shift of k times means each element moves k % (m * n) positions forward.

Map back to a 2D grid:
Convert the shifted 1D array back into a 2D grid.

Complexity

Time complexity:

Flattening the 2D grid:
O(m×n)
Shifting elements using a new array:
O(m×n)
Mapping back to 2D:
O(m×n)
Overall time complexity:
O(m×n)

Space complexity:

O(m×n)

 

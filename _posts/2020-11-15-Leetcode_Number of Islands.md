---
title: "LeetCode Number of Islands"
date: 2020-11-15 01:09:11
excerpt: "알고리즘 스터디 4회차"
categories:
  - Algorithm
tags:
  - DFS
  - LeetCode
  - python
  - Algorithm
---

### LeetCode Number of Islands

[Number of Islands](https://leetcode.com/problems/number-of-islands/)

DFS(깊이 우선 탐색)는 원리는 마음에 와닿지만 문제를 풀기란 쉽지 않았다.

```python
class Solution:
    def numIslands(self, grid: List[List[str]]) -> int:
        def dfs(i, j):

            if i<0 or i >= len(grid) or j < 0 or j >= len(grid[0]) or grid[i][j]!='1':
                return

            grid[i][j] = 0

            dfs(i+1, j)
            dfs(i-1, j)
            dfs(i, j+1)
            dfs(i, j-1)
        count = 0

        for i in range(len(grid)):
            for j in range(len(grid[0])):
                if grid[i][j] == '1':
                    dfs(i, j)
                    count+=1


        return count        
```

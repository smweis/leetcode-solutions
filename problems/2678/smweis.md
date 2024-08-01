# [Problem 2678: Number of Senior Citizens](https://leetcode.com/problems/number-of-senior-citizens/description/?envType=daily-question)

## Initial thoughts (stream-of-consciousness)
Easy - parse each element, compare to 60. Count total. 
## Refining the problem, round 2 thoughts

## Attempted solution(s)
```python
class Solution:
    def countSeniors(self, details: List[str]) -> int:

        n_sixty_year_olds = [int(i[11:13]) for i in details if int(i[11:13]) > 60]

        return len(n_sixty_year_olds)
```

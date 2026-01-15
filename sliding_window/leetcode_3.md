## Longest Substring Without Repeating Characters

- I got the most optimal solution -- Actual O(n) and not O(2n)
- The key was, having a limit var. This limit var allows us to check whether the last known pos of the current char was before the limit (and if yes, just update to this pos). (if not, error, this substring has a repeating char). This way, we eliminate the need of another pass which makes this truly O(n) instead of the conventional O(2n)
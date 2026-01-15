So far, here is what I have learned. 

### Approach

- Intuition —> You have a temp_hashmap that is basically the hashmap over your current state (window).
- Whether you have a fixed or dynamic sliding window, the state (current window) is updated (move left or both pointers) when the condition is not met. So when you are solving such questions, think of it this way —>
    - Every Sliding Window has its own hashmap that I can compare with the final condition. Check
    - Check for the final condition at every iteration
    - If the condition is not met, update l, or r (or both).

### Links to help

- [Perplexity: A nice misunderstanding cleared to understand the classic sliding window template of two pass](https://www.perplexity.ai/search/for-the-question-longest-subst-LQv29B_XSsuuCymO7B8SYA#0)


### Some Nice Leetcode questions to look at

- [Longest Substring Without Repeating Chars. Got the MOST optimal (O(n))](./leetcode_3.md)
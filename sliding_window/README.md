So far, here is what I have learned. 

### Approach

- Intuition —> You have a temp_hashmap that is basically the hashmap over your current state (window).
- Whether you have a fixed or dynamic sliding window, the state (current window) is updated (move left or both pointers) when the condition is not met. So when you are solving such questions, think of it this way —>
    - Every Sliding Window has its own hashmap that I can compare with the final condition. Check
    - Check for the final condition at every iteration
    - If the condition is not met, update l, or r (or both).
- **New Finding**
    - The question is to either have the longest state, or the shortest state (where state is correct). Depending on this, the l pointer can have diff purposes.
    - If we want longest, then we dont double check current correct state. Just do normal two pass template
    - But if we want shortest, then there is a chance that the current correct state is suboptimal, so keep updating the l pointer until its not correct while checking for the min(res) at every iteration (of l pointer)

### Links to help

- [Perplexity: A nice misunderstanding cleared to understand the classic sliding window template of two pass](https://www.perplexity.ai/search/for-the-question-longest-subst-LQv29B_XSsuuCymO7B8SYA#0)

### Some Nice Leetcode questions to look at

- [Longest Substring Without Repeating Chars. Got the MOST optimal (O(n))](./leetcode_3.md)
- [Min Size Subs summ](https://neetcode.io/problems/minimum-size-subarray-sum/question?list=neetcode250)
    - This is nice since the logic is reverse. Instead of maximising, you are finding the minimising. The r pointer moves until we have a correct state. But what if this state can be shorten too? Hence we keep moving the l pointer until state != correct (while checking for the best result)
- [Min Window Subs](https://leetcode.com/problems/minimum-window-substring/submissions/1889038052/) --> Check the Neetcode Sol. I couldnt do it since its completely reverse of prev med questions template. Check Perplexity comments [here](https://www.perplexity.ai/search/sliding-window-b7vA_RzoTRe_7TC_RZWlIg). Scroll down to get it

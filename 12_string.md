# String

Problem list from [0x3F's LeetCode Study Plan](https://leetcode.cn/circle/discuss/SJFwQI/) — String (KMP / Z-function / Manacher / String Hashing / AC Automaton / Suffix Array / Subsequence Automaton).

## I. KMP (Borders of Prefixes)

[KMP Explained](https://www.zhihu.com/question/21923021/answer/37475572)

Define a **proper prefix** of `s` as a prefix not equal to `s`, and a **proper suffix** of `s` as a suffix not equal to `s`.

Define a **border** of `s` as a string that is both a proper prefix and a proper suffix of `s`. For example, in `s = "aabcaa"`, both `"a"` and `"aa"` are borders of `s`.

For each prefix `p[:i]` of the pattern string `p`, compute the length of its longest border and store it in the `π` array.

Using the `π` array, we can quickly find every position at which the pattern string `p` occurs in the text string `t`.

> Note: The `π` array notation follows *Introduction to Algorithms*. Chinese data-structure textbooks usually call it the `next` array; some index it from 1, others from 0 (with a leading 0 prepended). The underlying idea is the same — only the implementation details differ.

- [28. Find the Index of the First Occurrence in a String](https://leetcode.com/problems/find-the-index-of-the-first-occurrence-in-a-string/) (template problem)
- [796. Rotate String](https://leetcode.com/problems/rotate-string/) (achieve linear time)
- [1392. Longest Happy Prefix](https://leetcode.com/problems/longest-happy-prefix/) 1876
- [3036. Number of Subarrays That Match a Pattern II](https://leetcode.com/problems/number-of-subarrays-that-match-a-pattern-ii/) 1895
- [1764. Form Array by Concatenating Subarrays of Another Array](https://leetcode.com/problems/form-array-by-concatenating-subarrays-of-another-array/) (achieve linear time)
- [1668. Maximum Repeating Substring](https://leetcode.com/problems/maximum-repeating-substring/) (achieve linear time)
- [459. Repeated Substring Pattern](https://leetcode.com/problems/repeated-substring-pattern/) (achieve linear time)
- [2800. Shortest String That Contains Three Strings](https://leetcode.com/problems/shortest-string-that-contains-three-strings/) (achieve linear time)
- [3008. Find Beautiful Indices in the Given Array II](https://leetcode.com/problems/find-beautiful-indices-in-the-given-array-ii/) 2016
- [214. Shortest Palindrome](https://leetcode.com/problems/shortest-palindrome/) (can also be solved with Manacher's algorithm)
- [3529. Count Cells In Overlapping Horizontal And Vertical Substrings](https://leetcode.com/problems/count-cells-in-overlapping-horizontal-and-vertical-substrings/) 2105
- [686. Repeated String Match](https://leetcode.com/problems/repeated-string-match/) ~2200
- [3455. Shortest Matching Substring](https://leetcode.com/problems/shortest-matching-substring/) 2303
- [1397. Find All Good Strings](https://leetcode.com/problems/find-all-good-strings/) 2667
- [3037. Find Pattern in Infinite Stream II](https://leetcode.com/problems/find-pattern-in-infinite-stream-ii/) 🔒 (same as problem 28)
- [3571. Find the Shortest Superstring II](https://leetcode.com/problems/find-the-shortest-superstring-ii/) 🔒 (related to problem 2800)

## II. Z-function (Prefixes of Suffixes)

> **Note**: In Chinese competitive-programming circles, this algorithm is also called **Extended KMP**.

For a string `s`, define `z[i]` as the length of the LCP (longest common prefix) between the suffix `s[i:]` and `s`, where `s[i:]` denotes the substring from `s[i]` to `s[n-1]`.

A common technique is to build the string `pattern + s` or `pattern + '#' + s`. If `z[m+i] >= m` (where `m` is the length of `pattern`), then the substring starting at `s[i]` matches `pattern`.

So some of the KMP substring-matching problems above can also be solved with the Z-function. Try solving [28. Find the Index of the First Occurrence in a String](https://leetcode.com/problems/find-the-index-of-the-first-occurrence-in-a-string/) with the Z-function.

- [2223. Sum of Scores of Built Strings](https://leetcode.com/problems/sum-of-scores-of-built-strings/) 2220 (template problem)
- [3031. Minimum Time to Revert Word to Initial State II](https://leetcode.com/problems/minimum-time-to-revert-word-to-initial-state-ii/) 2278
- [3045. Count Prefix And Suffix Pairs II](https://leetcode.com/problems/count-prefix-and-suffix-pairs-ii/) 2328
- [3303. Find the Occurrence of First Almost Equal Substring](https://leetcode.com/problems/find-the-occurrence-of-first-almost-equal-substring/) 2509
- [3292. Minimum Number of Valid Strings to Form Target II](https://leetcode.com/problems/minimum-number-of-valid-strings-to-form-target-ii/) 2662
- [3474. Lexicographically Smallest Generated String](https://leetcode.com/problems/lexicographically-smallest-generated-string/) (achieve O(n+m))

**LCP Array**

- [2430. Maximum Deletions on a String](https://leetcode.com/problems/maximum-deletions-on-a-string/) 2102
- [3388. Count Beautiful Splits in an Array](https://leetcode.com/problems/count-beautiful-splits-in-an-array/) 2365
- [2573. Find the String with LCP](https://leetcode.com/problems/find-the-string-with-lcp/) 2682
- [1977. Number of Ways to Separate Numbers](https://leetcode.com/problems/number-of-ways-to-separate-numbers/) 2817

## III. Manacher's Algorithm (Palindromic Substrings)

Manacher's algorithm computes the length of the longest palindromic substring centered at `s[i]` (or between `s[i]` and `s[i+1]`).

It can also:

- Determine whether an arbitrary substring is a palindrome.
- Compute the length of the longest palindromic substring starting at `s[i]`.
- Compute the length of the longest palindromic substring ending at `s[i]`.

> The Z-function and Manacher's algorithm both rely on a concept similar to a Z-box — comparing the two while learning can deepen your understanding of both.

[Template code](https://leetcode.com/problems/longest-palindromic-substring/solutions/2958179/mo-ban-on-manacher-suan-fa-pythonjavacgo-t6cx/)

- [5. Longest Palindromic Substring](https://leetcode.com/problems/longest-palindromic-substring/) (template problem)
- [647. Palindromic Substrings](https://leetcode.com/problems/palindromic-substrings/) (count the number of palindromic substrings)
- [214. Shortest Palindrome](https://leetcode.com/problems/shortest-palindrome/)
- [3327. Check if DFS Strings Are Palindromes](https://leetcode.com/problems/check-if-dfs-strings-are-palindromes/) 2454
- [1745. Palindrome Partitioning IV](https://leetcode.com/problems/palindrome-partitioning-iv/) (achieve O(n))
- [1960. Maximum Product of the Length of Two Palindromic Substrings](https://leetcode.com/problems/maximum-product-of-the-length-of-two-palindromic-substrings/) 2691
- [3844. Longest Almost Palindromic Substring](https://leetcode.com/problems/longest-almost-palindromic-substring/) (achieve O(n log n))
- [3504. Longest Palindrome After Substring Concatenation II](https://leetcode.com/problems/longest-palindrome-after-substring-concatenation-ii/) (achieve O(n+m))

Problems using **center expansion** (and its underlying idea):

[Template code](https://leetcode.com/problems/longest-palindromic-substring/solutions/2958179/mo-ban-on-manacher-suan-fa-pythonjavacgo-t6cx/)

- [5. Longest Palindromic Substring](https://leetcode.com/problems/longest-palindromic-substring/) (template problem)
- [3844. Longest Almost Palindromic Substring](https://leetcode.com/problems/longest-almost-palindromic-substring/) 1990
- [2472. Maximum Number of Non-overlapping Palindrome Substrings](https://leetcode.com/problems/maximum-number-of-non-overlapping-palindrome-substrings/) 2013
- [3504. Longest Palindrome After Substring Concatenation II](https://leetcode.com/problems/longest-palindrome-after-substring-concatenation-ii/) 2398
- [3615. Longest Palindromic Path in Graph](https://leetcode.com/problems/longest-palindromic-path-in-graph/) 2463
- [3579. Minimum Steps to Convert String with Operations](https://leetcode.com/problems/minimum-steps-to-convert-string-with-operations/) (achieve O(n^2))

## IV. String Hashing

Most problems in this list can be solved with string hashing.

We recommend doing [2156. Find Substring With Given Hash Value](https://leetcode.com/problems/find-substring-with-given-hash-value/) and [3756. Concatenate Non-Zero Digits And Multiply By Sum II](https://leetcode.com/problems/concatenate-non-zero-digits-and-multiply-by-sum-ii/) first — they'll help you understand how to compute a **polynomial hash**.

**Template code** is available in [my solution](https://leetcode.com/problems/construct-string-with-minimum-cost/solutions/2833949/hou-zhui-shu-zu-by-endlesscheng-32h9/), covering both single-modulus and double-modulus hashing.

**Tip**: You can use string hashing to compare the lexicographic order of two substrings — binary search on the length to compute their LCP (longest common prefix), then compare the character right after the LCP (which must differ, or not exist) to see which substring is smaller. Time complexity: O(log n). See problem 3722.

- [28. Find the Index of the First Occurrence in a String](https://leetcode.com/problems/find-the-index-of-the-first-occurrence-in-a-string/)
- [187. Repeated DNA Sequences](https://leetcode.com/problems/repeated-dna-sequences/)
- [1316. Distinct Echo Substrings](https://leetcode.com/problems/distinct-echo-substrings/) 1837
- [1297. Maximum Number Of Occurrences Of A Substring](https://leetcode.com/problems/maximum-number-of-occurrences-of-a-substring/) (achieve O(n))
- [2261. K-Divisible Elements Subarrays](https://leetcode.com/problems/k-divisible-elements-subarrays/) (achieve O(n^2))
- [3722. Lexicographically Smallest String After Reverse](https://leetcode.com/problems/lexicographically-smallest-string-after-reverse/) (achieve O(n log n))
- [3934. Smallest Unique Subarray](https://leetcode.com/problems/smallest-unique-subarray/) 2163
- [3213. Construct String with Minimum Cost](https://leetcode.com/problems/construct-string-with-minimum-cost/) 2171
- [1367. Linked List in Binary Tree](https://leetcode.com/problems/linked-list-in-binary-tree/) (achieve linear time)
- [1044. Longest Duplicate Substring](https://leetcode.com/problems/longest-duplicate-substring/) 2429
- [718. Maximum Length of Repeated Subarray](https://leetcode.com/problems/maximum-length-of-repeated-subarray/)
- [1923. Longest Common Subpath](https://leetcode.com/problems/longest-common-subpath/) 2661
- [3292. Minimum Number of Valid Strings to Form Target II](https://leetcode.com/problems/minimum-number-of-valid-strings-to-form-target-ii/) 2662
- [3844. Longest Almost Palindromic Substring](https://leetcode.com/problems/longest-almost-palindromic-substring/) (achieve O(n log n) or O(n))
- [2168. Unique Substrings With Equal Digit Frequency](https://leetcode.com/problems/unique-substrings-with-equal-digit-frequency/) 🔒 (same as problem 2261)
- [1554. Strings Differ by One Character](https://leetcode.com/problems/strings-differ-by-one-character/) 🔒
- [1062. Longest Repeating Substring](https://leetcode.com/problems/longest-repeating-substring/) 🔒 (same as problem 1044)

## V. Minimal String Rotation

Define a **left cyclic shift**: remove the first character `s[0]` of string `s` and append it to the end. For example, one left cyclic shift of `"abcd"` gives `"bcda"`.

Problem: given that you may perform any number of left cyclic shifts, compute the lexicographically smallest string obtainable.

**Note**: the string obtained after any number of left cyclic shifts is called a **cyclic rotation** of `s`.

The lexicographically smallest cyclic rotation of `s` can be computed in O(n) with a two-pointer approach: maintain two candidate start positions `i` and `j`, compare the strings starting at each, and — based on where the first mismatch occurs — skip ahead past all positions that are provably no better than the current best.

We recommend completing [1163. Last Substring in Lexicographical Order](https://leetcode.com/problems/last-substring-in-lexicographical-order/) first — minimal string rotation is the circular version of this problem.

- [899. Orderly Queue](https://leetcode.com/problems/orderly-queue/) (the case k=1 is exactly minimal string rotation, solvable in O(n))
- [3403. Find the Lexicographically Largest String From the Box I](https://leetcode.com/problems/find-the-lexicographically-largest-string-from-the-box-i/)
- [1625. Lexicographically Smallest String After Applying Operations](https://leetcode.com/problems/lexicographically-smallest-string-after-applying-operations/)
- [3406. Find the Lexicographically Largest String From the Box II](https://leetcode.com/problems/find-the-lexicographically-largest-string-from-the-box-ii/) 🔒
- [1708. Largest Subarray Length K](https://leetcode.com/problems/largest-subarray-length-k/) 🔒 (see the follow-up)

## VI. Trie

See "VI. Trie" in the [Data Structures list](https://leetcode.cn/circle/discuss/mOr1u6/).

## VII. Aho-Corasick Automaton (AC Automaton)

AC Automaton = Trie + KMP.

Since these problems can also be solved with other algorithms (string hashing, etc.), the difficulty ratings are for reference only.

- [1032. Stream of Characters](https://leetcode.com/problems/stream-of-characters/) 1970 (template problem)
- [1967. Number of Strings That Appear as Substrings in Word](https://leetcode.com/problems/number-of-strings-that-appear-as-substrings-in-word/) (template problem)
- [Interview 17.17. Multi Search](https://leetcode.com/problems/multi-search-lcci/) (template problem)
- [1408. String Matching in an Array](https://leetcode.com/problems/string-matching-in-an-array/) (achieve linear time)
- [3213. Construct String with Minimum Cost](https://leetcode.com/problems/construct-string-with-minimum-cost/) 2171
- [2781. Length Of The Longest Valid Substring](https://leetcode.com/problems/length-of-the-longest-valid-substring/) 2204
- [3292. Minimum Number of Valid Strings to Form Target II](https://leetcode.com/problems/minimum-number-of-valid-strings-to-form-target-ii/) 2662
- [3758. Convert Number Words to Digits](https://leetcode.com/problems/convert-number-words-to-digits/) 🔒 (a more general approach)

## VIII. Suffix Array / Suffix Automaton

Since these problems can also be solved with other algorithms (string hashing, etc.), the difficulty ratings are for reference only.

- [1163. Last Substring in Lexicographical Order](https://leetcode.com/problems/last-substring-in-lexicographical-order/) 1864
- [1754. Largest Merge Of Two Strings](https://leetcode.com/problems/largest-merge-of-two-strings/) (achieve O(n+m))
- [2904. Shortest And Lexicographically Smallest Beautiful String](https://leetcode.com/problems/shortest-and-lexicographically-smallest-beautiful-string/) (achieve O(n log n))
- [3722. Lexicographically Smallest String After Reverse](https://leetcode.com/problems/lexicographically-smallest-string-after-reverse/) (achieve O(n log n))
- [3934. Smallest Unique Subarray](https://leetcode.com/problems/smallest-unique-subarray/) 2163
- [3213. Construct String with Minimum Cost](https://leetcode.com/problems/construct-string-with-minimum-cost/) 2171
- [1044. Longest Duplicate Substring](https://leetcode.com/problems/longest-duplicate-substring/) 2429
- [718. Maximum Length of Repeated Subarray](https://leetcode.com/problems/maximum-length-of-repeated-subarray/)
- [1923. Longest Common Subpath](https://leetcode.com/problems/longest-common-subpath/) 2661
- [1408. String Matching in an Array](https://leetcode.com/problems/string-matching-in-an-array/)
- [3729. Count Distinct Subarrays Divisible By K In Sorted Array](https://leetcode.com/problems/count-distinct-subarrays-divisible-by-k-in-sorted-array/) (an approach that doesn't require the array to be non-increasing; counts substantively distinct subarrays)
- [3076. Shortest Uncommon Substring in an Array](https://leetcode.com/problems/shortest-uncommon-substring-in-an-array/)
- [3844. Longest Almost Palindromic Substring](https://leetcode.com/problems/longest-almost-palindromic-substring/) (achieve O(n log n))
- [3504. Longest Palindrome After Substring Concatenation II](https://leetcode.com/problems/longest-palindrome-after-substring-concatenation-ii/) (achieve O(n+m))
- [1316. Distinct Echo Substrings](https://leetcode.com/problems/distinct-echo-substrings/)
- [3388. Count Beautiful Splits in an Array](https://leetcode.com/problems/count-beautiful-splits-in-an-array/) (achieve O(n log n) or O(n))
- [2564. Substring XOR Queries](https://leetcode.com/problems/substring-xor-queries/) (see the [comment](https://leetcode.com/problems/substring-xor-queries/solutions/2107060/yu-chu-li-suo-you-s-zhong-de-shu-zi-by-e-yxl2/comments/1922325/) under my solution)
- [Interview 16.18. Pattern Matching](https://leetcode.com/problems/pattern-matching-lcci/) (suffix tree)
- [1698. Number of Distinct Substrings in a String](https://leetcode.com/problems/number-of-distinct-substrings-in-a-string/) 🔒
- [1062. Longest Repeating Substring](https://leetcode.com/problems/longest-repeating-substring/) 🔒 (same as problem 1044)
- [3135. Equalize Strings by Adding or Removing Characters at Ends](https://leetcode.com/problems/equalize-strings-by-adding-or-removing-characters-at-ends/) 🔒

## IX. Subsequence Automaton

The sections above are all about algorithms related to **substrings**. This section covers an algorithm related to **subsequences**: the subsequence automaton.

Despite the fancy name, it's really just precomputing, for each position `i`, the nearest index `>= i` at which a given character `c` occurs.

See the "Follow-up" in [this explanation](https://leetcode.com/problems/is-subsequence/solutions/2813031/jian-ji-xie-fa-pythonjavaccgojsrust-by-e-mz22/).

- [792. Number of Matching Subsequences](https://leetcode.com/problems/number-of-matching-subsequences/) 1695
- [514. Freedom Trail](https://leetcode.com/problems/freedom-trail/) ~2400 (achieve O(nm))
- [2014. Longest Subsequence Repeated K Times](https://leetcode.com/problems/longest-subsequence-repeated-k-times/) 2558
- [1055. Shortest Way to Form String](https://leetcode.com/problems/shortest-way-to-form-string/) 🔒
- [727. Minimum Window Subsequence](https://leetcode.com/problems/minimum-window-subsequence/) 🔒

## X. Others

- [3485. Longest Common Prefix of K Strings After Removal](https://leetcode.com/problems/longest-common-prefix-of-k-strings-after-removal/) 2290 (properties of LCP)
- [466. Count The Repetitions](https://leetcode.com/problems/count-the-repetitions/) (achieve O(|s1|+|s2|))
- [3491. Phone Number Prefix](https://leetcode.com/problems/phone-number-prefix/) 🔒 (non-brute-force approach)

## Related Lists

- [Data Structures list](https://leetcode.cn/circle/discuss/mOr1u6/) — the "VI. Trie" section.
- [Sliding Window & Two Pointers list](https://leetcode.cn/circle/discuss/0viNMK/) — the "§4.2 Merge Two Arrays/Strings" section.
- [Math list](https://leetcode.cn/circle/discuss/IYT3ss/) — the "§7.4 Polynomials" section.
- [Greedy list](https://leetcode.cn/circle/discuss/g6KTKL/) — the "III. String Greedy" section.

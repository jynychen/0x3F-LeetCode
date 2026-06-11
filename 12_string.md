# String Algorithms

> Problem list from [0x3F's LeetCode Problem Lists](https://leetcode.cn/circle/discuss/SJFwQI/)

## KMP（前缀的后缀）
------------

模板：

Python3

Java

C++

Go

    def kmp(text: str, pattern: str) -> List[int]:
        m = len(pattern)
        pi = [0] * m
        cnt = 0
        for i in range(1, m):
            b = pattern[i]
            while cnt and pattern[cnt] != b:
                cnt = pi[cnt - 1]
            if pattern[cnt] == b:
                cnt += 1
            pi[i] = cnt

        pos = []
        cnt = 0
        for i, b in enumerate(text):
            while cnt and pattern[cnt] != b:
                cnt = pi[cnt - 1]
            if pattern[cnt] == b:
                cnt += 1
            if cnt == len(pattern):
                pos.append(i - m + 1)
                cnt = pi[cnt - 1]
        return pos

*   [28. Find the Index of the First Occurrence in a String](https://leetcode.com/problems/find-the-index-of-the-first-occurrence-in-a-string/) ****
*   [796. Rotate String](https://leetcode.com/problems/rotate-string/)
*   [1392. Longest Happy Prefix](https://leetcode.com/problems/longest-happy-prefix/) 1876
*   [3036. Number of Subarrays that Match a Pattern Ii](https://leetcode.com/problems/number-of-subarrays-that-match-a-pattern-ii/) 1895
*   [1764. Form Array by Concatenating Subarrays of Another Array](https://leetcode.com/problems/form-array-by-concatenating-subarrays-of-another-array/)
*   [1668. Maximum Repeating Substring](https://leetcode.com/problems/maximum-repeating-substring/)
*   [459. Repeated Substring Pattern](https://leetcode.com/problems/repeated-substring-pattern/)
*   [2800. Shortest String that Contains Three Strings](https://leetcode.com/problems/shortest-string-that-contains-three-strings/)
*   [3008. Find Beautiful Indices in the Given Array Ii](https://leetcode.com/problems/find-beautiful-indices-in-the-given-array-ii/) 2016
*   [214. Shortest Palindrome](https://leetcode.com/problems/shortest-palindrome/) Manacher
*   [3529. Count Cells in Overlapping Horizontal and Vertical Substrings](https://leetcode.com/problems/count-cells-in-overlapping-horizontal-and-vertical-substrings/) 2105
*   [686. Repeated String Match](https://leetcode.com/problems/repeated-string-match/) 2200
*   [3455. Shortest Matching Substring](https://leetcode.com/problems/shortest-matching-substring/) 2303
*   [1397. Find All Good Strings](https://leetcode.com/problems/find-all-good-strings/) 2667
*   [3037. Find Pattern in Infinite Stream Ii](https://leetcode.com/problems/find-pattern-in-infinite-stream-ii/) (Premium)
*   [3571. Find the Shortest Superstring Ii](https://leetcode.com/problems/find-the-shortest-superstring-ii/) (Premium) 2800

-------------

模板：

Python3

Java

C++

Go

    def calc_z(s: str) -> List[int]:
        n = len(s)
        z = [0] * n
        box_l = box_r = 0
        for i in range(1, n):
            if i <= box_r:
                z[i] = min(z[i - box_l], box_r - i + 1)
            while i + z[i] < n and s[z[i]] == s[i + z[i]]:
                box_l, box_r = i, i + z[i]
                z[i] += 1
        z[0] = n
        return z

*   [2223. Sum of Scores of Built Strings](https://leetcode.com/problems/sum-of-scores-of-built-strings/) 2220 ****
*   [3031. Minimum Time to Revert Word to Initial State Ii](https://leetcode.com/problems/minimum-time-to-revert-word-to-initial-state-ii/) 2278
*   [3045. Count Prefix and Suffix Pairs Ii](https://leetcode.com/problems/count-prefix-and-suffix-pairs-ii/) 2328
*   [3303. Find the Occurrence of First Almost Equal Substring](https://leetcode.com/problems/find-the-occurrence-of-first-almost-equal-substring/) 2509
*   [3292. Minimum Number of Valid Strings to Form Target Ii](https://leetcode.com/problems/minimum-number-of-valid-strings-to-form-target-ii/) 2662
*   [3474. Lexicographically Smallest Generated String](https://leetcode.com/problems/lexicographically-smallest-generated-string/)

**LCP 数组**

*   [2430. Maximum Deletions on a String](https://leetcode.com/problems/maximum-deletions-on-a-string/) 2102
*   [3388. Count Beautiful Splits in an Array](https://leetcode.com/problems/count-beautiful-splits-in-an-array/) 2365
*   [1977. Number of Ways to Separate Numbers](https://leetcode.com/problems/number-of-ways-to-separate-numbers/) 2817

## Manacher 算法（回文串）
------------------

*   判断任意子串是否为回文串。
*   计算从 s\[i\] 开始的最长回文子串的长度。
*   计算以 s\[i\] 结尾的最长回文子串的长度。

*   [5. Longest Palindromic Substring](https://leetcode.com/problems/longest-palindromic-substring/) ****
*   [647. Palindromic Substrings](https://leetcode.com/problems/palindromic-substrings/)
*   [214. Shortest Palindrome](https://leetcode.com/problems/shortest-palindrome/)
*   [3327. Check If Dfs Strings Are Palindromes](https://leetcode.com/problems/check-if-dfs-strings-are-palindromes/) 2454
*   [1745. Palindrome Partitioning Iv](https://leetcode.com/problems/palindrome-partitioning-iv/)
*   [1960. Maximum Product of the Length of Two Palindromic Substrings](https://leetcode.com/problems/maximum-product-of-the-length-of-two-palindromic-substrings/) 2691
*   [3504. Longest Palindrome after Substring Concatenation Ii](https://leetcode.com/problems/longest-palindrome-after-substring-concatenation-ii/)

*   [5. Longest Palindromic Substring](https://leetcode.com/problems/longest-palindromic-substring/) ****
*   [2472. Maximum Number of Non Overlapping Palindrome Substrings](https://leetcode.com/problems/maximum-number-of-non-overlapping-palindrome-substrings/) 2013
*   [3504. Longest Palindrome after Substring Concatenation Ii](https://leetcode.com/problems/longest-palindrome-after-substring-concatenation-ii/) 2398
*   [3615. Longest Palindromic Path in Graph](https://leetcode.com/problems/longest-palindromic-path-in-graph/) 2463
*   [3579. Minimum Steps to Convert String with Operations](https://leetcode.com/problems/minimum-steps-to-convert-string-with-operations/)

## String Hashing
-------


**小技巧**：我们可以用字符串哈希比较两个子串的字典序大小。做法是二分长度，计算最长公共前缀（LCP），然后比较 LCP 的下一个字母。时间复杂度：O(logn)。见 3722 题。

*   [28. Find the Index of the First Occurrence in a String](https://leetcode.com/problems/find-the-index-of-the-first-occurrence-in-a-string/)
*   [187. Repeated Dna Sequences](https://leetcode.com/problems/repeated-dna-sequences/)
*   [1316. Distinct Echo Substrings](https://leetcode.com/problems/distinct-echo-substrings/) 1837
*   [1297. Maximum Number of Occurrences of a Substring](https://leetcode.com/problems/maximum-number-of-occurrences-of-a-substring/)
*   [2261. K Divisible Elements Subarrays](https://leetcode.com/problems/k-divisible-elements-subarrays/)
*   [3722. Lexicographically Smallest String after Reverse](https://leetcode.com/problems/lexicographically-smallest-string-after-reverse/)
*   [3213. Construct String with Minimum Cost](https://leetcode.com/problems/construct-string-with-minimum-cost/) 2171
*   [1367. Linked List in Binary Tree](https://leetcode.com/problems/linked-list-in-binary-tree/)
*   [1044. Longest Duplicate Substring](https://leetcode.com/problems/longest-duplicate-substring/) 2429
*   [718. Maximum Length of Repeated Subarray](https://leetcode.com/problems/maximum-length-of-repeated-subarray/)
*   [1923. Longest Common Subpath](https://leetcode.com/problems/longest-common-subpath/) 2661
*   [3292. Minimum Number of Valid Strings to Form Target Ii](https://leetcode.com/problems/minimum-number-of-valid-strings-to-form-target-ii/) 2662
*   [2168. Unique Substrings with Equal Digit Frequency](https://leetcode.com/problems/unique-substrings-with-equal-digit-frequency/) (Premium)
*   [1554. Strings Differ by One Character](https://leetcode.com/problems/strings-differ-by-one-character/) (Premium)
*   [1062. Longest Repeating Substring](https://leetcode.com/problems/longest-repeating-substring/) (Premium)

-------

    func smallestRepresentation(s string) string {
        n := len(s)
        s += s
        i := 0
        for j := 1; j < n; {
            k := 0
            for k < n && s[i+k] == s[j+k] {
                k++
            }
            if k >= n {
                break
            }

                // 此外：
                // ……
                j += k + 1
            } else {
                // 此外：
                // ……
                i, j = j, max(j, i+k)+1
            }
        }
        return s[i : i+n]
    }

*   [899. Orderly Queue](https://leetcode.com/problems/orderly-queue/) k\=1 ， O(n)
*   [3403. Find the Lexicographically Largest String from the Box I](https://leetcode.com/problems/find-the-lexicographically-largest-string-from-the-box-i/)
*   [1625. Lexicographically Smallest String after Applying Operations](https://leetcode.com/problems/lexicographically-smallest-string-after-applying-operations/)
*   [3406. Find the Lexicographically Largest String from the Box Ii](https://leetcode.com/problems/find-the-lexicographically-largest-string-from-the-box-ii/) (Premium)
*   [1708. Largest Subarray Length K](https://leetcode.com/problems/largest-subarray-length-k/) (Premium)

-----

*   见 [数据结构题单](https://leetcode.cn/circle/discuss/mOr1u6/) 第六章。

*   [1032. Stream of Characters](https://leetcode.com/problems/stream-of-characters/) 1970 ****
*   [面试题 17.17. Multi Search Lcci](https://leetcode.com/problems/multi-search-lcci/) ****
*   [1408. String Matching in an Array](https://leetcode.com/problems/string-matching-in-an-array/)
*   [3213. Construct String with Minimum Cost](https://leetcode.com/problems/construct-string-with-minimum-cost/) 2171
*   [2781. Length of the Longest Valid Substring](https://leetcode.com/problems/length-of-the-longest-valid-substring/) 2204
*   [3292. Minimum Number of Valid Strings to Form Target Ii](https://leetcode.com/problems/minimum-number-of-valid-strings-to-form-target-ii/) 2662

------------

*   [1163. Last Substring in Lexicographical Order](https://leetcode.com/problems/last-substring-in-lexicographical-order/) 1864
*   [1754. Largest Merge of Two Strings](https://leetcode.com/problems/largest-merge-of-two-strings/)
*   [2904. Shortest and Lexicographically Smallest Beautiful String](https://leetcode.com/problems/shortest-and-lexicographically-smallest-beautiful-string/)
*   [3722. Lexicographically Smallest String after Reverse](https://leetcode.com/problems/lexicographically-smallest-string-after-reverse/)
*   [3213. Construct String with Minimum Cost](https://leetcode.com/problems/construct-string-with-minimum-cost/) 2171
*   [1044. Longest Duplicate Substring](https://leetcode.com/problems/longest-duplicate-substring/) 2429
*   [718. Maximum Length of Repeated Subarray](https://leetcode.com/problems/maximum-length-of-repeated-subarray/)
*   [1923. Longest Common Subpath](https://leetcode.com/problems/longest-common-subpath/) 2661
*   [1408. String Matching in an Array](https://leetcode.com/problems/string-matching-in-an-array/)
*   [3729. Count Distinct Subarrays Divisible by K in Sorted Array](https://leetcode.com/problems/count-distinct-subarrays-divisible-by-k-in-sorted-array/)
*   [3076. Shortest Uncommon Substring in an Array](https://leetcode.com/problems/shortest-uncommon-substring-in-an-array/)
*   [3504. Longest Palindrome after Substring Concatenation Ii](https://leetcode.com/problems/longest-palindrome-after-substring-concatenation-ii/)
*   [1316. Distinct Echo Substrings](https://leetcode.com/problems/distinct-echo-substrings/)
*   [3388. Count Beautiful Splits in an Array](https://leetcode.com/problems/count-beautiful-splits-in-an-array/) O(n)
*   [2564. Substring Xor Queries](https://leetcode.com/problems/substring-xor-queries/)
*   [面试题 16.18. Pattern Matching Lcci](https://leetcode.com/problems/pattern-matching-lcci/)
*   [1698. Number of Distinct Substrings in a String](https://leetcode.com/problems/number-of-distinct-substrings-in-a-string/) (Premium)
*   [1062. Longest Repeating Substring](https://leetcode.com/problems/longest-repeating-substring/) (Premium)
*   [3135. Equalize Strings by Adding or Removing Characters at Ends](https://leetcode.com/problems/equalize-strings-by-adding-or-removing-characters-at-ends/) (Premium)

*   [792. Number of Matching Subsequences](https://leetcode.com/problems/number-of-matching-subsequences/) 1695
*   [514. Freedom Trail](https://leetcode.com/problems/freedom-trail/) 2400
*   [2014. Longest Subsequence Repeated K Times](https://leetcode.com/problems/longest-subsequence-repeated-k-times/) 2558
*   [1055. Shortest Way to Form String](https://leetcode.com/problems/shortest-way-to-form-string/) (Premium)
*   [727. Minimum Window Subsequence](https://leetcode.com/problems/minimum-window-subsequence/) (Premium)

十、其他
----

*   [3485. Longest Common Prefix of K Strings after Removal](https://leetcode.com/problems/longest-common-prefix-of-k-strings-after-removal/) 2290 LCP
*   [466. Count the Repetitions](https://leetcode.com/problems/count-the-repetitions/)
*   [3491. Phone Number Prefix](https://leetcode.com/problems/phone-number-prefix/) (Premium)


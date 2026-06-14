# Bit Manipulation

Problem list from [0x3F's LeetCode Study Plan](https://leetcode.cn/circle/discuss/dHn9Vk/) — Bit Manipulation (Basics / Properties / Bit Decomposition / Trial-and-Fill / Identities / Thinking).

> **Recommended reading first**: [From Set Theory to Bit Manipulation — A Summary of Common Bit Tricks](https://leetcode.cn/circle/discuss/CaOJ45/)

## I. Basics

- [3370. Smallest Number With All Set Bits](https://leetcode.com/problems/smallest-number-with-all-set-bits/) 1199
- [3827. Count Monobit Integers](https://leetcode.com/problems/count-monobit-integers/)
- [3226. Number of Bit Changes to Make Two Integers Equal](https://leetcode.com/problems/number-of-bit-changes-to-make-two-integers-equal/) 1247
- [1356. Sort Integers by The Number of 1 Bits](https://leetcode.com/problems/sort-integers-by-the-number-of-1-bits/) 1258
- [461. Hamming Distance](https://leetcode.com/problems/hamming-distance/) 1282
- [2220. Minimum Bit Flips to Convert Number](https://leetcode.com/problems/minimum-bit-flips-to-convert-number/) 1282 (same as 461)
- [1342. Number of Steps to Reduce a Number to Zero](https://leetcode.com/problems/number-of-steps-to-reduce-a-number-to-zero/) (achieve O(1))
- [476. Number Complement](https://leetcode.com/problems/number-complement/) (achieve O(1))
- [1009. Complement of Base 10 Integer](https://leetcode.com/problems/complement-of-base-10-integer/) (same as 476)
- [868. Binary Gap](https://leetcode.com/problems/binary-gap/) 1307
- [2917. Find the K-or of an Array](https://leetcode.com/problems/find-the-k-or-of-an-array/) 1389
- [693. Binary Number with Alternating Bits](https://leetcode.com/problems/binary-number-with-alternating-bits/)
- [2657. Find the Prefix Common Array of Two Arrays](https://leetcode.com/problems/find-the-prefix-common-array-of-two-arrays/)
- [Interview 05.01. Insert Into Bits LCCI](https://leetcode.com/problems/insert-into-bits-lcci/)
- [231. Power of Two](https://leetcode.com/problems/power-of-two/)
- [342. Power of Four](https://leetcode.com/problems/power-of-four/)
- [191. Number of 1 Bits](https://leetcode.com/problems/number-of-1-bits/)
- [338. Counting Bits](https://leetcode.com/problems/counting-bits/) (DP also works)
- [2595. Number of Even and Odd Bits](https://leetcode.com/problems/number-of-even-and-odd-bits/) (achieve O(1))
- [2154. Keep Multiplying Found Values by Two](https://leetcode.com/problems/keep-multiplying-found-values-by-two/) (O(n) time, O(1) space)
- [3211. Generate Binary Strings Without Adjacent Zeros](https://leetcode.com/problems/generate-binary-strings-without-adjacent-zeros/)

**Replace array operations with bitwise operations**:

- [3690. Split and Merge Array Transformation](https://leetcode.com/problems/split-and-merge-array-transformation/)

**Reverse a binary number**:

- [190. Reverse Bits](https://leetcode.com/problems/reverse-bits/)
- [3750. Minimum Number of Flips to Reverse Binary String](https://leetcode.com/problems/minimum-number-of-flips-to-reverse-binary-string/) 1289
- [3769. Sort Integers by Binary Reflection](https://leetcode.com/problems/sort-integers-by-binary-reflection/) 1364

## II. Properties of XOR (Exclusive OR)

Essentially, this is addition in the residue system modulo 2.

- [1486. XOR Operation in an Array](https://leetcode.com/problems/xor-operation-in-an-array/) 1181
- [1720. Decode XORed Array](https://leetcode.com/problems/decode-xored-array/) 1284
- [2433. Find The Original Array of Prefix Xor](https://leetcode.com/problems/find-the-original-array-of-prefix-xor/) 1367
- [1310. XOR Queries of a Subarray](https://leetcode.com/problems/xor-queries-of-a-subarray/) 1460
- [3702. Longest Subsequence With Non-Zero Bitwise XOR](https://leetcode.com/problems/longest-subsequence-with-non-zero-bitwise-xor/) 1489
- [2683. Neighboring Bitwise XOR](https://leetcode.com/problems/neighboring-bitwise-xor/) 1518
- [1829. Maximum XOR for Each Query](https://leetcode.com/problems/maximum-xor-for-each-query/) 1523
- [2997. Minimum Number of Operations to Make Array XOR Equal to K](https://leetcode.com/problems/minimum-number-of-operations-to-make-array-xor-equal-to-k/) 1525
- [1442. Count Triplets That Can Form Two Arrays of Equal XOR](https://leetcode.com/problems/count-triplets-that-can-form-two-arrays-of-equal-xor/) 1525
- [2429. Minimize XOR](https://leetcode.com/problems/minimize-xor/) 1532
- [2527. Find Xor-Beauty of Array](https://leetcode.com/problems/find-xor-beauty-of-array/) 1550
- [2317. Maximum XOR After Operations](https://leetcode.com/problems/maximum-xor-after-operations/) 1679
- [2588. Count the Number of Beautiful Subarrays](https://leetcode.com/problems/count-the-number-of-beautiful-subarrays/) 1697
- [2564. Substring XOR Queries](https://leetcode.com/problems/substring-xor-queries/) 1959
- [1734. Decode XORed Permutation](https://leetcode.com/problems/decode-xored-permutation/) 2024
- [2857. Count Pairs of Points With Distance k](https://leetcode.com/problems/count-pairs-of-points-with-distance-k/) 2082
- [1803. Count Pairs With XOR in a Range](https://leetcode.com/problems/count-pairs-with-xor-in-a-range/) 2479
- [3215. Count Triplets with Even XOR Set Bits II](https://leetcode.com/problems/count-triplets-with-even-xor-set-bits-ii/) 🔒

See also the "§6.4 0-1 Trie (XOR Trie)" section in the [Data Structures list](https://leetcode.cn/circle/discuss/mOr1u6/).

## III. Properties of AND / OR

The more numbers you AND together, the smaller the result.
The more numbers you OR together, the larger the result.

- [2980. Check if Bitwise OR Has Trailing Zeros](https://leetcode.com/problems/check-if-bitwise-or-has-trailing-zeros/) 1234
- [1318. Minimum Flips to Make a OR b Equal to c](https://leetcode.com/problems/minimum-flips-to-make-a-or-b-equal-to-c/) 1383
- [2419. Longest Subarray With Maximum Bitwise AND](https://leetcode.com/problems/longest-subarray-with-maximum-bitwise-and/) 1496
- [2871. Split Array Into Maximum Number of Subarrays](https://leetcode.com/problems/split-array-into-maximum-number-of-subarrays/) 1750
- [2401. Longest Nice Subarray](https://leetcode.com/problems/longest-nice-subarray/) 1750
- [2680. Maximum OR](https://leetcode.com/problems/maximum-or/) 1912 (O(1) extra space achievable)
- [3133. Minimum Array End](https://leetcode.com/problems/minimum-array-end/) 1935
- [3108. Minimum Cost Walk in Weighted Graph](https://leetcode.com/problems/minimum-cost-walk-in-weighted-graph/) 2109
- [3117. Minimum Sum of Values by Dividing Array](https://leetcode.com/problems/minimum-sum-of-values-by-dividing-array/) 2735
- [3125. Maximum Number That Makes Result of Bitwise AND Zero](https://leetcode.com/problems/maximum-number-that-makes-result-of-bitwise-and-zero/) 🔒

### AND/OR LogTrick

Note: some of the problems below can be solved in optimal O(n) time using a sliding window + stack.

- [3171. Find Subarray With Bitwise OR Closest to K](https://leetcode.com/problems/find-subarray-with-bitwise-or-closest-to-k/) (example)
- [1521. Find a Value of a Mysterious Function Closest to Target](https://leetcode.com/problems/find-a-value-of-a-mysterious-function-closest-to-target/) (same as 3171, OR → AND)
- [3097. Shortest Subarray With OR at Least K II](https://leetcode.com/problems/shortest-subarray-with-or-at-least-k-ii/) 1891
- [2411. Smallest Subarrays With Maximum Bitwise OR](https://leetcode.com/problems/smallest-subarrays-with-maximum-bitwise-or/) 1938
- [3209. Number of Subarrays With AND Value of K](https://leetcode.com/problems/number-of-subarrays-with-and-value-of-k/) 2050
- [898. Bitwise ORs of Subarrays](https://leetcode.com/problems/bitwise-ors-of-subarrays/)

### GCD LogTrick

- [2447. Number of Subarrays With GCD Equal to K](https://leetcode.com/problems/number-of-subarrays-with-gcd-equal-to-k/) (non-brute-force)
- [2654. Minimum Number of Operations to Make All Array Elements Equal to 1](https://leetcode.com/problems/minimum-number-of-operations-to-make-all-array-elements-equal-to-1/) (non-brute-force)
- [3605. Minimum Stability Factor of Array](https://leetcode.com/problems/minimum-stability-factor-of-array/) 2410
- [3574. Maximize Subarray GCD Score](https://leetcode.com/problems/maximize-subarray-gcd-score/) (non-brute-force)
- [2941. Maximum GCD-Sum of a Subarray](https://leetcode.com/problems/maximum-gcd-sum-of-a-subarray/) 🔒

## IV. Bit Decomposition / Contribution Technique

- [477. Total Hamming Distance](https://leetcode.com/problems/total-hamming-distance/)
- [1863. Sum of All Subset XOR Totals](https://leetcode.com/problems/sum-of-all-subset-xor-totals/) (O(n) achievable)
- [2425. Bitwise XOR of All Pairings](https://leetcode.com/problems/bitwise-xor-of-all-pairings/) 1622 (O(n+m) achievable)
- [2275. Largest Combination With Bitwise AND Greater Than Zero](https://leetcode.com/problems/largest-combination-with-bitwise-and-greater-than-zero/) 1642
- [1835. Find XOR Sum of All Pairs Bitwise AND](https://leetcode.com/problems/find-xor-sum-of-all-pairs-bitwise-and/) 1825 (identity approach also works)
- [3688. Bitwise OR of Even Numbers in an Array](https://leetcode.com/problems/bitwise-or-of-even-numbers-in-an-array/) (see the thinking question in the solution)
- [2505. Bitwise OR of All Subsequence Sums](https://leetcode.com/problems/bitwise-or-of-all-subsequence-sums/) 🔒

**Decimal digit decomposition**:

- [3153. Sum of Digit Differences of All Pairs](https://leetcode.com/problems/sum-of-digit-differences-of-all-pairs/) 1645

## V. Trial-and-Fill (Greedy Bit Construction)

- [421. Maximum XOR of Two Numbers in an Array](https://leetcode.com/problems/maximum-xor-of-two-numbers-in-an-array/)
- [3806. Maximum Bitwise AND After Increment Operations](https://leetcode.com/problems/maximum-bitwise-and-after-increment-operations/) 2259
- [2935. Maximum Strong Pair XOR II](https://leetcode.com/problems/maximum-strong-pair-xor-ii/) 2349
- [3007. Maximum Number That Sum of the Prices Is Less Than or Equal to K](https://leetcode.com/problems/maximum-number-that-sum-of-the-prices-is-less-than-or-equal-to-k/)
- [3145. Find Products of Elements of Big Array](https://leetcode.com/problems/find-products-of-elements-of-big-array/) 2859 (similar to Champernowne number)
- [3022. Minimize OR of Remaining Elements Using Operations](https://leetcode.com/problems/minimize-or-of-remaining-elements-using-operations/) 2918
- [3287. Find the Maximum Sequence Value of Array](https://leetcode.com/problems/find-the-maximum-sequence-value-of-array/) (O(nU log U), where U=27)
- [3344. Maximum Sized Array](https://leetcode.com/problems/maximum-sized-array/) 🔒

## VI. Identities

- [1835. Find XOR Sum of All Pairs Bitwise AND](https://leetcode.com/problems/find-xor-sum-of-all-pairs-bitwise-and/) 1825
- [2354. Number of Excellent Pairs](https://leetcode.com/problems/number-of-excellent-pairs/) 2076

## VII. Linear Basis

- [3681. Maximum XOR of Subsequences](https://leetcode.com/problems/maximum-xor-of-subsequences/) (template problem)
- [3630. Partition Array for Maximum XOR and AND](https://leetcode.com/problems/partition-array-for-maximum-xor-and-and/) 2744

## VIII. Thinking Problems

Greedy, brain teasers, etc.

- [2546. Apply Bitwise Operations to Make Strings Equal](https://leetcode.com/problems/apply-bitwise-operations-to-make-strings-equal/) 1605
- [1558. Minimum Numbers of Function Calls to Make Target Array](https://leetcode.com/problems/minimum-numbers-of-function-calls-to-make-target-array/) 1637
- [2571. Minimum Operations to Reduce an Integer to 0](https://leetcode.com/problems/minimum-operations-to-reduce-an-integer-to-0/) 1649 (clever conclusion)
- [3315. Construct the Minimum Bitwise Array II](https://leetcode.com/problems/construct-the-minimum-bitwise-array-ii/) 1715
- [2568. Minimum Impossible OR](https://leetcode.com/problems/minimum-impossible-or/) 1754
- [3644. Maximum K to Sort a Permutation](https://leetcode.com/problems/maximum-k-to-sort-a-permutation/) 1775
- [2509. Cycle Length Queries in a Tree](https://leetcode.com/problems/cycle-length-queries-in-a-tree/) 1948
- [2939. Maximum Xor Product](https://leetcode.com/problems/maximum-xor-product/) 2128
- [2749. Minimum Operations to Make the Integer Zero](https://leetcode.com/problems/minimum-operations-to-make-the-integer-zero/) 2132
- [2835. Minimum Operations to Form Subsequence With Target Sum](https://leetcode.com/problems/minimum-operations-to-form-subsequence-with-target-sum/) 2207
- [2897. Apply Operations on Array to Maximize Sum of Squares](https://leetcode.com/problems/apply-operations-on-array-to-maximize-sum-of-squares/) 2301
- [810. Chalkboard XOR Game](https://leetcode.com/problems/chalkboard-xor-game/) 2341
- [3064. Guess the Number Using Bitwise Questions I](https://leetcode.com/problems/guess-the-number-using-bitwise-questions-i/) 🔒
- [3094. Guess the Number Using Bitwise Questions II](https://leetcode.com/problems/guess-the-number-using-bitwise-questions-ii/) 🔒

## IX. Others

- [136. Single Number](https://leetcode.com/problems/single-number/)
- [260. Single Number III](https://leetcode.com/problems/single-number-iii/)
- [2965. Find Missing and Repeated Values](https://leetcode.com/problems/find-missing-and-repeated-values/)
- [137. Single Number II](https://leetcode.com/problems/single-number-ii/)
- [645. Set Mismatch](https://leetcode.com/problems/set-mismatch/)
- [371. Sum of Two Integers](https://leetcode.com/problems/sum-of-two-integers/)
- [201. Bitwise AND of Numbers Range](https://leetcode.com/problems/bitwise-and-of-numbers-range/)
- [2438. Range Product Queries of Powers](https://leetcode.com/problems/range-product-queries-of-powers/) 1610
- [1680. Concatenation of Consecutive Binary Numbers](https://leetcode.com/problems/concatenation-of-consecutive-binary-numbers/) 1630
- [1261. Find Elements in a Contaminated Binary Tree](https://leetcode.com/problems/find-elements-in-a-contaminated-binary-tree/) (O(1) extra space)
- [89. Gray Code](https://leetcode.com/problems/gray-code/)
- [1238. Circular Permutation in Binary Representation](https://leetcode.com/problems/circular-permutation-in-binary-representation/) 1775
- [3766. Minimum Operations to Make Binary Palindrome](https://leetcode.com/problems/minimum-operations-to-make-binary-palindrome/) (non-brute-force)
- [3782. Last Remaining Integer After Alternating Deletion Operations](https://leetcode.com/problems/last-remaining-integer-after-alternating-deletion-operations/) 2074
- [390. Elimination Game](https://leetcode.com/problems/elimination-game/) (similar to 3782)
- [982. Triples with Bitwise AND Equal To Zero](https://leetcode.com/problems/triples-with-bitwise-and-equal-to-zero/) 2085
- [3307. Find the K-th Character in String Game II](https://leetcode.com/problems/find-the-k-th-character-in-string-game-ii/) 2232
- [1611. Minimum One Bit Operations to Make Integers Zero](https://leetcode.com/problems/minimum-one-bit-operations-to-make-integers-zero/) 2345
- [3514. Number of Unique XOR Triplets II](https://leetcode.com/problems/number-of-unique-xor-triplets-ii/) (Fast Walsh–Hadamard Transform / FWT)
- [LCP 81. NAND Puzzle](https://leetcode.cn/problems/ryfUiz/)
- [751. IP to CIDR](https://leetcode.com/problems/ip-to-cidr/) 🔒
- [3595. Once Twice](https://leetcode.com/problems/once-twice/) 🔒 (combines the ideas of 137 and 260)
- [3141. Maximum Hamming Distances](https://leetcode.com/problems/maximum-hamming-distances/) 🔒

## Related Lists

- [Data Structures list](https://leetcode.cn/circle/discuss/mOr1u6/) — the "§6.4 0-1 Trie (XOR Trie)" section.
- [Linked List, Binary Tree and Backtracking](https://leetcode.cn/circle/discuss/K0n2gO/) — some backtracking problems can be solved with binary enumeration.

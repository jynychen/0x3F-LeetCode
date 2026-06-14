# Dynamic Programming

Problem list from [0x3F's LeetCode Study Plan](https://leetcode.cn/circle/discuss/tXLS3i/) — Dynamic Programming (Introduction / Grid / Knapsack / Linear / Partition / State Machine / Interval / Bitmask / Digit / Optimization / Tree / Graph / Game / Probability).

Memoized search (top-down) is the recommended starting point for beginners; after writing it, also write the bottom-up recurrence, which enables further time/space optimization. Within each section, problems are sorted by difficulty rating (the number on the right).

## I. Introduction to DP

### §1.1 Climbing Stairs

- [70. Climbing Stairs](https://leetcode.com/problems/climbing-stairs/)
- [746. Min Cost Climbing Stairs](https://leetcode.com/problems/min-cost-climbing-stairs/) ~1500
- [3693. Climbing Stairs II](https://leetcode.com/problems/climbing-stairs-ii/) 1560 (note: although the statement says 1-indexed, the input array is still 0-indexed)
- [377. Combination Sum IV](https://leetcode.com/problems/combination-sum-iv/) ~1600
- [2466. Count Ways To Build Good Strings](https://leetcode.com/problems/count-ways-to-build-good-strings/) 1694
- [2266. Count Number of Texts](https://leetcode.com/problems/count-number-of-texts/) 1857
- [2533. Number of Good Binary Strings](https://leetcode.com/problems/number-of-good-binary-strings/) 🔒 (same as 2466)

### §1.2 House Robber

- [198. House Robber](https://leetcode.com/problems/house-robber/)
- [213. House Robber II](https://leetcode.com/problems/house-robber-ii/) (circular array)
- [2320. Count Number of Ways to Place Houses](https://leetcode.com/problems/count-number-of-ways-to-place-houses/) 1608
- [3840. House Robber V](https://leetcode.com/problems/house-robber-v/) 1619
- [740. Delete and Earn](https://leetcode.com/problems/delete-and-earn/)
- [3186. Maximum Total Damage With Spell Casting](https://leetcode.com/problems/maximum-total-damage-with-spell-casting/) 1841

**Mind Extensions**:

- [2140. Solving Questions With Brainpower](https://leetcode.com/problems/solving-questions-with-brainpower/) 1709

### §1.3 Maximum Subarray Sum (Maximum Subsegment Sum)

- [53. Maximum Subarray](https://leetcode.com/problems/maximum-subarray/) (see the thinking exercise in my solution)
- [2606. Find the Substring With Maximum Cost](https://leetcode.com/problems/find-the-substring-with-maximum-cost/) 1422
- [1749. Maximum Absolute Sum of Any Subarray](https://leetcode.com/problems/maximum-absolute-sum-of-any-subarray/) 1542
- [1191. K-Concatenation Maximum Sum](https://leetcode.com/problems/k-concatenation-maximum-sum/) 1748
- [918. Maximum Sum Circular Subarray](https://leetcode.com/problems/maximum-sum-circular-subarray/) 1777 (circular array)
- [2321. Maximum Score Of Spliced Array](https://leetcode.com/problems/maximum-score-of-spliced-array/) 1791

**Mind Extensions**:

- [152. Maximum Product Subarray](https://leetcode.com/problems/maximum-product-subarray/)
- [1186. Maximum Subarray Sum with One Deletion](https://leetcode.com/problems/maximum-subarray-sum-with-one-deletion/) 1799
- [3381. Maximum Subarray Sum With Length Divisible by K](https://leetcode.com/problems/maximum-subarray-sum-with-length-divisible-by-k/) 1943
- [3938. Maximum Path Intersection Sum in a Grid](https://leetcode.com/problems/maximum-path-intersection-sum-in-a-grid/) 2252

### Thinking Exercise

After finishing this chapter, think: when should you return f[n], and when should you return max(f)?

## II. Grid DP

For some 2D DP problems (e.g. knapsack, LCS), drawing the DP matrix shows that the transitions can be viewed as moving on a grid. Practicing concrete grid DP first makes the more abstract 2D DP easier (for example, why the space-optimized 0-1 knapsack iterates in reverse).

### §2.1 Basics

- [64. Minimum Path Sum](https://leetcode.com/problems/minimum-path-sum/)
- [62. Unique Paths](https://leetcode.com/problems/unique-paths/)
- [63. Unique Paths II](https://leetcode.com/problems/unique-paths-ii/)
- [120. Triangle](https://leetcode.com/problems/triangle/)
- [3393. Count Paths With the Given XOR Value](https://leetcode.com/problems/count-paths-with-the-given-xor-value/) 1573
- [931. Minimum Falling Path Sum](https://leetcode.com/problems/minimum-falling-path-sum/) 1573
- [3603. Minimum Cost Path with Alternating Directions II](https://leetcode.com/problems/minimum-cost-path-with-alternating-directions-ii/) 1639
- [2304. Minimum Path Cost in a Grid](https://leetcode.com/problems/minimum-path-cost-in-a-grid/) 1658
- [1289. Minimum Falling Path Sum II](https://leetcode.com/problems/minimum-falling-path-sum-ii/) 1697 (optimization)
- [3882. Minimum XOR Path in a Grid](https://leetcode.com/problems/minimum-xor-path-in-a-grid/) 1771
- [3418. Maximum Amount of Money Robot Can Earn](https://leetcode.com/problems/maximum-amount-of-money-robot-can-earn/) 1798
- [3742. Maximum Path Score in a Grid](https://leetcode.com/problems/maximum-path-score-in-a-grid/) 1804

**Mind Extensions**:

- [2684. Maximum Number of Moves in a Grid](https://leetcode.com/problems/maximum-number-of-moves-in-a-grid/) 1626
- [1824. Minimum Sideway Jumps](https://leetcode.com/problems/minimum-sideway-jumps/) 1778

### §2.2 Advanced

- [1594. Maximum Non Negative Product in a Matrix](https://leetcode.com/problems/maximum-non-negative-product-in-a-matrix/) 1807
- [1301. Number of Paths with Max Score](https://leetcode.com/problems/number-of-paths-with-max-score/) 1853
- [3665. Twisted Mirror Path Count](https://leetcode.com/problems/twisted-mirror-path-count/) 1883
- [2435. Paths in Matrix Whose Sum Is Divisible by K](https://leetcode.com/problems/paths-in-matrix-whose-sum-is-divisible-by-k/) 1952
- [174. Dungeon Game](https://leetcode.com/problems/dungeon-game/)
- [329. Longest Increasing Path in a Matrix](https://leetcode.com/problems/longest-increasing-path-in-a-matrix/)
- [2328. Number of Increasing Paths in a Grid](https://leetcode.com/problems/number-of-increasing-paths-in-a-grid/) 2001
- [2267. Check if There Is a Valid Parentheses String Path](https://leetcode.com/problems/check-if-there-is-a-valid-parentheses-string-path/) 2085
- [1937. Maximum Number of Points with Cost](https://leetcode.com/problems/maximum-number-of-points-with-cost/) 2106
- [3363. Find the Maximum Number of Fruits Collected](https://leetcode.com/problems/find-the-maximum-number-of-fruits-collected/) (actual difficulty 2200)
- [1463. Cherry Pickup II](https://leetcode.com/problems/cherry-pickup-ii/)
- [741. Cherry Pickup](https://leetcode.com/problems/cherry-pickup/)
- [3459. Length of Longest V-Shaped Diagonal Segment](https://leetcode.com/problems/length-of-longest-v-shaped-diagonal-segment/) 2337 (state design)
- [2510. Check if There is a Path With Equal Number of 0's and 1's](https://leetcode.com/problems/check-if-there-is-a-path-with-equal-number-of-0s-and-1s/) 🔒

## III. Knapsack

### §3.1 0-1 Knapsack

Each item can be chosen at most once — take it or skip it. So 0-1 knapsack represents the "take or skip" pattern.

For the "choose which one" pattern, see §4.2 Longest Increasing Subsequence.

- [416. Partition Equal Subset Sum](https://leetcode.com/problems/partition-equal-subset-sum/)
- [494. Target Sum](https://leetcode.com/problems/target-sum/)
- [2915. Length of the Longest Subsequence That Sums to Target](https://leetcode.com/problems/length-of-the-longest-subsequence-that-sums-to-target/) 1659
- [3877. Minimum Removals to Achieve Target XOR](https://leetcode.com/problems/minimum-removals-to-achieve-target-xor/) 1745
- [2787. Ways to Express an Integer as Sum of Powers](https://leetcode.com/problems/ways-to-express-an-integer-as-sum-of-powers/) 1818

**Advanced**:

- [474. Ones and Zeroes](https://leetcode.com/problems/ones-and-zeroes/) (2D knapsack)
- [3946. Maximum Number of Items From Sale I](https://leetcode.com/problems/maximum-number-of-items-from-sale-i/) 1728
- [3180. Maximum Total Reward Using Operations I](https://leetcode.com/problems/maximum-total-reward-using-operations-i/) 1849
- [3489. Zero Array Transformation IV](https://leetcode.com/problems/zero-array-transformation-iv/) 2068
- [1774. Closest Dessert Cost](https://leetcode.com/problems/closest-dessert-cost/) (non-brute-force approach)
- [3685. Subsequence Sum After Capping Elements](https://leetcode.com/problems/subsequence-sum-after-capping-elements/) 2073
- [1049. Last Stone Weight II](https://leetcode.com/problems/last-stone-weight-ii/) 2092
- [879. Profitable Schemes](https://leetcode.com/problems/profitable-schemes/) 2204
- [3082. Find the Sum of the Power of All Subsequences](https://leetcode.com/problems/find-the-sum-of-the-power-of-all-subsequences/) 2242
- [956. Tallest Billboard](https://leetcode.com/problems/tallest-billboard/) 2381
- [2518. Number of Great Partitions](https://leetcode.com/problems/number-of-great-partitions/) 2415
- [2742. Painting the Walls](https://leetcode.com/problems/painting-the-walls/) 2425 (at least fill)
- [3287. Find the Maximum Sequence Value of Array](https://leetcode.com/problems/find-the-maximum-sequence-value-of-array/) 2545
- [3181. Maximum Total Reward Using Operations II](https://leetcode.com/problems/maximum-total-reward-using-operations-ii/) 2688 (bitset optimization)
- [LCP 47. Entrance Security Check](https://leetcode.cn/problems/oPs9Bm/)
- [2291. Maximum Profit From Trading Stocks](https://leetcode.com/problems/maximum-profit-from-trading-stocks/) 🔒
- [2431. Maximize Total Tastiness of Purchased Fruits](https://leetcode.com/problems/maximize-total-tastiness-of-purchased-fruits/) 🔒
- [3647. Maximum Weight in Two Bags](https://leetcode.com/problems/maximum-weight-in-two-bags/) 🔒 (multiple knapsack)
- [2189. Number of Ways to Build House of Cards](https://leetcode.com/problems/number-of-ways-to-build-house-of-cards/) 🔒

### §3.2 Unbounded Knapsack

Items can be chosen repeatedly, with no count limit.

- [322. Coin Change](https://leetcode.com/problems/coin-change/)
- [518. Coin Change II](https://leetcode.com/problems/coin-change-ii/)
- [279. Perfect Squares](https://leetcode.com/problems/perfect-squares/)
- [3610. Minimum Number of Primes to Sum to Target](https://leetcode.com/problems/minimum-number-of-primes-to-sum-to-target/) 🔒
- [3183. The Number of Ways to Make the Sum](https://leetcode.com/problems/the-number-of-ways-to-make-the-sum/) 🔒 (mixed knapsack)

**Mind Extensions**:

- [3592. Inverse Coin Change](https://leetcode.com/problems/inverse-coin-change/) 1701
- [1449. Form Largest Integer With Digits That Add up to Target](https://leetcode.com/problems/form-largest-integer-with-digits-that-add-up-to-target/) 1927

### §3.3 Bounded Knapsack (Optional)

Items can be chosen repeatedly, with a count limit.

**Counting schemes**:

Note: counting-scheme problems cannot use binary optimization. For example, choosing 3 from 6 identical items has only one way, but binary optimization splits 6 into 1+2+3, giving two ways.

To optimize, consider a congruence prefix sum.

- [2585. Number of Ways to Earn Points](https://leetcode.com/problems/number-of-ways-to-earn-points/) 1910
- [3333. Find the Original Typed String II](https://leetcode.com/problems/find-the-original-typed-string-ii/) 2629
- [2902. Count of Sub-Multisets With Bounded Sum](https://leetcode.com/problems/count-of-sub-multisets-with-bounded-sum/) 2759

**Binary optimization**:

- [3489. Zero Array Transformation IV](https://leetcode.com/problems/zero-array-transformation-iv/)

### §3.4 Grouped Knapsack

Within each group, choose at most / exactly one item.

- [1155. Number of Dice Rolls With Target Sum](https://leetcode.com/problems/number-of-dice-rolls-with-target-sum/) 1654
- [1981. Minimize the Difference Between Target and Chosen Elements](https://leetcode.com/problems/minimize-the-difference-between-target-and-chosen-elements/) 2010
- [2218. Maximum Value of K Coins From Piles](https://leetcode.com/problems/maximum-value-of-k-coins-from-piles/) 2158

### §3.5 Tree Knapsack (Optional)

> Note: currently LeetCode only has dependency-free knapsack, with time complexity O(nW^2), where n is the number of tree nodes and W is the capacity. With dependencies it can be optimized to O(nW).

- [3939. Count Non Adjacent Subsets in a Rooted Tree](https://leetcode.com/problems/count-non-adjacent-subsets-in-a-rooted-tree/) 2354
- [3562. Maximum Profit from Trading Stocks with Discounts](https://leetcode.com/problems/maximum-profit-from-trading-stocks-with-discounts/) 2458

## IV. Classic Linear DP

### §4.1 Longest Common Subsequence (LCS)

Generally define f[i][j] as the result for (s[:i], t[:j]).

#### §4.1.1 Basics

- [1143. Longest Common Subsequence](https://leetcode.com/problems/longest-common-subsequence/)
- [583. Delete Operation for Two Strings](https://leetcode.com/problems/delete-operation-for-two-strings/)
- [712. Minimum ASCII Delete Sum for Two Strings](https://leetcode.com/problems/minimum-ascii-delete-sum-for-two-strings/)
- [72. Edit Distance](https://leetcode.com/problems/edit-distance/)
- [1035. Uncrossed Lines](https://leetcode.com/problems/uncrossed-lines/) 1806
- [1458. Max Dot Product of Two Subsequences](https://leetcode.com/problems/max-dot-product-of-two-subsequences/) 1824 (how to express "non-empty subsequence")
- [3836. Maximum Score Using Exactly K Pairs](https://leetcode.com/problems/maximum-score-using-exactly-k-pairs/) 1988

**Mind Extensions**:

- [718. Maximum Length of Repeated Subarray](https://leetcode.com/problems/maximum-length-of-repeated-subarray/)

#### §4.1.2 Advanced

- [3290. Maximum Multiplication Score](https://leetcode.com/problems/maximum-multiplication-score/) 1692
- [115. Distinct Subsequences](https://leetcode.com/problems/distinct-subsequences/)
- [3628. Maximum Number of Subsequences After One Inserting](https://leetcode.com/problems/maximum-number-of-subsequences-after-one-inserting/) 1754
- [3316. Find Maximum Removals From Source String](https://leetcode.com/problems/find-maximum-removals-from-source-string/) 2062
- [1639. Number of Ways to Form a Target String Given a Dictionary](https://leetcode.com/problems/number-of-ways-to-form-a-target-string-given-a-dictionary/) 2082
- [97. Interleaving String](https://leetcode.com/problems/interleaving-string/)
- [1092. Shortest Common Supersequence](https://leetcode.com/problems/shortest-common-supersequence/)
- [44. Wildcard Matching](https://leetcode.com/problems/wildcard-matching/)
- [10. Regular Expression Matching](https://leetcode.com/problems/regular-expression-matching/)

**Thinking exercise**:

### §4.2 Longest Increasing Subsequence (LIS)

There are several approaches:

- Enumerate which element to take.

- Binary search.

- Compute the LCS of a and its sorted copy sortedA (use LCS to find LIS).

- Data-structure optimization (see problem 2407).

#### §4.2.1 Basics

- [300. Longest Increasing Subsequence](https://leetcode.com/problems/longest-increasing-subsequence/)
- [334. Increasing Triplet Subsequence](https://leetcode.com/problems/increasing-triplet-subsequence/)
- [2826. Sorting Three Groups](https://leetcode.com/problems/sorting-three-groups/) 1721
- [1964. Find the Longest Valid Obstacle Course at Each Position](https://leetcode.com/problems/find-the-longest-valid-obstacle-course-at-each-position/) 1933
- [2111. Minimum Operations to Make the Array K-Increasing](https://leetcode.com/problems/minimum-operations-to-make-the-array-k-increasing/) 1941 (includes an advanced variant)

#### §4.2.2 Advanced

- [3825. Longest Strictly Increasing Subsequence With Non-Zero Bitwise AND](https://leetcode.com/problems/longest-strictly-increasing-subsequence-with-non-zero-bitwise-and/) 1846
- [1671. Minimum Number of Removals to Make Mountain Array](https://leetcode.com/problems/minimum-number-of-removals-to-make-mountain-array/) 1913
- [354. Russian Doll Envelopes](https://leetcode.com/problems/russian-doll-envelopes/)
- [1626. Best Team With No Conflicts](https://leetcode.com/problems/best-team-with-no-conflicts/) 2027
- [1691. Maximum Height by Stacking Cuboids](https://leetcode.com/problems/maximum-height-by-stacking-cuboids/) 2172
- [960. Delete Columns to Make Sorted III](https://leetcode.com/problems/delete-columns-to-make-sorted-iii/) 2247
- [3920. Maximize Fixed Points After Deletions](https://leetcode.com/problems/maximize-fixed-points-after-deletions/) 2264
- [2407. Longest Increasing Subsequence II](https://leetcode.com/problems/longest-increasing-subsequence-ii/) 2280
- [673. Number of Longest Increasing Subsequence](https://leetcode.com/problems/number-of-longest-increasing-subsequence/)
- [1187. Make Array Strictly Increasing](https://leetcode.com/problems/make-array-strictly-increasing/) 2316
- [1713. Minimum Operations to Make a Subsequence](https://leetcode.com/problems/minimum-operations-to-make-a-subsequence/) 2351 (use LIS to compute LCS)
- [3288. Length of the Longest Increasing Path](https://leetcode.com/problems/length-of-the-longest-increasing-path/) 2450

**Mind Extensions**:

- [368. Largest Divisible Subset](https://leetcode.com/problems/largest-divisible-subset/) ~1800
- [2901. Longest Unequal Adjacent Groups Subsequence II](https://leetcode.com/problems/longest-unequal-adjacent-groups-subsequence-ii/) 1899

**Thinking exercise**:

## V. Partition DP

### §5.1 Decide Whether a Partition Exists

Generally define f[i] as whether the length-i prefix a[:i] can be partitioned.

Enumerate the left endpoint L of the last subarray, transition from f[L] to f[i], and check whether a[L:i] meets the requirement.

- [2369. Check if There is a Valid Partition For The Array](https://leetcode.com/problems/check-if-there-is-a-valid-partition-for-the-array/) 1780
- [139. Word Break](https://leetcode.com/problems/word-break/)

### §5.2 Optimal Partition

Compute the minimum (maximum) number of parts, the best partition score, etc.

Generally define f[i] as the minimum (maximum) number of subarrays the length-i prefix a[:i] is split into under the constraints (or as the number of partition schemes).

Enumerate the left endpoint L of the last subarray, transition from f[L] to f[i], and consider the effect of a[L:i] on the optimum.

- [132. Palindrome Partitioning II](https://leetcode.com/problems/palindrome-partitioning-ii/)
- [2707. Extra Characters in a String](https://leetcode.com/problems/extra-characters-in-a-string/) 1736
- [3196. Maximize Total Cost of Alternating Subarrays](https://leetcode.com/problems/maximize-total-cost-of-alternating-subarrays/) 1847 (also has a state-machine DP approach)
- [2767. Partition String Into Minimum Beautiful Substrings](https://leetcode.com/problems/partition-string-into-minimum-beautiful-substrings/) 1865
- [91. Decode Ways](https://leetcode.com/problems/decode-ways/)
- [639. Decode Ways II](https://leetcode.com/problems/decode-ways-ii/)
- [LCR 165. Decrypt Numbers](https://leetcode.cn/problems/ba-shu-zi-fan-yi-cheng-zi-fu-chuan-lcof/)
- [1043. Partition Array for Maximum Sum](https://leetcode.com/problems/partition-array-for-maximum-sum/) 1916
- [3144. Minimum Substring Partition of Equal Character Frequency](https://leetcode.com/problems/minimum-substring-partition-of-equal-character-frequency/) 1917
- [1416. Restore The Array](https://leetcode.com/problems/restore-the-array/) 1920
- [2472. Maximum Number of Non-overlapping Palindrome Substrings](https://leetcode.com/problems/maximum-number-of-non-overlapping-palindrome-substrings/) 2013
- [1105. Filling Bookcase Shelves](https://leetcode.com/problems/filling-bookcase-shelves/) 2014
- [2547. Minimum Cost to Split an Array](https://leetcode.com/problems/minimum-cost-to-split-an-array/) 2020
- [3578. Count Partitions With Max-Min Difference at Most K](https://leetcode.com/problems/count-partitions-with-max-min-difference-at-most-k/) 2033 (optimization)
- [2430. Maximum Deletions on a String](https://leetcode.com/problems/maximum-deletions-on-a-string/) 2102
- [2463. Minimum Total Distance Traveled](https://leetcode.com/problems/minimum-total-distance-traveled/) 2454
- [3579. Minimum Steps to Convert String with Operations](https://leetcode.com/problems/minimum-steps-to-convert-string-with-operations/) 2493 (can achieve O(n^2))
- [3500. Minimum Cost to Divide Array Into Subarrays](https://leetcode.com/problems/minimum-cost-to-divide-array-into-subarrays/) 2569 (formula transformation)
- [2977. Minimum Cost to Convert String II](https://leetcode.com/problems/minimum-cost-to-convert-string-ii/) 2696
- [3441. Minimum Cost Good Caption](https://leetcode.com/problems/minimum-cost-good-caption/) 2765
- [2052. Minimum Cost to Separate Sentence Into Rows](https://leetcode.com/problems/minimum-cost-to-separate-sentence-into-rows/) 🔒
- [2464. Minimum Subarrays in a Valid Split](https://leetcode.com/problems/minimum-subarrays-in-a-valid-split/) 🔒

### §5.3 Partition with a Constrained Number of Parts

Split the array into (exactly / at most) k contiguous subarrays and compute an optimum related to these subarrays.

Generally define f[i][j] as the optimum of splitting the length-j prefix a[:j] into i contiguous subarrays.

Enumerate the left endpoint L of the last subarray, transition from f[i-1][L] to f[i][j], and consider the effect of a[L:j] on the optimum.

> Note: for exact-count partition DP, controlling the inner-loop bounds can reduce the time complexity from O(nk) to O((n-k)k). See problem 3473.

- [813. Largest Sum of Averages](https://leetcode.com/problems/largest-sum-of-averages/) 1937
- [3599. Partition Array to Minimize XOR](https://leetcode.com/problems/partition-array-to-minimize-xor/) 1955 (more than one approach)
- [410. Split Array Largest Sum](https://leetcode.com/problems/split-array-largest-sum/)
- [1278. Palindrome Partitioning III](https://leetcode.com/problems/palindrome-partitioning-iii/) 1979
- [1745. Palindrome Partitioning IV](https://leetcode.com/problems/palindrome-partitioning-iv/)
- [1335. Minimum Difficulty of a Job Schedule](https://leetcode.com/problems/minimum-difficulty-of-a-job-schedule/) 2035
- [1473. Paint House III](https://leetcode.com/problems/paint-house-iii/) 2056
- [2209. Minimum White Tiles After Covering With Carpets](https://leetcode.com/problems/minimum-white-tiles-after-covering-with-carpets/) 2106
- [1478. Allocate Mailboxes](https://leetcode.com/problems/allocate-mailboxes/) 2190
- [3473. Sum of K Subarrays With Length at Least M](https://leetcode.com/problems/sum-of-k-subarrays-with-length-at-least-m/) 2274 (optimization)
- [1959. Minimum Total Space Wasted With K Resizing Operations](https://leetcode.com/problems/minimum-total-space-wasted-with-k-resizing-operations/) 2310
- [2478. Number of Beautiful Partitions](https://leetcode.com/problems/number-of-beautiful-partitions/) 2344
- [3538. Merge Operations for Minimum Travel Time](https://leetcode.com/problems/merge-operations-for-minimum-travel-time/) 2461 (adjacency-dependent)
- [3505. Minimum Operations to Make Elements Within K Subarrays Equal](https://leetcode.com/problems/minimum-operations-to-make-elements-within-k-subarrays-equal/) 2539
- [3077. Maximum Strength of K Disjoint Subarrays](https://leetcode.com/problems/maximum-strength-of-k-disjoint-subarrays/) 2557 (more than one approach)
- [2911. Minimum Changes to Make K Semi-palindromes](https://leetcode.com/problems/minimum-changes-to-make-k-semi-palindromes/) 2608
- [3117. Minimum Sum of Values by Dividing Array](https://leetcode.com/problems/minimum-sum-of-values-by-dividing-array/) 2735

## VI. State Machine DP

Generally define f[i][j] as the optimum for prefix a[:i] in state j. j is usually small.

### §6.1 Buy and Sell Stock

- [121. Best Time to Buy and Sell Stock](https://leetcode.com/problems/best-time-to-buy-and-sell-stock/) (1 transaction)
- [122. Best Time to Buy and Sell Stock II](https://leetcode.com/problems/best-time-to-buy-and-sell-stock-ii/) (unlimited transactions)
- [123. Best Time to Buy and Sell Stock III](https://leetcode.com/problems/best-time-to-buy-and-sell-stock-iii/) (2 transactions)
- [188. Best Time to Buy and Sell Stock IV](https://leetcode.com/problems/best-time-to-buy-and-sell-stock-iv/) (k transactions)
- [3573. Best Time to Buy and Sell Stock V](https://leetcode.com/problems/best-time-to-buy-and-sell-stock-v/) (k transactions 1777)
- [309. Best Time to Buy and Sell Stock with Cooldown](https://leetcode.com/problems/best-time-to-buy-and-sell-stock-with-cooldown/) (unlimited transactions)
- [714. Best Time to Buy and Sell Stock with Transaction Fee](https://leetcode.com/problems/best-time-to-buy-and-sell-stock-with-transaction-fee/) (unlimited transactions)

### §6.2 Basics

- [198. House Robber](https://leetcode.com/problems/house-robber/)
- [3259. Maximum Energy Boost From Two Drinks](https://leetcode.com/problems/maximum-energy-boost-from-two-drinks/) 1484
- [2222. Number of Ways to Select Buildings](https://leetcode.com/problems/number-of-ways-to-select-buildings/) 1657
- [2708. Maximum Strength of a Group](https://leetcode.com/problems/maximum-strength-of-a-group/) (achieve O(n) time (cf. 152))
- [1567. Maximum Length of Subarray With Positive Product](https://leetcode.com/problems/maximum-length-of-subarray-with-positive-product/) 1710
- [2786. Visit Array Positions to Maximize Score](https://leetcode.com/problems/visit-array-positions-to-maximize-score/) 1733
- [1911. Maximum Alternating Subsequence Sum](https://leetcode.com/problems/maximum-alternating-subsequence-sum/) 1786
- [376. Wiggle Subsequence](https://leetcode.com/problems/wiggle-subsequence/)
- [3466. Maximum Coin Collection](https://leetcode.com/problems/maximum-coin-collection/) 🔒

### §6.3 Advanced

- [3628. Maximum Number of Subsequences After One Inserting](https://leetcode.com/problems/maximum-number-of-subsequences-after-one-inserting/) 1754
- [2771. Longest Non-decreasing Subarray From Two Arrays](https://leetcode.com/problems/longest-non-decreasing-subarray-from-two-arrays/) 1792
- [1186. Maximum Subarray Sum with One Deletion](https://leetcode.com/problems/maximum-subarray-sum-with-one-deletion/) 1799
- [1594. Maximum Non Negative Product in a Matrix](https://leetcode.com/problems/maximum-non-negative-product-in-a-matrix/) 1807
- [3738. Longest Non Decreasing Subarray After Replacing At Most One Element](https://leetcode.com/problems/longest-non-decreasing-subarray-after-replacing-at-most-one-element/) 1811
- [3196. Maximize Total Cost of Alternating Subarrays](https://leetcode.com/problems/maximize-total-cost-of-alternating-subarrays/) 1847 (also has a partition DP approach)
- [935. Knight Dialer](https://leetcode.com/problems/knight-dialer/)
- [3891. Minimum Increase to Maximize Special Indices](https://leetcode.com/problems/minimum-increase-to-maximize-special-indices/) 1953
- [1537. Get The Maximum Score](https://leetcode.com/problems/get-the-maximum-score/) 1961
- [3811. Number of Alternating XOR Partitions](https://leetcode.com/problems/number-of-alternating-xor-partitions/) 2006 (more than one approach)
- [2919. Minimum Increment Operations to Make Array Beautiful](https://leetcode.com/problems/minimum-increment-operations-to-make-array-beautiful/) 2031
- [3872. Longest Arithmetic Sequence After Changing At Most One Element](https://leetcode.com/problems/longest-arithmetic-sequence-after-changing-at-most-one-element/) 2042
- [801. Minimum Swaps To Make Sequences Increasing](https://leetcode.com/problems/minimum-swaps-to-make-sequences-increasing/) 2066
- [3434. Maximum Frequency After Subarray Operation](https://leetcode.com/problems/maximum-frequency-after-subarray-operation/) 2094
- [1955. Count Number of Special Subsequences](https://leetcode.com/problems/count-number-of-special-subsequences/) 2125
- [3830. Longest Alternating Subarray After Removing At Most One Element](https://leetcode.com/problems/longest-alternating-subarray-after-removing-at-most-one-element/) 2162
- [3068. Find the Maximum Sum of Node Values](https://leetcode.com/problems/find-the-maximum-sum-of-node-values/) 2268
- [3640. Trionic Array II](https://leetcode.com/problems/trionic-array-ii/) 2278
- [2272. Substring With Largest Variance](https://leetcode.com/problems/substring-with-largest-variance/) 2516
- [3661. Maximum Walls Destroyed by Robots](https://leetcode.com/problems/maximum-walls-destroyed-by-robots/) 2525
- [3077. Maximum Strength of K Disjoint Subarrays](https://leetcode.com/problems/maximum-strength-of-k-disjoint-subarrays/) 2557 (more than one approach)
- [3743. Maximize Cyclic Partition Score](https://leetcode.com/problems/maximize-cyclic-partition-score/) 3125 (circular array)
- [LCP 19. Autumn Leaves Collection](https://leetcode.cn/problems/UlBDOe/)
- [276. Paint Fence](https://leetcode.com/problems/paint-fence/) 🔒
- [1746. Maximum Subarray Sum After One Operation](https://leetcode.com/problems/maximum-subarray-sum-after-one-operation/) 🔒
- [2036. Maximum Alternating Subarray Sum](https://leetcode.com/problems/maximum-alternating-subarray-sum/) 🔒
- [2361. Minimum Costs Using the Train Line](https://leetcode.com/problems/minimum-costs-using-the-train-line/) 🔒
- [3269. Constructing Two Increasing Arrays](https://leetcode.com/problems/constructing-two-increasing-arrays/) 🔒

## VII. Other Linear DP

### §7.1 One-Dimensional DP

Transitions between prefixes/suffixes, e.g. from f[i-1] to f[i], or from f[j] to f[i].

- [3147. Taking Maximum Energy From the Mystic Dungeon](https://leetcode.com/problems/taking-maximum-energy-from-the-mystic-dungeon/) 1460
- [2944. Minimum Number of Coins for Fruits](https://leetcode.com/problems/minimum-number-of-coins-for-fruits/) 1709
- [2140. Solving Questions With Brainpower](https://leetcode.com/problems/solving-questions-with-brainpower/) 1709 (can use push DP)
- [983. Minimum Cost For Tickets](https://leetcode.com/problems/minimum-cost-for-tickets/) 1786 (has an O(n) approach)
- [368. Largest Divisible Subset](https://leetcode.com/problems/largest-divisible-subset/) ~1800
- [2901. Longest Unequal Adjacent Groups Subsequence II](https://leetcode.com/problems/longest-unequal-adjacent-groups-subsequence-ii/) 1899
- [650. 2 Keys Keyboard](https://leetcode.com/problems/2-keys-keyboard/) ~2000
- [871. Minimum Number of Refueling Stops](https://leetcode.com/problems/minimum-number-of-refueling-stops/) 2074
- [32. Longest Valid Parentheses](https://leetcode.com/problems/longest-valid-parentheses/)
- [2167. Minimum Time to Remove All Cars Containing Illegal Goods](https://leetcode.com/problems/minimum-time-to-remove-all-cars-containing-illegal-goods/) 2219
- [2188. Minimum Time to Finish the Race](https://leetcode.com/problems/minimum-time-to-finish-the-race/) 2315
- [2896. Apply Operations to Make Two Strings Equal](https://leetcode.com/problems/apply-operations-to-make-two-strings-equal/) (achieve O(n))
- [818. Race Car](https://leetcode.com/problems/race-car/) 2392
- [3389. Minimum Operations to Make Character Frequencies Equal](https://leetcode.com/problems/minimum-operations-to-make-character-frequencies-equal/) 2940
- [3464. Maximize the Distance Between Points on a Square](https://leetcode.com/problems/maximize-the-distance-between-points-on-a-square/)
- [3205. Maximum Array Hopping Score I](https://leetcode.com/problems/maximum-array-hopping-score-i/) 🔒 (has an O(n) approach)
- [1259. Handshakes That Don't Cross](https://leetcode.com/problems/handshakes-that-dont-cross/) 🔒
- [2597. The Number of Beautiful Subsets](https://leetcode.com/problems/the-number-of-beautiful-subsets/) (solve with DP)
- [2638. Count the Number of K-Free Subsets](https://leetcode.com/problems/count-the-number-of-k-free-subsets/) 🔒 (harder version of the problem above)

### §7.2 Non-overlapping Intervals

- [2830. Maximize the Profit as the Salesman](https://leetcode.com/problems/maximize-the-profit-as-the-salesman/) 1851
- [2008. Maximum Earnings From Taxi](https://leetcode.com/problems/maximum-earnings-from-taxi/) 1872
- [2054. Two Best Non-Overlapping Events](https://leetcode.com/problems/two-best-non-overlapping-events/) 1883
- [1235. Maximum Profit in Job Scheduling](https://leetcode.com/problems/maximum-profit-in-job-scheduling/) 2023 (more than one approach)
- [1751. Maximum Number of Events That Can Be Attended II](https://leetcode.com/problems/maximum-number-of-events-that-can-be-attended-ii/) 2041
- [3414. Maximum Score of Non-overlapping Intervals](https://leetcode.com/problems/maximum-score-of-non-overlapping-intervals/) 2723

### §7.3 Subarray DP

- [53. Maximum Subarray](https://leetcode.com/problems/maximum-subarray/)
- [152. Maximum Product Subarray](https://leetcode.com/problems/maximum-product-subarray/)
- [1186. Maximum Subarray Sum with One Deletion](https://leetcode.com/problems/maximum-subarray-sum-with-one-deletion/) 1799
- [3738. Longest Non Decreasing Subarray After Replacing At Most One Element](https://leetcode.com/problems/longest-non-decreasing-subarray-after-replacing-at-most-one-element/) 1811
- [3524. Find X Value of Array I](https://leetcode.com/problems/find-x-value-of-array-i/) 2008 (push DP)
- [3872. Longest Arithmetic Sequence After Changing At Most One Element](https://leetcode.com/problems/longest-arithmetic-sequence-after-changing-at-most-one-element/) 2042
- [3830. Longest Alternating Subarray After Removing At Most One Element](https://leetcode.com/problems/longest-alternating-subarray-after-removing-at-most-one-element/) 2162
- [3448. Count Substrings Divisible By Last Digit](https://leetcode.com/problems/count-substrings-divisible-by-last-digit/) 2387 (push DP)

**Mind Extensions**:

- [2262. Total Appeal of A String](https://leetcode.com/problems/total-appeal-of-a-string/) 2033
- [828. Count Unique Characters of All Substrings of a Given String](https://leetcode.com/problems/count-unique-characters-of-all-substrings-of-a-given-string/) 2034
- [467. Unique Substrings In Wraparound String](https://leetcode.com/problems/unique-substrings-in-wraparound-string/)

### §7.4 Valid Subsequence DP

Compute the longest length, count, element sum, etc. of valid subsequences.

Generally define f[x] as the longest length / count / element sum of valid subsequences ending with element x, transitioning from the second-to-last number of the subsequence.

Note that x here is not an index but an element value. If x is not an integer, or the value range is large, use a hash map instead of an array.

- [2501. Longest Square Streak in an Array](https://leetcode.com/problems/longest-square-streak-in-an-array/) 1480
- [1218. Longest Arithmetic Subsequence of Given Difference](https://leetcode.com/problems/longest-arithmetic-subsequence-of-given-difference/) 1597
- [2826. Sorting Three Groups](https://leetcode.com/problems/sorting-three-groups/) 1721 (more than one approach)
- [1027. Longest Arithmetic Subsequence](https://leetcode.com/problems/longest-arithmetic-subsequence/) 1759
- [2370. Longest Ideal Subsequence](https://leetcode.com/problems/longest-ideal-subsequence/) 1835
- [873. Length of Longest Fibonacci Subsequence](https://leetcode.com/problems/length-of-longest-fibonacci-subsequence/) 1911
- [3686. Number of Stable Subsequences](https://leetcode.com/problems/number-of-stable-subsequences/) 1969
- [3202. Find the Maximum Length of Valid Subsequence II](https://leetcode.com/problems/find-the-maximum-length-of-valid-subsequence-ii/) 1974
- [446. Arithmetic Slices II - Subsequence](https://leetcode.com/problems/arithmetic-slices-ii-subsequence/) (count)
- [3811. Number of Alternating XOR Partitions](https://leetcode.com/problems/number-of-alternating-xor-partitions/) 2006 (more than one approach)
- [3351. Sum of Good Subsequences](https://leetcode.com/problems/sum-of-good-subsequences/) 2086 (sum)
- [3041. Maximize Consecutive Elements in an Array After Modification](https://leetcode.com/problems/maximize-consecutive-elements-in-an-array-after-modification/) 2231
- [3409. Longest Subsequence With Decreasing Adjacent Difference](https://leetcode.com/problems/longest-subsequence-with-decreasing-adjacent-difference/) 2500 (state design)
- [3098. Find the Sum of Subsequence Powers](https://leetcode.com/problems/find-the-sum-of-subsequence-powers/) 2553
- [2901. Longest Unequal Adjacent Groups Subsequence II](https://leetcode.com/problems/longest-unequal-adjacent-groups-subsequence-ii/) (achieve linear time)
- [3299. Sum of Consecutive Subsequences](https://leetcode.com/problems/sum-of-consecutive-subsequences/) 🔒

**Mind Extensions**:

- [1048. Longest String Chain](https://leetcode.com/problems/longest-string-chain/) 1599
- [940. Distinct Subsequences II](https://leetcode.com/problems/distinct-subsequences-ii/) 1985
- [1987. Number of Unique Good Subsequences](https://leetcode.com/problems/number-of-unique-good-subsequences/) 2422 (same idea as 940)
- [730. Count Different Palindromic Subsequences](https://leetcode.com/problems/count-different-palindromic-subsequences/)

### §7.5 Submatrix DP

- [3148. Maximum Difference Score in a Grid](https://leetcode.com/problems/maximum-difference-score-in-a-grid/) 1820
- [221. Maximal Square](https://leetcode.com/problems/maximal-square/)
- [1277. Count Square Submatrices With All Ones](https://leetcode.com/problems/count-square-submatrices-with-all-ones/)
- [2088. Count Fertile Pyramids in a Land](https://leetcode.com/problems/count-fertile-pyramids-in-a-land/) 2105
- [3197. Find the Minimum Area to Cover All Ones II](https://leetcode.com/problems/find-the-minimum-area-to-cover-all-ones-ii/) (achieve O(mn))

### §7.6 Multi-dimensional DP

Don't know how to design the state? Then practice this section well.

- [2222. Number of Ways to Select Buildings](https://leetcode.com/problems/number-of-ways-to-select-buildings/) 1657 (how to generalize 3 to k?)
- [2826. Sorting Three Groups](https://leetcode.com/problems/sorting-three-groups/) 1721 (more than one approach)
- [2400. Number of Ways to Reach a Position After Exactly k Steps](https://leetcode.com/problems/number-of-ways-to-reach-a-position-after-exactly-k-steps/) 1751
- [1262. Greatest Sum Divisible by Three](https://leetcode.com/problems/greatest-sum-divisible-by-three/) 1762
- [3780. Maximum Sum of Three Numbers Divisible by Three](https://leetcode.com/problems/maximum-sum-of-three-numbers-divisible-by-three/) (general approach)
- [3332. Maximum Points Tourist Can Earn](https://leetcode.com/problems/maximum-points-tourist-can-earn/) 1828
- [3176. Find the Maximum Length of a Good Subsequence I](https://leetcode.com/problems/find-the-maximum-length-of-a-good-subsequence-i/) 1849
- [1269. Number of Ways to Stay in the Same Place After Some Steps](https://leetcode.com/problems/number-of-ways-to-stay-in-the-same-place-after-some-steps/) 1854
- [3250. Find the Count of Monotonic Pairs I](https://leetcode.com/problems/find-the-count-of-monotonic-pairs-i/) 1898
- [3218. Minimum Cost for Cutting Cake I](https://leetcode.com/problems/minimum-cost-for-cutting-cake-i/) (also has a greedy approach)
- [3122. Minimum Number of Operations to Satisfy Conditions](https://leetcode.com/problems/minimum-number-of-operations-to-satisfy-conditions/) 1905
- [576. Out of Boundary Paths](https://leetcode.com/problems/out-of-boundary-paths/)
- [403. Frog Jump](https://leetcode.com/problems/frog-jump/)
- [3850. Count Sequences to K](https://leetcode.com/problems/count-sequences-to-k/) 1965
- [3725. Count Ways to Choose Coprime Integers from Rows](https://leetcode.com/problems/count-ways-to-choose-coprime-integers-from-rows/) 1982
- [1223. Dice Roll Simulation](https://leetcode.com/problems/dice-roll-simulation/) 2008
- [1320. Minimum Distance to Type a Word Using Two Fingers](https://leetcode.com/problems/minimum-distance-to-type-a-word-using-two-fingers/) 2028 (state optimization)
- [3366. Minimum Array Sum](https://leetcode.com/problems/minimum-array-sum/) 2040
- [1575. Count All Possible Routes](https://leetcode.com/problems/count-all-possible-routes/) 2055
- [3154. Find Number of Ways to Reach the K-th Stair](https://leetcode.com/problems/find-number-of-ways-to-reach-the-k-th-stair/) 2071
- [2318. Number of Distinct Roll Sequences](https://leetcode.com/problems/number-of-distinct-roll-sequences/) 2090
- [3469. Find Minimum Cost to Remove Array Elements](https://leetcode.com/problems/find-minimum-cost-to-remove-array-elements/) 2112 (state design)
- [2746. Decremental String Concatenation](https://leetcode.com/problems/decremental-string-concatenation/) 2126
- [1444. Number of Ways of Cutting a Pizza](https://leetcode.com/problems/number-of-ways-of-cutting-a-pizza/) 2127
- [3320. Count The Number of Winning Sequences](https://leetcode.com/problems/count-the-number-of-winning-sequences/) 2153
- [3429. Paint House IV](https://leetcode.com/problems/paint-house-iv/) 2166
- [2896. Apply Operations to Make Two Strings Equal](https://leetcode.com/problems/apply-operations-to-make-two-strings-equal/) 2172
- [1420. Build Array Where You Can Find The Maximum Exactly K Comparisons](https://leetcode.com/problems/build-array-where-you-can-find-the-maximum-exactly-k-comparisons/) 2176
- [3193. Count the Number of Inversions](https://leetcode.com/problems/count-the-number-of-inversions/) 2266
- [3892. Minimum Operations to Achieve At Least K Peaks](https://leetcode.com/problems/minimum-operations-to-achieve-at-least-k-peaks/) 2280
- [2312. Selling Pieces of Wood](https://leetcode.com/problems/selling-pieces-of-wood/) 2363
- [3177. Find the Maximum Length of a Good Subsequence II](https://leetcode.com/problems/find-the-maximum-length-of-a-good-subsequence-ii/) 2365
- [1884. Egg Drop With 2 Eggs and N Floors](https://leetcode.com/problems/egg-drop-with-2-eggs-and-n-floors/)
- [887. Super Egg Drop](https://leetcode.com/problems/super-egg-drop/) 2377
- [920. Number of Music Playlists](https://leetcode.com/problems/number-of-music-playlists/) 2400
- [514. Freedom Trail](https://leetcode.com/problems/freedom-trail/) (achieve O(mn))
- [3336. Find the Number of Subsequences With Equal GCD](https://leetcode.com/problems/find-the-number-of-subsequences-with-equal-gcd/) 2403
- [1388. Pizza With 3n Slices](https://leetcode.com/problems/pizza-with-3n-slices/) 2410
- [903. Valid Permutations for DI Sequence](https://leetcode.com/problems/valid-permutations-for-di-sequence/) 2433
- [1900. The Earliest and Latest Rounds Where Players Compete](https://leetcode.com/problems/the-earliest-and-latest-rounds-where-players-compete/) 2455
- [1531. String Compression II](https://leetcode.com/problems/string-compression-ii/) 2576
- [1883. Minimum Skips to Arrive at Meeting On Time](https://leetcode.com/problems/minimum-skips-to-arrive-at-meeting-on-time/) 2588 (trick to avoid floating-point)
- [964. Least Operators to Express Number](https://leetcode.com/problems/least-operators-to-express-number/) 2594
- [1787. Make the XOR of All Segments Equal to Zero](https://leetcode.com/problems/make-the-xor-of-all-segments-equal-to-zero/) 2640
- [3509. Maximum Product of Subsequences With an Alternating Sum Equal to K](https://leetcode.com/problems/maximum-product-of-subsequences-with-an-alternating-sum-equal-to-k/) 2703
- [3441. Minimum Cost Good Caption](https://leetcode.com/problems/minimum-cost-good-caption/) 2765
- [2060. Check if an Original String Exists Given Two Encoded Strings](https://leetcode.com/problems/check-if-an-original-string-exists-given-two-encoded-strings/) 2804
- [2809. Minimum Time to Make Array Sum At Most x](https://leetcode.com/problems/minimum-time-to-make-array-sum-at-most-x/) 2979
- [3003. Maximize the Number of Partitions After Operations](https://leetcode.com/problems/maximize-the-number-of-partitions-after-operations/) 3039 (how to analyze the time complexity)
- [3225. Maximum Score From Grid Operations](https://leetcode.com/problems/maximum-score-from-grid-operations/) 3028 (original IOI2022 problem)
- [LCP 57. Whack-a-Mole](https://leetcode.cn/problems/ZbAuEH/)
- [LCP 43. Traffic at the Intersection](https://leetcode.cn/problems/Y1VbOX/)
- [LCP 65. Comfortable Humidity](https://leetcode.cn/problems/3aqs1c/)
- [LCP 36. Most Groups of Tiles](https://leetcode.cn/problems/Up5XYM/)
- [LCP 38. Guard the Castle](https://leetcode.cn/problems/7rLGCR/)
- [256. Paint House](https://leetcode.com/problems/paint-house/) 🔒
- [265. Paint House II](https://leetcode.com/problems/paint-house-ii/) 🔒
- [3339. Find the Number of K-Even Arrays](https://leetcode.com/problems/find-the-number-of-k-even-arrays/) 🔒
- [568. Maximum Vacation Days](https://leetcode.com/problems/maximum-vacation-days/) 🔒
- [1692. Count Ways to Distribute Candies](https://leetcode.com/problems/count-ways-to-distribute-candies/) 🔒
- [2143. Choose Numbers From Two Arrays in Range](https://leetcode.com/problems/choose-numbers-from-two-arrays-in-range/) 🔒
- [3269. Constructing Two Increasing Arrays](https://leetcode.com/problems/constructing-two-increasing-arrays/) 🔒

**Mind Extensions**:

- [638. Shopping Offers](https://leetcode.com/problems/shopping-offers/)

### §7.7 Counting DP

- [1079. Letter Tile Possibilities](https://leetcode.com/problems/letter-tile-possibilities/) (achieve O(n^2))
- [1866. Number of Ways to Rearrange Sticks With K Sticks Visible](https://leetcode.com/problems/number-of-ways-to-rearrange-sticks-with-k-sticks-visible/) 2333
- [3317. Find the Number of Possible Ways for an Event](https://leetcode.com/problems/find-the-number-of-possible-ways-for-an-event/) 2414
- [3343. Count Number of Balanced Permutations](https://leetcode.com/problems/count-number-of-balanced-permutations/) 2615
- [3539. Find Sum of Array Product of Magical Sequences](https://leetcode.com/problems/find-sum-of-array-product-of-magical-sequences/) 2694

## VIII. Interval DP

Repeatedly shrink from both ends of the array to solve for the optimum over an index interval.

Generally define f[i][j] as the optimum over index interval [i, j].

### §8.1 Longest Palindromic Subsequence

- [516. Longest Palindromic Subsequence](https://leetcode.com/problems/longest-palindromic-subsequence/)
- [1312. Minimum Insertion Steps to Make a String Palindrome](https://leetcode.com/problems/minimum-insertion-steps-to-make-a-string-palindrome/) 1787
- [3472. Longest Palindromic Subsequence After at Most K Operations](https://leetcode.com/problems/longest-palindromic-subsequence-after-at-most-k-operations/) 1884
- [1771. Maximize Palindrome Length From Subsequences](https://leetcode.com/problems/maximize-palindrome-length-from-subsequences/) 2182
- [730. Count Different Palindromic Subsequences](https://leetcode.com/problems/count-different-palindromic-subsequences/)
- [1682. Longest Palindromic Subsequence II](https://leetcode.com/problems/longest-palindromic-subsequence-ii/) 🔒
- [1216. Valid Palindrome III](https://leetcode.com/problems/valid-palindrome-iii/) 🔒
- [1246. Palindrome Removal](https://leetcode.com/problems/palindrome-removal/) 🔒

### §8.2 Interval DP

For elimination problems similar to regular balanced strings (RBS), the following properties usually hold:

- Adjacent matching characters can be eliminated.

- After eliminating adjacent matches, previously non-adjacent characters become adjacent and can be eliminated. That is, for A = x + B + y, if x and y match and B can be fully eliminated, then A can be fully eliminated.

- For A = B + C, if B and C can each be fully eliminated, then A can be fully eliminated.

Problems with the above properties (e.g. problem 3563) can be solved with interval DP.

Define f(i, j) as the optimum for eliminating s[i..j].

Base case: f(i+1, i), i.e. the empty string.

Answer: f(0, n-1).

- [5. Longest Palindromic Substring](https://leetcode.com/problems/longest-palindromic-substring/)
- [647. Palindromic Substrings](https://leetcode.com/problems/palindromic-substrings/)
- [3040. Maximum Number of Operations With the Same Score II](https://leetcode.com/problems/maximum-number-of-operations-with-the-same-score-ii/) 1709
- [1130. Minimum Cost Tree From Leaf Values](https://leetcode.com/problems/minimum-cost-tree-from-leaf-values/) 1919
- [96. Unique Binary Search Trees](https://leetcode.com/problems/unique-binary-search-trees/)
- [375. Guess Number Higher or Lower II](https://leetcode.com/problems/guess-number-higher-or-lower-ii/)
- [1770. Maximum Score from Performing Multiplication Operations](https://leetcode.com/problems/maximum-score-from-performing-multiplication-operations/) 2068
- [1547. Minimum Cost to Cut a Stick](https://leetcode.com/problems/minimum-cost-to-cut-a-stick/) 2116
- [1039. Minimum Score Triangulation of Polygon](https://leetcode.com/problems/minimum-score-triangulation-of-polygon/) 2130
- [1000. Minimum Cost to Merge Stones](https://leetcode.com/problems/minimum-cost-to-merge-stones/) 2423
- [2019. The Score of Students Solving Math Expression](https://leetcode.com/problems/the-score-of-students-solving-math-expression/) 2584
- [Interview 08.14. Boolean Evaluation](https://leetcode.cn/problems/boolean-evaluation-lcci/)
- [3563. Lexicographically Smallest String After Adjacent Removals](https://leetcode.com/problems/lexicographically-smallest-string-after-adjacent-removals/) 2585
- [3277. Maximum XOR Score Subarray Queries](https://leetcode.com/problems/maximum-xor-score-subarray-queries/) 2693
- [87. Scramble String](https://leetcode.com/problems/scramble-string/)
- [312. Burst Balloons](https://leetcode.com/problems/burst-balloons/)
- [664. Strange Printer](https://leetcode.com/problems/strange-printer/)
- [546. Remove Boxes](https://leetcode.com/problems/remove-boxes/) (same as CF1107E)
- [471. Encode String with Shortest Length](https://leetcode.com/problems/encode-string-with-shortest-length/) 🔒
- [3018. Maximum Number of Removal Queries That Can Be Processed I](https://leetcode.com/problems/maximum-number-of-removal-queries-that-can-be-processed-i/) 🔒

## IX. Bitmask DP (State Compression DP)

### §9.1 Permutation Bitmask DP ① Adjacency-Independent

Brute force enumerates all permutations and computes a problem-related value for each, with time complexity (typically) O(n!), solving n <= 10.

Bitmask DP reduces the time complexity (typically) to O(n * 2^n), solving n <= 20.

There are generally two ways to define the state:

- Define f[S] as the optimum when the set of already-arranged elements (indices) is S, transitioning by enumerating which element to place at the current position.

- Define f[S] as the optimum when the set of selectable elements (indices) is S, transitioning by enumerating which element to place at the current position.

> Note: some problems also pass with brute force + pruning, so the difficulty ratings are for reference only.

- [526. Beautiful Arrangement](https://leetcode.com/problems/beautiful-arrangement/)
- [3376. Minimum Time to Break Locks I](https://leetcode.com/problems/minimum-time-to-break-locks-i/)
- [1879. Minimum XOR Sum of Two Arrays](https://leetcode.com/problems/minimum-xor-sum-of-two-arrays/) 2145
- [2850. Minimum Moves to Spread Stones Over Grid](https://leetcode.com/problems/minimum-moves-to-spread-stones-over-grid/)
- [1947. Maximum Compatibility Score Sum](https://leetcode.com/problems/maximum-compatibility-score-sum/)
- [1799. Maximize Score After N Operations](https://leetcode.com/problems/maximize-score-after-n-operations/)
- [3533. Concatenated Divisibility](https://leetcode.com/problems/concatenated-divisibility/) 2257 (lexicographic; brute force)
- [3530. Maximum Profit from Valid Topological Order in DAG](https://leetcode.com/problems/maximum-profit-from-valid-topological-order-in-dag/) 2353 (topological order)
- [2172. Maximum AND Sum of Array](https://leetcode.com/problems/maximum-and-sum-of-array/) 2392
- [2992. Number of Self-Divisible Permutations](https://leetcode.com/problems/number-of-self-divisible-permutations/) 🔒
- [2403. Minimum Time to Kill All Monsters](https://leetcode.com/problems/minimum-time-to-kill-all-monsters/) 🔒 (same as 3376)
- [1066. Campus Bikes II](https://leetcode.com/problems/campus-bikes-ii/) 🔒

### §9.2 Permutation Bitmask DP ② Adjacency-Dependent

Generally define f[S][i] as the optimum when the unchosen (or chosen) set is S and the last placed element (index) is i, transitioning by enumerating the element to place at the current position.

Time complexity (typically) O(n^2 * 2^n).

- [2741. Special Permutations](https://leetcode.com/problems/special-permutations/) 2021
- [996. Number of Squareful Arrays](https://leetcode.com/problems/number-of-squareful-arrays/)
- [1681. Minimum Incompatibility](https://leetcode.com/problems/minimum-incompatibility/) 2390 (see my comment under the official solution)
- [3615. Longest Palindromic Path in Graph](https://leetcode.com/problems/longest-palindromic-path-in-graph/) 2463
- [3283. Maximum Number of Moves to Kill All Pawns](https://leetcode.com/problems/maximum-number-of-moves-to-kill-all-pawns/) 2473
- [3149. Find the Minimum Cost Array Permutation](https://leetcode.com/problems/find-the-minimum-cost-array-permutation/) 2642

### §9.3 Traveling Salesman Problem (TSP)

Essentially the same as permutation type ②.

- [943. Find the Shortest Superstring](https://leetcode.com/problems/find-the-shortest-superstring/) 2186
- [847. Shortest Path Visiting All Nodes](https://leetcode.com/problems/shortest-path-visiting-all-nodes/) 2201
- [LCP 13. Treasure Hunt](https://leetcode.cn/problems/xun-bao/)
- [2247. Maximum Cost of Trip With K Highways](https://leetcode.com/problems/maximum-cost-of-trip-with-k-highways/) 🔒

**Similar problems**:

- [3568. Minimum Moves to Clean the Classroom](https://leetcode.com/problems/minimum-moves-to-clean-the-classroom/) 2143
- [864. Shortest Path to Get All Keys](https://leetcode.com/problems/shortest-path-to-get-all-keys/) 2259

### §9.4 Subset Bitmask DP

Generally define f[S] as the optimum when the unchosen (or chosen) set is S, transitioning by enumerating subsets of S (or of its complement).

Time complexity (typically) O(3^n).

> Note: some grid problems can also use "take or skip" to reduce the number of states; see §9.5 Broken Profile DP.

- [2305. Fair Distribution of Cookies](https://leetcode.com/problems/fair-distribution-of-cookies/) 1887
- [1986. Minimum Number of Work Sessions to Finish the Tasks](https://leetcode.com/problems/minimum-number-of-work-sessions-to-finish-the-tasks/) 1995
- [3670. Maximum Product of Two Integers With No Common Bits](https://leetcode.com/problems/maximum-product-of-two-integers-with-no-common-bits/) 2234
- [1723. Find Minimum Time to Finish All Jobs](https://leetcode.com/problems/find-minimum-time-to-finish-all-jobs/) 2284
- [1655. Distribute Repeating Integers](https://leetcode.com/problems/distribute-repeating-integers/) 2307
- [3444. Minimum Increments for Target Multiples in an Array](https://leetcode.com/problems/minimum-increments-for-target-multiples-in-an-array/) 2337
- [3575. Maximum Good Subtree Score](https://leetcode.com/problems/maximum-good-subtree-score/) 2360
- [1349. Maximum Students Taking Exam](https://leetcode.com/problems/maximum-students-taking-exam/) 2386
- [1681. Minimum Incompatibility](https://leetcode.com/problems/minimum-incompatibility/) 2390 (has an O(n^2 * 2^n) approach)
- [3801. Minimum Cost to Merge Sorted Lists](https://leetcode.com/problems/minimum-cost-to-merge-sorted-lists/) 2399
- [2572. Count the Number of Square-Free Subsets](https://leetcode.com/problems/count-the-number-of-square-free-subsets/) 2420
- [1994. The Number of Good Subsets](https://leetcode.com/problems/the-number-of-good-subsets/) 2465
- [1494. Parallel Courses II](https://leetcode.com/problems/parallel-courses-ii/)
- [LCP 04. Broken Board Dominoes](https://leetcode.cn/problems/broken-board-dominoes/)
- [LCP 53. Guard the Space City](https://leetcode.cn/problems/EJvmW4/)
- [465. Optimal Account Balancing](https://leetcode.com/problems/optimal-account-balancing/) 🔒
- [2152. Minimum Number of Lines to Cover Points](https://leetcode.com/problems/minimum-number-of-lines-to-cover-points/) 🔒

**Related problems**:

- [3594. Minimum Time to Transport All Individuals](https://leetcode.com/problems/minimum-time-to-transport-all-individuals/) 2604

### §9.5 Broken Profile DP

- [1411. Number of Ways to Paint N × 3 Grid](https://leetcode.com/problems/number-of-ways-to-paint-n-3-grid/) 1845
- [1931. Painting a Grid With Three Different Colors](https://leetcode.com/problems/painting-a-grid-with-three-different-colors/) 2170
- [1349. Maximum Students Taking Exam](https://leetcode.com/problems/maximum-students-taking-exam/) 2386
- [1659. Maximize Grid Happiness](https://leetcode.com/problems/maximize-grid-happiness/) 2655
- [980. Unique Paths III](https://leetcode.com/problems/unique-paths-iii/)
- [LCP 04. Broken Board Dominoes](https://leetcode.cn/problems/broken-board-dominoes/)
- [LCP 76. Magic Chessboard](https://leetcode.cn/problems/1ybDKD/)
- [2184. Number of Ways to Build Sturdy Brick Wall](https://leetcode.com/problems/number-of-ways-to-build-sturdy-brick-wall/) 🔒

**Mind Extensions**:

- [756. Pyramid Transition Matrix](https://leetcode.com/problems/pyramid-transition-matrix/) 1990

### §9.6 SOS DP

Sum Over Subsets DP (SOS DP), commonly called high-dimensional prefix sum in competitive programming.

- [3670. Maximum Product of Two Integers With No Common Bits](https://leetcode.com/problems/maximum-product-of-two-integers-with-no-common-bits/) 2234
- [2002. Maximum Product of the Length of Two Palindromic Subsequences](https://leetcode.com/problems/maximum-product-of-the-length-of-two-palindromic-subsequences/)
- [2044. Count Number of Maximum Bitwise-OR Subsets](https://leetcode.com/problems/count-number-of-maximum-bitwise-or-subsets/)
- [2732. Find a Good Subset of the Matrix](https://leetcode.com/problems/find-a-good-subset-of-the-matrix/)
- [3757. Number of Effective Subsequences](https://leetcode.com/problems/number-of-effective-subsequences/) 2519

### §9.7 Other Bitmask DP

- [473. Matchsticks to Square](https://leetcode.com/problems/matchsticks-to-square/)
- [698. Partition to K Equal Sum Subsets](https://leetcode.com/problems/partition-to-k-equal-sum-subsets/)
- [1125. Smallest Sufficient Team](https://leetcode.com/problems/smallest-sufficient-team/) 2251
- [1434. Number of Ways to Wear Different Hats to Each Other](https://leetcode.com/problems/number-of-ways-to-wear-different-hats-to-each-other/) 2273
- [464. Can I Win](https://leetcode.com/problems/can-i-win/)
- [691. Stickers to Spell Word](https://leetcode.com/problems/stickers-to-spell-word/)
- [3276. Select Cells in Grid with Maximum Score](https://leetcode.com/problems/select-cells-in-grid-with-maximum-score/) 2403 (a different viewpoint)
- [1595. Minimum Cost to Connect Two Groups of Points](https://leetcode.com/problems/minimum-cost-to-connect-two-groups-of-points/) 2538
- [1815. Maximum Number of Groups Getting Fresh Donuts](https://leetcode.com/problems/maximum-number-of-groups-getting-fresh-donuts/) 2559
- [LCP 69. Hello LeetCode!](https://leetcode.cn/problems/rMeRt2/)
- [LCP 82. Tree of All Souls](https://leetcode.cn/problems/cnHoX6/)
- [351. Android Unlock Patterns](https://leetcode.com/problems/android-unlock-patterns/) 🔒

## X. Digit DP

Used to solve how many numbers in [l, r] meet a requirement, or the sum of such numbers, etc.

### §10.1 Count Valid Numbers

- [3747. Count Distinct Integers After Removing Zeros](https://leetcode.com/problems/count-distinct-integers-after-removing-zeros/) 1848
- [2719. Count of Integers](https://leetcode.com/problems/count-of-integers/)
- [762. Prime Number of Set Bits in Binary Representation](https://leetcode.com/problems/prime-number-of-set-bits-in-binary-representation/) (non-brute-force approach)
- [1399. Count Largest Group](https://leetcode.com/problems/count-largest-group/) (non-brute-force approach)
- [1742. Maximum Number of Balls in a Box](https://leetcode.com/problems/maximum-number-of-balls-in-a-box/) (non-brute-force approach)
- [788. Rotated Digits](https://leetcode.com/problems/rotated-digits/) (non-brute-force approach)
- [902. Numbers At Most N Given Digit Set](https://leetcode.com/problems/numbers-at-most-n-given-digit-set/) 1990
- [600. Non-negative Integers without Consecutive Ones](https://leetcode.com/problems/non-negative-integers-without-consecutive-ones/)
- [2376. Count Special Integers](https://leetcode.com/problems/count-special-integers/) 2120
- [357. Count Numbers with Unique Digits](https://leetcode.com/problems/count-numbers-with-unique-digits/) (same as 2376)
- [3791. Number of Balanced Integers in a Range](https://leetcode.com/problems/number-of-balanced-integers-in-a-range/) 2132
- [3906. Count Good Integers on a Grid Path](https://leetcode.com/problems/count-good-integers-on-a-grid-path/) 2160
- [1012. Numbers With Repeated Digits](https://leetcode.com/problems/numbers-with-repeated-digits/) 2230
- [3519. Count Numbers with Non-Decreasing Digits](https://leetcode.com/problems/count-numbers-with-non-decreasing-digits/) 2246 (base conversion)
- [3869. Count Fancy Numbers in a Range](https://leetcode.com/problems/count-fancy-numbers-in-a-range/) 2255
- [2827. Number of Beautiful Integers in the Range](https://leetcode.com/problems/number-of-beautiful-integers-in-the-range/) 2324
- [2999. Count the Number of Powerful Integers](https://leetcode.com/problems/count-the-number-of-powerful-integers/) 2351
- [2801. Count Stepping Numbers in Range](https://leetcode.com/problems/count-stepping-numbers-in-range/) 2367
- [2843. Count Symmetric Integers](https://leetcode.com/problems/count-symmetric-integers/) (non-brute-force approach)
- [3352. Count K-Reducible Numbers Less Than N](https://leetcode.com/problems/count-k-reducible-numbers-less-than-n/) 2451
- [3621. Number of Integers With Popcount-Depth Equal to K I](https://leetcode.com/problems/number-of-integers-with-popcount-depth-equal-to-k-i/) (same as 3352)
- [3490. Count Beautiful Numbers](https://leetcode.com/problems/count-beautiful-numbers/) 2502
- [1397. Find All Good Strings](https://leetcode.com/problems/find-all-good-strings/) 2667
- [1215. Stepping Numbers](https://leetcode.com/problems/stepping-numbers/) 🔒
- [3032. Count Numbers With Unique Digits II](https://leetcode.com/problems/count-numbers-with-unique-digits-ii/) 🔒
- [3704. Count No-Zero Pairs That Sum to N](https://leetcode.com/problems/count-no-zero-pairs-that-sum-to-n/) 2419 (pairs)

### §10.2 Sum of Values of Valid Numbers

Each element x has an associated value f(x); compute the total value of elements in [low, high] satisfying the constraints.

For example, f(x)=x gives the sum of qualifying elements, and f(x)=digsum(x) gives their digit-sum.

- [3871. Count Commas in Range II](https://leetcode.com/problems/count-commas-in-range-ii/) (more than one approach)
- [233. Number of Digit One](https://leetcode.com/problems/number-of-digit-one/)
- [Interview 17.06. Number of 2s in Range](https://leetcode.cn/problems/number-of-2s-in-range-lcci/)
- [3007. Maximum Number That Sum of the Prices Is Less Than or Equal to K](https://leetcode.com/problems/maximum-number-that-sum-of-the-prices-is-less-than-or-equal-to-k/) 2258
- [3753. Total Waviness of Numbers in Range II](https://leetcode.com/problems/total-waviness-of-numbers-in-range-ii/) 2297
- [1067. Digit Count in Range](https://leetcode.com/problems/digit-count-in-range/) 🔒

### §10.3 Other Digit DP

- [3677. Count Binary Palindromic Numbers](https://leetcode.com/problems/count-binary-palindromic-numbers/) 2223
- [3348. Smallest Divisible Digit Product II](https://leetcode.com/problems/smallest-divisible-digit-product-ii/) 3101 (lower bound only)

## XI. DP Optimization

### §11.1 Prefix-Sum-Optimized DP

- [1871. Jump Game VII](https://leetcode.com/problems/jump-game-vii/) 1896 (more than one approach)
- [2327. Number of People Aware of a Secret](https://leetcode.com/problems/number-of-people-aware-of-a-secret/) (achieve O(n))
- [3699. Number of ZigZag Arrays I](https://leetcode.com/problems/number-of-zigzag-arrays-i/) 2123
- [3883. Count Non Decreasing Arrays With Given Digit Sums](https://leetcode.com/problems/count-non-decreasing-arrays-with-given-digit-sums/) 2172
- [1997. First Day Where You Have Been in All the Rooms](https://leetcode.com/problems/first-day-where-you-have-been-in-all-the-rooms/) 2260
- [629. K Inverse Pairs Array](https://leetcode.com/problems/k-inverse-pairs-array/)
- [3193. Count the Number of Inversions](https://leetcode.com/problems/count-the-number-of-inversions/) 2266
- [3473. Sum of K Subarrays With Length at Least M](https://leetcode.com/problems/sum-of-k-subarrays-with-length-at-least-m/) 2274 (partition type)
- [3251. Find the Count of Monotonic Pairs II](https://leetcode.com/problems/find-the-count-of-monotonic-pairs-ii/) 2323 (more than one approach)
- [2478. Number of Beautiful Partitions](https://leetcode.com/problems/number-of-beautiful-partitions/) 2344
- [837. New 21 Game](https://leetcode.com/problems/new-21-game/) 2350 (can also use sliding window)
- [3797. Count Routes to Climb a Rectangular Grid](https://leetcode.com/problems/count-routes-to-climb-a-rectangular-grid/) 2376
- [3077. Maximum Strength of K Disjoint Subarrays](https://leetcode.com/problems/maximum-strength-of-k-disjoint-subarrays/) 2557 (partition type)
- [3333. Find the Original Typed String II](https://leetcode.com/problems/find-the-original-typed-string-ii/) 2629 (more than one approach)
- [2902. Count of Sub-Multisets With Bounded Sum](https://leetcode.com/problems/count-of-sub-multisets-with-bounded-sum/) 2759
- [1977. Number of Ways to Separate Numbers](https://leetcode.com/problems/number-of-ways-to-separate-numbers/) 2817
- [3130. Find All Possible Stable Binary Arrays II](https://leetcode.com/problems/find-all-possible-stable-binary-arrays-ii/) 2825 (more than one approach)

### §11.2 Monotonic-Stack-Optimized DP

Prerequisite: see the [Monotonic Stack list](03_monotonic_stack.md).

- [1335. Minimum Difficulty of a Job Schedule](https://leetcode.com/problems/minimum-difficulty-of-a-job-schedule/) 2035
- [2866. Beautiful Towers II](https://leetcode.com/problems/beautiful-towers-ii/) 2072
- [2617. Minimum Number of Visited Cells in a Grid](https://leetcode.com/problems/minimum-number-of-visited-cells-in-a-grid/) 2582
- [2355. Maximum Number Of Books You Can Take](https://leetcode.com/problems/maximum-number-of-books-you-can-take/) 🔒

### §11.3 Monotonic-Queue-Optimized DP

Generally used to maintain the extremum over a range of transition sources.

- Precondition: as the interval's right endpoint grows, the left endpoint also grows (like a sliding window).

- Before transitioning, remove useless data from the front of the queue.

- Compute the transition (directly from the front of the queue).

- Before inserting data (usually f[i]) at the back of the queue, remove useless data from the back.

- [2944. Minimum Number of Coins for Fruits](https://leetcode.com/problems/minimum-number-of-coins-for-fruits/) 1709 (achieve O(n))
- [1696. Jump Game VI](https://leetcode.com/problems/jump-game-vi/) 1954
- [1425. Constrained Subsequence Sum](https://leetcode.com/problems/constrained-subsequence-sum/) 2032
- [3578. Count Partitions With Max-Min Difference at Most K](https://leetcode.com/problems/count-partitions-with-max-min-difference-at-most-k/) 2033
- [375. Guess Number Higher or Lower II](https://leetcode.com/problems/guess-number-higher-or-lower-ii/) (achieve O(n^2))
- [1687. Delivering Boxes from Storage to Ports](https://leetcode.com/problems/delivering-boxes-from-storage-to-ports/) 2610
- [2463. Minimum Total Distance Traveled](https://leetcode.com/problems/minimum-total-distance-traveled/) (achieve O(mn))
- [3117. Minimum Sum of Values by Dividing Array](https://leetcode.com/problems/minimum-sum-of-values-by-dividing-array/) 2735
- [2945. Find Maximum Non-decreasing Array Length](https://leetcode.com/problems/find-maximum-non-decreasing-array-length/) 2943
- [2969. Minimum Number of Coins for Fruits II](https://leetcode.com/problems/minimum-number-of-coins-for-fruits-ii/) 🔒

### §11.4 BIT / Segment-Tree-Optimized DP

- [1626. Best Team With No Conflicts](https://leetcode.com/problems/best-team-with-no-conflicts/) 2027
- [2407. Longest Increasing Subsequence II](https://leetcode.com/problems/longest-increasing-subsequence-ii/) 2280
- [3915. Maximum Sum of Alternating Subsequence With Distance at Least K](https://leetcode.com/problems/maximum-sum-of-alternating-subsequence-with-distance-at-least-k/) 2288
- [2770. Maximum Number of Jumps to Reach the Last Index](https://leetcode.com/problems/maximum-number-of-jumps-to-reach-the-last-index/) (achieve O(n log n))
- [2926. Maximum Balanced Subsequence Sum](https://leetcode.com/problems/maximum-balanced-subsequence-sum/) 2448 (max-sum LIS)
- [2547. Minimum Cost to Split an Array](https://leetcode.com/problems/minimum-cost-to-split-an-array/) (achieve O(n log n))
- [3671. Sum of Beautiful Subsequences](https://leetcode.com/problems/sum-of-beautiful-subsequences/) 2647
- [2916. Subarrays Distinct Element Sum of Squares II](https://leetcode.com/problems/subarrays-distinct-element-sum-of-squares-ii/) 2816 (idea similar to 2547)

### §11.5 Trie-Optimized DP

- [139. Word Break](https://leetcode.com/problems/word-break/)
- [2707. Extra Characters in a String](https://leetcode.com/problems/extra-characters-in-a-string/)
- [Interview 17.13. Re-Space](https://leetcode.cn/problems/re-space-lcci/)
- [472. Concatenated Words](https://leetcode.com/problems/concatenated-words/) ~2300
- [2977. Minimum Cost to Convert String II](https://leetcode.com/problems/minimum-cost-to-convert-string-ii/) 2696

### §11.6 Matrix-Exponentiation-Optimized DP

There are two types of matrix-exponentiation-optimized DP:

- Linear DP (constant-coefficient homogeneous linear recurrence): transition coefficients go in the first row, other rows have m[i+1][i]=1, e.g. 70, 1137.

- Multi-dimensional or state-machine DP: transition coefficients form a k×k matrix, e.g. 935.

Time complexity is generally O(k^3 log n).

- [70. Climbing Stairs](https://leetcode.com/problems/climbing-stairs/)
- [509. Fibonacci Number](https://leetcode.com/problems/fibonacci-number/)
- [1137. N-th Tribonacci Number](https://leetcode.com/problems/n-th-tribonacci-number/)
- [1220. Count Vowels Permutation](https://leetcode.com/problems/count-vowels-permutation/)
- [552. Student Attendance Record II](https://leetcode.com/problems/student-attendance-record-ii/)
- [935. Knight Dialer](https://leetcode.com/problems/knight-dialer/)
- [790. Domino and Tromino Tiling](https://leetcode.com/problems/domino-and-tromino-tiling/)
- [1411. Number of Ways to Paint N × 3 Grid](https://leetcode.com/problems/number-of-ways-to-paint-n-3-grid/)
- [1931. Painting a Grid With Three Different Colors](https://leetcode.com/problems/painting-a-grid-with-three-different-colors/)
- [3337. Total Characters in String After Transformations II](https://leetcode.com/problems/total-characters-in-string-after-transformations-ii/) 2412
- [3700. Number of ZigZag Arrays II](https://leetcode.com/problems/number-of-zigzag-arrays-ii/) 2435
- [2851. String Transformation](https://leetcode.com/problems/string-transformation/) 2858
- [2912. Number of Ways to Reach Destination in the Grid](https://leetcode.com/problems/number-of-ways-to-reach-destination-in-the-grid/) 🔒

### §11.7 Slope Optimization (Convex Hull Trick)

Also called convex hull optimization (CHT, Convex Hull Trick).

- [3826. Minimum Partition Score](https://leetcode.com/problems/minimum-partition-score/) 2345
- [3494. Find the Minimum Amount of Time to Brew Potions](https://leetcode.com/problems/find-the-minimum-amount-of-time-to-brew-potions/)
- [3500. Minimum Cost to Divide Array Into Subarrays](https://leetcode.com/problems/minimum-cost-to-divide-array-into-subarrays/)
- [3693. Climbing Stairs II](https://leetcode.com/problems/climbing-stairs-ii/) (approach independent of K=3)

### §11.8 WQS Binary Search Optimization

Convert a problem of choosing at most k items (high complexity) into one of choosing any number of items (low complexity).

Time complexity is generally O(n log U) or O(n log n).

- [188. Best Time to Buy and Sell Stock IV](https://leetcode.com/problems/best-time-to-buy-and-sell-stock-iv/)
- [3573. Best Time to Buy and Sell Stock V](https://leetcode.com/problems/best-time-to-buy-and-sell-stock-v/)
- [2209. Minimum White Tiles After Covering With Carpets](https://leetcode.com/problems/minimum-white-tiles-after-covering-with-carpets/)
- [3826. Minimum Partition Score](https://leetcode.com/problems/minimum-partition-score/)
- [3743. Maximize Cyclic Partition Score](https://leetcode.com/problems/maximize-cyclic-partition-score/)
- [3929. Minimum Partition Score II](https://leetcode.com/problems/minimum-partition-score-ii/) 🔒 (same as 3826)

In addition, some problems in §5.3 can also use WQS binary search optimization.

### §11.9 Other Optimized DP

- [3654. Minimum Sum After Divisible Sum Deletions](https://leetcode.com/problems/minimum-sum-after-divisible-sum-deletions/) 2039
- [1937. Maximum Number of Points with Cost](https://leetcode.com/problems/maximum-number-of-points-with-cost/) 2106
- [2713. Maximum Strictly Increasing Cells in a Matrix](https://leetcode.com/problems/maximum-strictly-increasing-cells-in-a-matrix/) 2387
- [3651. Minimum Cost Path with Teleportations](https://leetcode.com/problems/minimum-cost-path-with-teleportations/) 2411
- [2318. Number of Distinct Roll Sequences](https://leetcode.com/problems/number-of-distinct-roll-sequences/) (inclusion-exclusion optimization (similar to CF1943D2))
- [3181. Maximum Total Reward Using Operations II](https://leetcode.com/problems/maximum-total-reward-using-operations-ii/) 2688 (bitset optimization)
- [2267. Check if There Is a Valid Parentheses String Path](https://leetcode.com/problems/check-if-there-is-a-valid-parentheses-string-path/) (can be further optimized with bitset)
- [3213. Construct String with Minimum Cost](https://leetcode.com/problems/construct-string-with-minimum-cost/) (string hashing / suffix array / Aho-Corasick optimization)
- [3292. Minimum Number of Valid Strings to Form Target II](https://leetcode.com/problems/minimum-number-of-valid-strings-to-form-target-ii/) (string hashing / Aho-Corasick optimization)
- [3743. Maximize Cyclic Partition Score](https://leetcode.com/problems/maximize-cyclic-partition-score/) (Minkowski sum)
- [LCP 14. Partition Array](https://leetcode.cn/problems/qie-fen-shu-zu/)
- [LCP 59. Build Bridges to Cross the River](https://leetcode.cn/problems/NfY1m5/) (Slope Trick)
- [2263. Make Array Non-decreasing or Non-increasing](https://leetcode.com/problems/make-array-non-decreasing-or-non-increasing/) 🔒 (Slope Trick)
- [3916. Number of Zigzag Arrays III](https://leetcode.com/problems/number-of-zigzag-arrays-iii/) 🔒 (Lagrange interpolation)

For binary lifting, see the LCA / binary lifting section of the data-structure list.

## XII. Tree DP

Note: some feel tree DP doesn't revisit the same state (no overlapping subproblems) and is just ordinary recursion. There's some merit to that, but since the bottom-up mindset matches DP, it is still called tree DP. Top-down recursion does have overlapping subproblems and usually needs memoized search.

### §12.1 Tree Diameter

- [543. Diameter of Binary Tree](https://leetcode.com/problems/diameter-of-binary-tree/)
- [687. Longest Univalue Path](https://leetcode.com/problems/longest-univalue-path/)
- [124. Binary Tree Maximum Path Sum](https://leetcode.com/problems/binary-tree-maximum-path-sum/)
- [2385. Amount of Time for Binary Tree to Be Infected](https://leetcode.com/problems/amount-of-time-for-binary-tree-to-be-infected/) 1711
- [2246. Longest Path With Different Adjacent Characters](https://leetcode.com/problems/longest-path-with-different-adjacent-characters/) 2126
- [3203. Find Minimum Diameter After Merging Two Trees](https://leetcode.com/problems/find-minimum-diameter-after-merging-two-trees/) 2266
- [1617. Count Subtrees With Max Distance Between Cities](https://leetcode.com/problems/count-subtrees-with-max-distance-between-cities/) 2309
- [2538. Difference Between Maximum and Minimum Price Sum](https://leetcode.com/problems/difference-between-maximum-and-minimum-price-sum/) 2398
- [1522. Diameter of N-Ary Tree](https://leetcode.com/problems/diameter-of-n-ary-tree/) 🔒
- [1245. Tree Diameter](https://leetcode.com/problems/tree-diameter/) 🔒
- [549. Binary Tree Longest Consecutive Sequence II](https://leetcode.com/problems/binary-tree-longest-consecutive-sequence-ii/) 🔒
- [3372. Maximize the Number of Target Nodes After Connecting Trees I](https://leetcode.com/problems/maximize-the-number-of-target-nodes-after-connecting-trees-i/) (algorithmic optimization)

> Note: the diameter can also be found with two DFS passes.

### §12.2 Maximum Independent Set on a Tree

- [337. House Robber III](https://leetcode.com/problems/house-robber-iii/) (classic: party without bosses)
- [2646. Minimize the Total Price of the Trips](https://leetcode.com/problems/minimize-the-total-price-of-the-trips/) 2238
- [3544. Subtree Inversion Sum](https://leetcode.com/problems/subtree-inversion-sum/) 2545 (memoized search / tree push DP)
- [2378. Choose Edges to Maximize Score in a Tree](https://leetcode.com/problems/choose-edges-to-maximize-score-in-a-tree/) 🔒
- [3949. Subtree Inversion Sum II](https://leetcode.com/problems/subtree-inversion-sum-ii/) 🔒

### §12.3 Minimum Dominating Set on a Tree

- [968. Binary Tree Cameras](https://leetcode.com/problems/binary-tree-cameras/) 2124

### §12.4 Rerooting DP

> Also called the two-pass scanning method.

Let y be a child of x. What happens when we re-root the tree from x to y?

- From x's perspective, remove subtree y; let the remaining part be F.

- When y is the root, x hangs below y, and F becomes one of y's subtrees.

- [834. Sum of Distances in Tree](https://leetcode.com/problems/sum-of-distances-in-tree/) 2197
- [2581. Count Number of Possible Root Nodes](https://leetcode.com/problems/count-number-of-possible-root-nodes/) 2228
- [3772. Maximum Subgraph Score in a Tree](https://leetcode.com/problems/maximum-subgraph-score-in-a-tree/) 2235
- [2858. Minimum Edge Reversals So Every Node Is Reachable](https://leetcode.com/problems/minimum-edge-reversals-so-every-node-is-reachable/) 2295
- [310. Minimum Height Trees](https://leetcode.com/problems/minimum-height-trees/) (can also use topological sort)
- [3241. Time Taken to Mark All Nodes](https://leetcode.com/problems/time-taken-to-mark-all-nodes/) 2522
- [3372. Maximize the Number of Target Nodes After Connecting Trees I](https://leetcode.com/problems/maximize-the-number-of-target-nodes-after-connecting-trees-i/) (achieve O((n+m)k), for large n and m but small k)

> Note: prefix/suffix decomposition can be seen as rerooting DP on a chain.

### §12.5 Other Tree DP

- [2925. Maximum Score After Applying Operations on a Tree](https://leetcode.com/problems/maximum-score-after-applying-operations-on-a-tree/) 1940
- [3068. Find the Maximum Sum of Node Values](https://leetcode.com/problems/find-the-maximum-sum-of-node-values/) 2268
- [2920. Maximum Points After Collecting Coins From All Nodes](https://leetcode.com/problems/maximum-points-after-collecting-coins-from-all-nodes/) 2351 (memoized search)
- [3575. Maximum Good Subtree Score](https://leetcode.com/problems/maximum-good-subtree-score/) 2360
- [3562. Maximum Profit from Trading Stocks with Discounts](https://leetcode.com/problems/maximum-profit-from-trading-stocks-with-discounts/) 2458 (knapsack)
- [1916. Count Ways to Build Rooms in an Ant Colony](https://leetcode.com/problems/count-ways-to-build-rooms-in-an-ant-colony/) 2486
- [3367. Maximize Sum of Weights after Edge Removals](https://leetcode.com/problems/maximize-sum-of-weights-after-edge-removals/) 2602
- [LCP 10. Binary Tree Task Scheduling](https://leetcode.cn/problems/er-cha-shu-ren-wu-diao-du/)
- [LCP 34. Binary Tree Coloring](https://leetcode.cn/problems/er-cha-shu-ran-se-UGC/)
- [LCP 64. Binary Tree Lights](https://leetcode.cn/problems/U7WvvU/)
- [2313. Minimum Flips in Binary Tree to Get Result](https://leetcode.com/problems/minimum-flips-in-binary-tree-to-get-result/) 🔒

## XIII. Graph DP

- [3243. Shortest Distance After Road Addition Queries I](https://leetcode.com/problems/shortest-distance-after-road-addition-queries-i/) 1568
- [787. Cheapest Flights Within K Stops](https://leetcode.com/problems/cheapest-flights-within-k-stops/) 1786
- [1786. Number of Restricted Paths From First to Last Node](https://leetcode.com/problems/number-of-restricted-paths-from-first-to-last-node/) 2079
- [2050. Parallel Courses III](https://leetcode.com/problems/parallel-courses-iii/) 2084 (DAG)
- [3620. Network Recovery Pathways](https://leetcode.com/problems/network-recovery-pathways/) (DAG)
- [1976. Number of Ways to Arrive at Destination](https://leetcode.com/problems/number-of-ways-to-arrive-at-destination/) 2095
- [3543. Maximum Weighted K-Edge Path](https://leetcode.com/problems/maximum-weighted-k-edge-path/) 2110 (DAG; bitset)
- [1857. Largest Color Value in a Directed Graph](https://leetcode.com/problems/largest-color-value-in-a-directed-graph/) 2313 (DAG)
- [1928. Minimum Cost to Reach Destination in Time](https://leetcode.com/problems/minimum-cost-to-reach-destination-in-time/) 2413
- [913. Cat and Mouse](https://leetcode.com/problems/cat-and-mouse/) 2800 (topological order)
- [1728. Cat and Mouse II](https://leetcode.com/problems/cat-and-mouse-ii/) 2849 (topological order)
- [LCP 07. Pass Messages](https://leetcode.cn/problems/chuan-di-xin-xi/)
- [1548. The Most Similar Path in a Graph](https://leetcode.com/problems/the-most-similar-path-in-a-graph/) 🔒

See also "All-Pairs Shortest Path: Floyd" in the Graph Algorithms list, which is essentially multi-dimensional DP.

## XIV. Game Theory DP

- [1025. Divisor Game](https://leetcode.com/problems/divisor-game/) 1435 (has a math approach)
- [877. Stone Game](https://leetcode.com/problems/stone-game/) 1590 (has a math approach)
- [486. Predict the Winner](https://leetcode.com/problems/predict-the-winner/)
- [1510. Stone Game IV](https://leetcode.com/problems/stone-game-iv/) 1787
- [1690. Stone Game VII](https://leetcode.com/problems/stone-game-vii/) 1951
- [1406. Stone Game III](https://leetcode.com/problems/stone-game-iii/) 2027
- [1140. Stone Game II](https://leetcode.com/problems/stone-game-ii/) 2035
- [1563. Stone Game V](https://leetcode.com/problems/stone-game-v/) 2087
- [464. Can I Win](https://leetcode.com/problems/can-i-win/)
- [1872. Stone Game VIII](https://leetcode.com/problems/stone-game-viii/) 2440
- [913. Cat and Mouse](https://leetcode.com/problems/cat-and-mouse/) 2800
- [1728. Cat and Mouse II](https://leetcode.com/problems/cat-and-mouse-ii/) 2849
- [294. Flip Game II](https://leetcode.com/problems/flip-game-ii/) 🔒

## XV. Probability / Expectation DP

- [688. Knight Probability in Chessboard](https://leetcode.com/problems/knight-probability-in-chessboard/)
- [837. New 21 Game](https://leetcode.com/problems/new-21-game/) 2350
- [1467. Probability of a Two Boxes Having The Same Number of Distinct Balls](https://leetcode.com/problems/probability-of-a-two-boxes-having-the-same-number-of-distinct-balls/) 2357
- [808. Soup Servings](https://leetcode.com/problems/soup-servings/) 2397
- [LCR 185. Probability of Dice Roll Sums](https://leetcode.cn/problems/nge-tou-zi-de-dian-shu-lcof/)
- [Ubiquant-04. Chip Game](https://leetcode.cn/contest/ubiquant2022/problems/I3Gm2h/)
- [1230. Toss Strange Coins](https://leetcode.com/problems/toss-strange-coins/) 🔒

## Topic: Output a Specific Solution

Note the difference from backtracking: some backtracking problems require all solutions, while here only one is required.

- [368. Largest Divisible Subset](https://leetcode.com/problems/largest-divisible-subset/)
- [1363. Largest Multiple of Three](https://leetcode.com/problems/largest-multiple-of-three/) 1823 (lexicographic)
- [1449. Form Largest Integer With Digits That Add up to Target](https://leetcode.com/problems/form-largest-integer-with-digits-that-add-up-to-target/) 1927 (lexicographic)
- [1092. Shortest Common Supersequence](https://leetcode.com/problems/shortest-common-supersequence/) 1977
- [943. Find the Shortest Superstring](https://leetcode.com/problems/find-the-shortest-superstring/) 2186
- [1125. Smallest Sufficient Team](https://leetcode.com/problems/smallest-sufficient-team/) 2251
- [3533. Concatenated Divisibility](https://leetcode.com/problems/concatenated-divisibility/) 2257 (lexicographic; brute force)
- [3260. Find the Largest Palindrome Divisible by K](https://leetcode.com/problems/find-the-largest-palindrome-divisible-by-k/) 2370 (lexicographic; brute force)
- [3149. Find the Minimum Cost Array Permutation](https://leetcode.com/problems/find-the-minimum-cost-array-permutation/) 2642 (lexicographic)
- [3441. Minimum Cost Good Caption](https://leetcode.com/problems/minimum-cost-good-caption/) 2765 (lexicographic)
- [3348. Smallest Divisible Digit Product II](https://leetcode.com/problems/smallest-divisible-digit-product-ii/) 3101 (lexicographic; brute force)
- [656. Coin Path](https://leetcode.com/problems/coin-path/) 🔒 (lexicographic)
- [471. Encode String with Shortest Length](https://leetcode.com/problems/encode-string-with-shortest-length/) 🔒

## Topic: Prefix/Suffix Decomposition

Some problems can also be solved with state-machine DP or grouped loops (see the two-pointers list).

If only a few elements are involved rather than a whole prefix/suffix, you can also think "enumerate right, maintain left" (see the data-structures list).

- [724. Find Pivot Index](https://leetcode.com/problems/find-pivot-index/) (achieve O(n))
- [1991. Find the Middle Index in Array](https://leetcode.com/problems/find-the-middle-index-in-array/) (same as 724)
- [2574. Left and Right Sum Differences](https://leetcode.com/problems/left-and-right-sum-differences/) 1206
- [3707. Equal Score Substrings](https://leetcode.com/problems/equal-score-substrings/) 1262
- [3912. Valid Elements in an Array](https://leetcode.com/problems/valid-elements-in-an-array/) 1273
- [3788. Maximum Score of a Split](https://leetcode.com/problems/maximum-score-of-a-split/) 1306
- [2270. Number of Ways to Split Array](https://leetcode.com/problems/number-of-ways-to-split-array/) 1334
- [3904. Smallest Stable Index II](https://leetcode.com/problems/smallest-stable-index-ii/) 1352
- [2256. Minimum Average Difference](https://leetcode.com/problems/minimum-average-difference/) 1395
- [1422. Maximum Score After Splitting a String](https://leetcode.com/problems/maximum-score-after-splitting-a-string/) (achieve O(n))
- [238. Product of Array Except Self](https://leetcode.com/problems/product-of-array-except-self/)
- [1493. Longest Subarray Of 1s After Deleting One Element](https://leetcode.com/problems/longest-subarray-of-1s-after-deleting-one-element/) 1423
- [845. Longest Mountain In Array](https://leetcode.com/problems/longest-mountain-in-array/) 1437 (can also use a grouped loop)
- [2012. Sum of Beauty in the Array](https://leetcode.com/problems/sum-of-beauty-in-the-array/) 1468
- [2909. Minimum Sum of Mountain Triplets II](https://leetcode.com/problems/minimum-sum-of-mountain-triplets-ii/) 1479
- [2483. Minimum Penalty for a Shop](https://leetcode.com/problems/minimum-penalty-for-a-shop/) 1495
- [1525. Number of Good Ways to Split a String](https://leetcode.com/problems/number-of-good-ways-to-split-a-string/) 1500
- [3583. Count Special Triplets](https://leetcode.com/problems/count-special-triplets/) 1510
- [3354. Make Array Elements Equal to Zero](https://leetcode.com/problems/make-array-elements-equal-to-zero/) (achieve O(n))
- [1930. Unique Length-3 Palindromic Subsequences](https://leetcode.com/problems/unique-length-3-palindromic-subsequences/) 1533
- [2780. Minimum Index of a Valid Split](https://leetcode.com/problems/minimum-index-of-a-valid-split/) 1550
- [2874. Maximum Value of an Ordered Triplet II](https://leetcode.com/problems/maximum-value-of-an-ordered-triplet-ii/) 1583
- [1664. Ways to Make a Fair Array](https://leetcode.com/problems/ways-to-make-a-fair-array/) 1590
- [123. Best Time to Buy and Sell Stock III](https://leetcode.com/problems/best-time-to-buy-and-sell-stock-iii/) (split into two instances of 121)
- [3698. Split Array With Minimum Difference](https://leetcode.com/problems/split-array-with-minimum-difference/) 1649
- [3598. Longest Common Prefix Between Adjacent Strings After Removals](https://leetcode.com/problems/longest-common-prefix-between-adjacent-strings-after-removals/) 1655
- [2222. Number of Ways to Select Buildings](https://leetcode.com/problems/number-of-ways-to-select-buildings/) 1657
- [1031. Maximum Sum of Two Non-Overlapping Subarrays](https://leetcode.com/problems/maximum-sum-of-two-non-overlapping-subarrays/) 1680
- [689. Maximum Sum of 3 Non-Overlapping Subarrays](https://leetcode.com/problems/maximum-sum-of-3-non-overlapping-subarrays/)
- [2420. Find All Good Indices](https://leetcode.com/problems/find-all-good-indices/) 1695
- [3862. Find The Smallest Balanced Index](https://leetcode.com/problems/find-the-smallest-balanced-index/) 1697
- [2100. Find Good Days to Rob the Bank](https://leetcode.com/problems/find-good-days-to-rob-the-bank/) 1702
- [926. Flip String to Monotone Increasing](https://leetcode.com/problems/flip-string-to-monotone-increasing/)
- [334. Increasing Triplet Subsequence](https://leetcode.com/problems/increasing-triplet-subsequence/)
- [1653. Minimum Deletions to Make String Balanced](https://leetcode.com/problems/minimum-deletions-to-make-string-balanced/) 1794
- [1186. Maximum Subarray Sum with One Deletion](https://leetcode.com/problems/maximum-subarray-sum-with-one-deletion/) 1799
- [3738. Longest Non Decreasing Subarray After Replacing At Most One Element](https://leetcode.com/problems/longest-non-decreasing-subarray-after-replacing-at-most-one-element/) 1811
- [42. Trapping Rain Water](https://leetcode.com/problems/trapping-rain-water/)
- [2711. Difference of Number of Distinct Values on Diagonals](https://leetcode.com/problems/difference-of-number-of-distinct-values-on-diagonals/) (achieve O(mn))
- [1477. Find Two Non-overlapping Sub-arrays Each With Target Sum](https://leetcode.com/problems/find-two-non-overlapping-sub-arrays-each-with-target-sum/) 1851
- [2680. Maximum OR](https://leetcode.com/problems/maximum-or/) 1912
- [1671. Minimum Number of Removals to Make Mountain Array](https://leetcode.com/problems/minimum-number-of-removals-to-make-mountain-array/) 1913
- [3891. Minimum Increase to Maximize Special Indices](https://leetcode.com/problems/minimum-increase-to-maximize-special-indices/) 1953
- [3872. Longest Arithmetic Sequence After Changing At Most One Element](https://leetcode.com/problems/longest-arithmetic-sequence-after-changing-at-most-one-element/) 2042
- [2906. Construct Product Matrix](https://leetcode.com/problems/construct-product-matrix/) 2075
- [3334. Find the Maximum Factor Score of Array](https://leetcode.com/problems/find-the-maximum-factor-score-of-array/) (non-brute-force approach)
- [3830. Longest Alternating Subarray After Removing At Most One Element](https://leetcode.com/problems/longest-alternating-subarray-after-removing-at-most-one-element/) 2162
- [2167. Minimum Time to Remove All Cars Containing Illegal Goods](https://leetcode.com/problems/minimum-time-to-remove-all-cars-containing-illegal-goods/) 2219
- [2484. Count Palindromic Subsequences](https://leetcode.com/problems/count-palindromic-subsequences/) 2223
- [2163. Minimum Difference in Sums After Removal of Elements](https://leetcode.com/problems/minimum-difference-in-sums-after-removal-of-elements/) 2225
- [2565. Subsequence With The Minimum Score](https://leetcode.com/problems/subsequence-with-the-minimum-score/) 2432
- [1995. Count Special Quadruplets](https://leetcode.com/problems/count-special-quadruplets/) (four numbers)
- [2552. Count Increasing Quadruplets](https://leetcode.com/problems/count-increasing-quadruplets/) 2433 (four numbers)
- [3302. Find The Lexicographically Smallest Valid Sequence](https://leetcode.com/problems/find-the-lexicographically-smallest-valid-sequence/) 2474 (advanced version of 2565)
- [3404. Count Special Subsequences](https://leetcode.com/problems/count-special-subsequences/) 2445 (four numbers)
- [3303. Find the Occurrence of First Almost Equal Substring](https://leetcode.com/problems/find-the-occurrence-of-first-almost-equal-substring/) 2509
- [3287. Find the Maximum Sequence Value of Array](https://leetcode.com/problems/find-the-maximum-sequence-value-of-array/) 2545
- [3257. Maximum Value Sum by Placing Three Rooks II](https://leetcode.com/problems/maximum-value-sum-by-placing-three-rooks-ii/) 2553
- [3410. Maximize Subarray Sum After Removing All Occurrences of One Element](https://leetcode.com/problems/maximize-subarray-sum-after-removing-all-occurrences-of-one-element/) 2844
- [3003. Maximize the Number of Partitions After Operations](https://leetcode.com/problems/maximize-the-number-of-partitions-after-operations/) 3039
- [487. Max Consecutive Ones II](https://leetcode.com/problems/max-consecutive-ones-ii/) 🔒
- [1746. Maximum Subarray Sum After One Operation](https://leetcode.com/problems/maximum-subarray-sum-after-one-operation/) 🔒

**Additional problems**:

- [121. Best Time to Buy and Sell Stock](https://leetcode.com/problems/best-time-to-buy-and-sell-stock/) (given a length-n prices array, return a length-n answer array where answer[i] is the answer to problem 121 under the constraint that trading is forbidden on day i (i.e. prices[i] is removed))

## Topic: Jump Game

- [1306. Jump Game III](https://leetcode.com/problems/jump-game-iii/) 1397
- [2770. Maximum Number of Jumps to Reach the Last Index](https://leetcode.com/problems/maximum-number-of-jumps-to-reach-the-last-index/) 1533
- [403. Frog Jump](https://leetcode.com/problems/frog-jump/)
- [1340. Jump Game V](https://leetcode.com/problems/jump-game-v/) 1866
- [1871. Jump Game VII](https://leetcode.com/problems/jump-game-vii/) 1896
- [1696. Jump Game VI](https://leetcode.com/problems/jump-game-vi/) 1954
- [975. Odd Even Jump](https://leetcode.com/problems/odd-even-jump/) 2079
- [1654. Minimum Jumps to Reach Home](https://leetcode.com/problems/minimum-jumps-to-reach-home/) 2124
- [LCP 09. Minimum Jumps](https://leetcode.cn/problems/zui-xiao-tiao-yue-ci-shu/)
- [LCP 20. Express Bus](https://leetcode.cn/problems/meChtZ/)
- [656. Coin Path](https://leetcode.com/problems/coin-path/) 🔒
- [2297. Jump Game VIII](https://leetcode.com/problems/jump-game-viii/) 🔒

## Other

- [1387. Sort Integers by The Power Value](https://leetcode.com/problems/sort-integers-by-the-power-value/) 1507
- [397. Integer Replacement](https://leetcode.com/problems/integer-replacement/)
- [2998. Minimum Number of Operations to Make X and Y Equal](https://leetcode.com/problems/minimum-number-of-operations-to-make-x-and-y-equal/) 1795
- [823. Binary Trees With Factors](https://leetcode.com/problems/binary-trees-with-factors/) 1900
- [1553. Minimum Number of Days to Eat N Oranges](https://leetcode.com/problems/minimum-number-of-days-to-eat-n-oranges/) 2048
- [2930. Number of Strings Which Can Be Rearranged to Contain Substring](https://leetcode.com/problems/number-of-strings-which-can-be-rearranged-to-contain-substring/) 2227
- [1896. Minimum Cost to Change the Final Value of Expression](https://leetcode.com/problems/minimum-cost-to-change-the-final-value-of-expression/) 2532

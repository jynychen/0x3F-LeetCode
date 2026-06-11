# Dynamic Programming

> Problem list from [0x3F's LeetCode Problem Lists](https://leetcode.cn/circle/discuss/tXLS3i/)

Preface

**Memoized search** is a beginner-friendly approach (useful even for advanced problems). Recommended: [DP Introduction: From Memoization to Tabulation](/link/?target=https%3A%2F%2Fwww.bilibili.com%2Fvideo%2FBV1Xj411K7oF%2F).

## Basics DP
-------

### §1.1 Climbing Stairs

*   [70. Climbing Stairs](https://leetcode.com/problems/climbing-stairs/)
*   [746. Min Cost Climbing Stairs](https://leetcode.com/problems/min-cost-climbing-stairs/) 1500
*   [3693. Climbing Stairs Ii](https://leetcode.com/problems/climbing-stairs-ii/) 1560
*   [377. Combination Sum Iv](https://leetcode.com/problems/combination-sum-iv/) 1600
*   [2466. Count Ways to Build Good Strings](https://leetcode.com/problems/count-ways-to-build-good-strings/) 1694
*   [2266. Count Number of Texts](https://leetcode.com/problems/count-number-of-texts/) 1857
*   [2533. Number of Good Binary Strings](https://leetcode.com/problems/number-of-good-binary-strings/) (Premium)

### §1.2 House Robber

#### FAQ

**Q**: When converting memoized search to tabulation, how to determine the DP array size? Why sometimes n+1, sometimes n+2?

**A**: Check the range of the memoized search parameters (min and max). For example, if i ranges from −1 (boundary) to n−1 (entry), there are n+1 distinct values, so the DP array needs size n+1. If i ranges from −2 to n−1, the array needs size n+2.

*   [198. House Robber](https://leetcode.com/problems/house-robber/)
*   [213. House Robber Ii](https://leetcode.com/problems/house-robber-ii/)
*   [2320. Count Number of Ways to Place Houses](https://leetcode.com/problems/count-number-of-ways-to-place-houses/) 1608
*   [740. Delete and Earn](https://leetcode.com/problems/delete-and-earn/)
*   [3186. Maximum Total Damage with Spell Casting](https://leetcode.com/problems/maximum-total-damage-with-spell-casting/) 1841

**Advanced Thinking**:

*   [2140. Solving Questions with Brainpower](https://leetcode.com/problems/solving-questions-with-brainpower/) 1709

### §1.3 Maximum Subarray Sum

*   [53. Maximum Subarray](https://leetcode.com/problems/maximum-subarray/) ****
*   [2606. Find the Substring with Maximum Cost](https://leetcode.com/problems/find-the-substring-with-maximum-cost/) 1422
*   [1749. Maximum Absolute Sum of Any Subarray](https://leetcode.com/problems/maximum-absolute-sum-of-any-subarray/) 1542
*   [1191. K Concatenation Maximum Sum](https://leetcode.com/problems/k-concatenation-maximum-sum/) 1748
*   [918. Maximum Sum Circular Subarray](https://leetcode.com/problems/maximum-sum-circular-subarray/) 1777
*   [2321. Maximum Score of Spliced Array](https://leetcode.com/problems/maximum-score-of-spliced-array/) 1791

**Advanced Thinking**:

*   [152. Maximum Product Subarray](https://leetcode.com/problems/maximum-product-subarray/)
*   [1186. Maximum Subarray Sum with One Deletion](https://leetcode.com/problems/maximum-subarray-sum-with-one-deletion/) 1799

### Exercises

## Grid DP

### §2.1 Basics

*   [64. Minimum Path Sum](https://leetcode.com/problems/minimum-path-sum/)
*   [62. Unique Paths](https://leetcode.com/problems/unique-paths/)
*   [63. Unique Paths Ii](https://leetcode.com/problems/unique-paths-ii/)
*   [120. Triangle](https://leetcode.com/problems/triangle/)
*   [3393. Count Paths with the Given Xor Value](https://leetcode.com/problems/count-paths-with-the-given-xor-value/) 1573
*   [931. Minimum Falling Path Sum](https://leetcode.com/problems/minimum-falling-path-sum/) 1573
*   [2684. Maximum Number of Moves in a Grid](https://leetcode.com/problems/maximum-number-of-moves-in-a-grid/) 1626
*   [3603. Minimum Cost Path with Alternating Directions Ii](https://leetcode.com/problems/minimum-cost-path-with-alternating-directions-ii/) 1639
*   [2304. Minimum Path Cost in a Grid](https://leetcode.com/problems/minimum-path-cost-in-a-grid/) 1658
*   [1289. Minimum Falling Path Sum Ii](https://leetcode.com/problems/minimum-falling-path-sum-ii/) 1697
*   [3418. Maximum Amount of Money Robot Can Earn](https://leetcode.com/problems/maximum-amount-of-money-robot-can-earn/) 1798
*   [3742. Maximum Path Score in a Grid](https://leetcode.com/problems/maximum-path-score-in-a-grid/) 1804

**Advanced Thinking**:

*   [1824. Minimum Sideway Jumps](https://leetcode.com/problems/minimum-sideway-jumps/) 1778

### §2.2 Advanced

*   [1594. Maximum Non Negative Product in a Matrix](https://leetcode.com/problems/maximum-non-negative-product-in-a-matrix/) 1807
*   [1301. Number of Paths with Max Score](https://leetcode.com/problems/number-of-paths-with-max-score/) 1853
*   [3665. Twisted Mirror Path Count](https://leetcode.com/problems/twisted-mirror-path-count/) 1883
*   [2435. Paths in Matrix Whose Sum is Divisible by K](https://leetcode.com/problems/paths-in-matrix-whose-sum-is-divisible-by-k/) 1952
*   [174. Dungeon Game](https://leetcode.com/problems/dungeon-game/)
*   [329. Longest Increasing Path in a Matrix](https://leetcode.com/problems/longest-increasing-path-in-a-matrix/)
*   [2328. Number of Increasing Paths in a Grid](https://leetcode.com/problems/number-of-increasing-paths-in-a-grid/) 2001
*   [2267. Check If There is a Valid Parentheses String Path](https://leetcode.com/problems/check-if-there-is-a-valid-parentheses-string-path/) 2085
*   [1937. Maximum Number of Points with Cost](https://leetcode.com/problems/maximum-number-of-points-with-cost/) 2106
*   [3363. Find the Maximum Number of Fruits Collected](https://leetcode.com/problems/find-the-maximum-number-of-fruits-collected/) 2200
*   [1463. Cherry Pickup Ii](https://leetcode.com/problems/cherry-pickup-ii/)
*   [741. Cherry Pickup](https://leetcode.com/problems/cherry-pickup/)
*   [3459. Length of Longest V Shaped Diagonal Segment](https://leetcode.com/problems/length-of-longest-v-shaped-diagonal-segment/) 2337
*   [2510. Check If There is a Path with Equal Number of 0s and 1s](https://leetcode.com/problems/check-if-there-is-a-path-with-equal-number-of-0s-and-1s/) (Premium)

## Knapsack
----

### §3.1 0-1 Knapsack

*   [416. Partition Equal Subset Sum](https://leetcode.com/problems/partition-equal-subset-sum/)
*   [494. Target Sum](https://leetcode.com/problems/target-sum/)
*   [2915. Length of the Longest Subsequence that Sums to Target](https://leetcode.com/problems/length-of-the-longest-subsequence-that-sums-to-target/) 1659
*   [2787. Ways to Express an Integer As Sum of Powers](https://leetcode.com/problems/ways-to-express-an-integer-as-sum-of-powers/) 1818
*   [3180. Maximum Total Reward Using Operations I](https://leetcode.com/problems/maximum-total-reward-using-operations-i/) 1849

**Advanced**:

*   [474. Ones and Zeroes](https://leetcode.com/problems/ones-and-zeroes/)
*   [3489. Zero Array Transformation Iv](https://leetcode.com/problems/zero-array-transformation-iv/) 2068
*   [3685. Subsequence Sum after Capping Elements](https://leetcode.com/problems/subsequence-sum-after-capping-elements/) 2073
*   [1049. Last Stone Weight Ii](https://leetcode.com/problems/last-stone-weight-ii/) 2092
*   [1774. Closest Dessert Cost](https://leetcode.com/problems/closest-dessert-cost/)
*   [879. Profitable Schemes](https://leetcode.com/problems/profitable-schemes/) 2204
*   [3082. Find the Sum of the Power of All Subsequences](https://leetcode.com/problems/find-the-sum-of-the-power-of-all-subsequences/) 2242
*   [956. Tallest Billboard](https://leetcode.com/problems/tallest-billboard/) 2381
*   [2518. Number of Great Partitions](https://leetcode.com/problems/number-of-great-partitions/) 2415
*   [2742. Painting the Walls](https://leetcode.com/problems/painting-the-walls/) 2425
*   [3287. Find the Maximum Sequence Value of Array](https://leetcode.com/problems/find-the-maximum-sequence-value-of-array/) 2545
*   [3181. Maximum Total Reward Using Operations Ii](https://leetcode.com/problems/maximum-total-reward-using-operations-ii/) 2688 bitset
*   [LCP 47. Ops9bm](https://leetcode.com/problems/oPs9Bm/)
*   [2291. Maximum Profit from Trading Stocks](https://leetcode.com/problems/maximum-profit-from-trading-stocks/) (Premium)
*   [2431. Maximize Total Tastiness of Purchased Fruits](https://leetcode.com/problems/maximize-total-tastiness-of-purchased-fruits/) (Premium)
*   [3647. Maximum Weight in Two Bags](https://leetcode.com/problems/maximum-weight-in-two-bags/) (Premium)
*   [2189. Number of Ways to Build House of Cards](https://leetcode.com/problems/number-of-ways-to-build-house-of-cards/) (Premium)

### §3.2 Unbounded Knapsack

*   [322. Coin Change](https://leetcode.com/problems/coin-change/)
*   [518. Coin Change Ii](https://leetcode.com/problems/coin-change-ii/)
*   [279. Perfect Squares](https://leetcode.com/problems/perfect-squares/)
*   [3610. Minimum Number of Primes to Sum to Target](https://leetcode.com/problems/minimum-number-of-primes-to-sum-to-target/) (Premium)
*   [3183. The Number of Ways to Make the Sum](https://leetcode.com/problems/the-number-of-ways-to-make-the-sum/) (Premium)

**Advanced Thinking**:

*   [3592. Inverse Coin Change](https://leetcode.com/problems/inverse-coin-change/) 1701
*   [1449. Form Largest Integer with Digits that Add Up to Target](https://leetcode.com/problems/form-largest-integer-with-digits-that-add-up-to-target/) 1927

### §3.3 Bounded Knapsack (Optional)

**Count Solutions**

*   [2585. Number of Ways to Earn Points](https://leetcode.com/problems/number-of-ways-to-earn-points/) 1910
*   [3333. Find the Original Typed String Ii](https://leetcode.com/problems/find-the-original-typed-string-ii/) 2629
*   [2902. Count of Sub Multisets with Bounded Sum](https://leetcode.com/problems/count-of-sub-multisets-with-bounded-sum/) 2759

**Binary Optimization**

*   [3489. Zero Array Transformation Iv](https://leetcode.com/problems/zero-array-transformation-iv/)

### §3.4 Grouped Knapsack

*   [1155. Number of Dice Rolls with Target Sum](https://leetcode.com/problems/number-of-dice-rolls-with-target-sum/) 1654
*   [1981. Minimize the Difference Between Target and Chosen Elements](https://leetcode.com/problems/minimize-the-difference-between-target-and-chosen-elements/) 2010
*   [2218. Maximum Value of K Coins from Piles](https://leetcode.com/problems/maximum-value-of-k-coins-from-piles/) 2158

### §3.5 Tree Knapsack (Optional)

*   [3562. Maximum Profit from Trading Stocks with Discounts](https://leetcode.com/problems/maximum-profit-from-trading-stocks-with-discounts/) 2458

## Classic Linear DP
---------

### §4.1 Longest Common Subsequence (LCS)

#### §4.1.1 Basics

*   [1143. Longest Common Subsequence](https://leetcode.com/problems/longest-common-subsequence/)
*   [583. Delete Operation for Two Strings](https://leetcode.com/problems/delete-operation-for-two-strings/)
*   [712. Minimum Ascii Delete Sum for Two Strings](https://leetcode.com/problems/minimum-ascii-delete-sum-for-two-strings/)
*   [72. Edit Distance](https://leetcode.com/problems/edit-distance/)
*   [1035. Uncrossed Lines](https://leetcode.com/problems/uncrossed-lines/) 1806
*   [1458. Max Dot Product of Two Subsequences](https://leetcode.com/problems/max-dot-product-of-two-subsequences/) 1824

**Advanced Thinking**:

*   [718. Maximum Length of Repeated Subarray](https://leetcode.com/problems/maximum-length-of-repeated-subarray/)

#### §4.1.2 Advanced

*   [3290. Maximum Multiplication Score](https://leetcode.com/problems/maximum-multiplication-score/) 1692
*   [115. Distinct Subsequences](https://leetcode.com/problems/distinct-subsequences/)
*   [3628. Maximum Number of Subsequences after One Inserting](https://leetcode.com/problems/maximum-number-of-subsequences-after-one-inserting/) 1754
*   [3316. Find Maximum Removals from Source String](https://leetcode.com/problems/find-maximum-removals-from-source-string/) 2062
*   [1639. Number of Ways to Form a Target String Given a Dictionary](https://leetcode.com/problems/number-of-ways-to-form-a-target-string-given-a-dictionary/) 2082
*   [97. Interleaving String](https://leetcode.com/problems/interleaving-string/)
*   [1092. Shortest Common Supersequence](https://leetcode.com/problems/shortest-common-supersequence/)
*   [44. Wildcard Matching](https://leetcode.com/problems/wildcard-matching/)
*   [10. Regular Expression Matching](https://leetcode.com/problems/regular-expression-matching/)

**Exercises**:

### §4.2 Longest Increasing Subsequence (LIS)

#### §4.2.1 Basics

*   [300. Longest Increasing Subsequence](https://leetcode.com/problems/longest-increasing-subsequence/)
*   [2826. Sorting Three Groups](https://leetcode.com/problems/sorting-three-groups/) 1721
*   [1671. Minimum Number of Removals to Make Mountain Array](https://leetcode.com/problems/minimum-number-of-removals-to-make-mountain-array/) 1913
*   [1964. Find the Longest Valid Obstacle Course at Each Position](https://leetcode.com/problems/find-the-longest-valid-obstacle-course-at-each-position/) 1933
*   [2111. Minimum Operations to Make the Array K Increasing](https://leetcode.com/problems/minimum-operations-to-make-the-array-k-increasing/) 1941

#### §4.2.2 Advanced

*   [354. Russian Doll Envelopes](https://leetcode.com/problems/russian-doll-envelopes/)
*   [1626. Best Team with No Conflicts](https://leetcode.com/problems/best-team-with-no-conflicts/) 2027
*   [1691. Maximum Height by Stacking Cuboids](https://leetcode.com/problems/maximum-height-by-stacking-cuboids/) 2172
*   [960. Delete Columns to Make Sorted Iii](https://leetcode.com/problems/delete-columns-to-make-sorted-iii/) 2247
*   [2407. Longest Increasing Subsequence Ii](https://leetcode.com/problems/longest-increasing-subsequence-ii/) 2280
*   [673. Number of Longest Increasing Subsequence](https://leetcode.com/problems/number-of-longest-increasing-subsequence/)
*   [1187. Make Array Strictly Increasing](https://leetcode.com/problems/make-array-strictly-increasing/) 2316
*   [1713. Minimum Operations to Make a Subsequence](https://leetcode.com/problems/minimum-operations-to-make-a-subsequence/) 2351  LIS  LCS
*   [3288. Length of the Longest Increasing Path](https://leetcode.com/problems/length-of-the-longest-increasing-path/) 2450

**Advanced Thinking**:

*   [368. Largest Divisible Subset](https://leetcode.com/problems/largest-divisible-subset/) 1800
*   [2901. Longest Unequal Adjacent Groups Subsequence Ii](https://leetcode.com/problems/longest-unequal-adjacent-groups-subsequence-ii/) 1899

**Exercises**:

### §5.1 Can We Partition?

*   [2369. Check If There is a Valid Partition for the Array](https://leetcode.com/problems/check-if-there-is-a-valid-partition-for-the-array/) 1780
*   [139. Word Break](https://leetcode.com/problems/word-break/)

### §5.2 Optimal Partition

*   [132. Palindrome Partitioning Ii](https://leetcode.com/problems/palindrome-partitioning-ii/)
*   [2707. Extra Characters in a String](https://leetcode.com/problems/extra-characters-in-a-string/) 1736
*   [3196. Maximize Total Cost of Alternating Subarrays](https://leetcode.com/problems/maximize-total-cost-of-alternating-subarrays/) 1847  DP
*   [2767. Partition String Into Minimum Beautiful Substrings](https://leetcode.com/problems/partition-string-into-minimum-beautiful-substrings/) 1865
*   [91. Decode Ways](https://leetcode.com/problems/decode-ways/)
*   [639. Decode Ways Ii](https://leetcode.com/problems/decode-ways-ii/)
*   [LCR 165. Ba Shu Zi Fan Yi Cheng Zi Fu Chuan Lcof](https://leetcode.com/problems/ba-shu-zi-fan-yi-cheng-zi-fu-chuan-lcof/)
*   [1043. Partition Array for Maximum Sum](https://leetcode.com/problems/partition-array-for-maximum-sum/) 1916
*   [3144. Minimum Substring Partition of Equal Character Frequency](https://leetcode.com/problems/minimum-substring-partition-of-equal-character-frequency/) 1917
*   [1416. Restore the Array](https://leetcode.com/problems/restore-the-array/) 1920
*   [2472. Maximum Number of Non Overlapping Palindrome Substrings](https://leetcode.com/problems/maximum-number-of-non-overlapping-palindrome-substrings/) 2013
*   [1105. Filling Bookcase Shelves](https://leetcode.com/problems/filling-bookcase-shelves/) 2014
*   [2547. Minimum Cost to Split an Array](https://leetcode.com/problems/minimum-cost-to-split-an-array/) 2020
*   [3578. Count Partitions with Max Min Difference at Most K](https://leetcode.com/problems/count-partitions-with-max-min-difference-at-most-k/) 2033
*   [2430. Maximum Deletions on a String](https://leetcode.com/problems/maximum-deletions-on-a-string/) 2102
*   [2463. Minimum Total Distance Traveled](https://leetcode.com/problems/minimum-total-distance-traveled/) 2454
*   [3579. Minimum Steps to Convert String with Operations](https://leetcode.com/problems/minimum-steps-to-convert-string-with-operations/) 2493
*   [3500. Minimum Cost to Divide Array Into Subarrays](https://leetcode.com/problems/minimum-cost-to-divide-array-into-subarrays/) 2569
*   [2977. Minimum Cost to Convert String Ii](https://leetcode.com/problems/minimum-cost-to-convert-string-ii/) 2696
*   [3441. Minimum Cost Good Caption](https://leetcode.com/problems/minimum-cost-good-caption/) 2765
*   [2052. Minimum Cost to Separate Sentence Into Rows](https://leetcode.com/problems/minimum-cost-to-separate-sentence-into-rows/) (Premium)
*   [2464. Minimum Subarrays in a Valid Split](https://leetcode.com/problems/minimum-subarrays-in-a-valid-split/) (Premium)

### §5.3 Constrained Partition Count

*   [813. Largest Sum of Averages](https://leetcode.com/problems/largest-sum-of-averages/) 1937
*   [3599. Partition Array to Minimize Xor](https://leetcode.com/problems/partition-array-to-minimize-xor/) 1955
*   [410. Split Array Largest Sum](https://leetcode.com/problems/split-array-largest-sum/)
*   [1278. Palindrome Partitioning Iii](https://leetcode.com/problems/palindrome-partitioning-iii/) 1979
*   [1745. Palindrome Partitioning Iv](https://leetcode.com/problems/palindrome-partitioning-iv/)
*   [1335. Minimum Difficulty of a Job Schedule](https://leetcode.com/problems/minimum-difficulty-of-a-job-schedule/) 2035
*   [1473. Paint House Iii](https://leetcode.com/problems/paint-house-iii/) 2056
*   [2209. Minimum White Tiles after Covering with Carpets](https://leetcode.com/problems/minimum-white-tiles-after-covering-with-carpets/) 2106
*   [1478. Allocate Mailboxes](https://leetcode.com/problems/allocate-mailboxes/) 2190
*   [3473. Sum of K Subarrays with Length at Least M](https://leetcode.com/problems/sum-of-k-subarrays-with-length-at-least-m/) 2274
*   [1959. Minimum Total Space Wasted with K Resizing Operations](https://leetcode.com/problems/minimum-total-space-wasted-with-k-resizing-operations/) 2310
*   [2478. Number of Beautiful Partitions](https://leetcode.com/problems/number-of-beautiful-partitions/) 2344
*   [3538. Merge Operations for Minimum Travel Time](https://leetcode.com/problems/merge-operations-for-minimum-travel-time/) 2461
*   [3505. Minimum Operations to Make Elements Within K Subarrays Equal](https://leetcode.com/problems/minimum-operations-to-make-elements-within-k-subarrays-equal/) 2539
*   [3077. Maximum Strength of K Disjoint Subarrays](https://leetcode.com/problems/maximum-strength-of-k-disjoint-subarrays/) 2557
*   [2911. Minimum Changes to Make K Semi Palindromes](https://leetcode.com/problems/minimum-changes-to-make-k-semi-palindromes/) 2608
*   [3117. Minimum Sum of Values by Dividing Array](https://leetcode.com/problems/minimum-sum-of-values-by-dividing-array/) 2735

### §6.1 Stock Trading

*   [121. Best Time to Buy and Sell Stock](https://leetcode.com/problems/best-time-to-buy-and-sell-stock/)
*   [122. Best Time to Buy and Sell Stock Ii](https://leetcode.com/problems/best-time-to-buy-and-sell-stock-ii/)
*   [123. Best Time to Buy and Sell Stock Iii](https://leetcode.com/problems/best-time-to-buy-and-sell-stock-iii/)
*   [188. Best Time to Buy and Sell Stock Iv](https://leetcode.com/problems/best-time-to-buy-and-sell-stock-iv/) k
*   [3573. Best Time to Buy and Sell Stock V](https://leetcode.com/problems/best-time-to-buy-and-sell-stock-v/) k  1777
*   [309. Best Time to Buy and Sell Stock with Cooldown](https://leetcode.com/problems/best-time-to-buy-and-sell-stock-with-cooldown/)
*   [714. Best Time to Buy and Sell Stock with Transaction Fee](https://leetcode.com/problems/best-time-to-buy-and-sell-stock-with-transaction-fee/)

### §6.2 Basics

*   [3259. Maximum Energy Boost from Two Drinks](https://leetcode.com/problems/maximum-energy-boost-from-two-drinks/) 1484
*   [2222. Number of Ways to Select Buildings](https://leetcode.com/problems/number-of-ways-to-select-buildings/) 1657
*   [2708. Maximum Strength of a Group](https://leetcode.com/problems/maximum-strength-of-a-group/) 152
*   [1567. Maximum Length of Subarray with Positive Product](https://leetcode.com/problems/maximum-length-of-subarray-with-positive-product/) 1710
*   [2786. Visit Array Positions to Maximize Score](https://leetcode.com/problems/visit-array-positions-to-maximize-score/) 1733
*   [1911. Maximum Alternating Subsequence Sum](https://leetcode.com/problems/maximum-alternating-subsequence-sum/) 1786
*   [376. Wiggle Subsequence](https://leetcode.com/problems/wiggle-subsequence/)
*   [3466. Maximum Coin Collection](https://leetcode.com/problems/maximum-coin-collection/) (Premium)

### §6.3 Advanced

*   [3628. Maximum Number of Subsequences after One Inserting](https://leetcode.com/problems/maximum-number-of-subsequences-after-one-inserting/) 1754
*   [2771. Longest Non Decreasing Subarray from Two Arrays](https://leetcode.com/problems/longest-non-decreasing-subarray-from-two-arrays/) 1792
*   [1186. Maximum Subarray Sum with One Deletion](https://leetcode.com/problems/maximum-subarray-sum-with-one-deletion/) 1799
*   [1594. Maximum Non Negative Product in a Matrix](https://leetcode.com/problems/maximum-non-negative-product-in-a-matrix/) 1807
*   [3738. Longest Non Decreasing Subarray after Replacing at Most One Element](https://leetcode.com/problems/longest-non-decreasing-subarray-after-replacing-at-most-one-element/) 1811
*   [3196. Maximize Total Cost of Alternating Subarrays](https://leetcode.com/problems/maximize-total-cost-of-alternating-subarrays/) 1847  DP
*   [935. Knight Dialer](https://leetcode.com/problems/knight-dialer/)
*   [1537. Get the Maximum Score](https://leetcode.com/problems/get-the-maximum-score/) 1961
*   [2919. Minimum Increment Operations to Make Array Beautiful](https://leetcode.com/problems/minimum-increment-operations-to-make-array-beautiful/) 2031
*   [801. Minimum Swaps to Make Sequences Increasing](https://leetcode.com/problems/minimum-swaps-to-make-sequences-increasing/) 2066
*   [3434. Maximum Frequency after Subarray Operation](https://leetcode.com/problems/maximum-frequency-after-subarray-operation/) 2094
*   [1955. Count Number of Special Subsequences](https://leetcode.com/problems/count-number-of-special-subsequences/) 2125
*   [3068. Find the Maximum Sum of Node Values](https://leetcode.com/problems/find-the-maximum-sum-of-node-values/) 2268
*   [3640. Trionic Array Ii](https://leetcode.com/problems/trionic-array-ii/) 2278
*   [2272. Substring with Largest Variance](https://leetcode.com/problems/substring-with-largest-variance/) 2516
*   [3661. Maximum Walls Destroyed by Robots](https://leetcode.com/problems/maximum-walls-destroyed-by-robots/) 2525
*   [3743. Maximize Cyclic Partition Score](https://leetcode.com/problems/maximize-cyclic-partition-score/) 3125
*   [LCP 19. Ulbdoe](https://leetcode.com/problems/UlBDOe/)
*   [276. Paint Fence](https://leetcode.com/problems/paint-fence/) (Premium)
*   [1746. Maximum Subarray Sum after One Operation](https://leetcode.com/problems/maximum-subarray-sum-after-one-operation/) (Premium)
*   [2036. Maximum Alternating Subarray Sum](https://leetcode.com/problems/maximum-alternating-subarray-sum/) (Premium)
*   [2361. Minimum Costs Using the Train Line](https://leetcode.com/problems/minimum-costs-using-the-train-line/) (Premium)
*   [3269. Constructing Two Increasing Arrays](https://leetcode.com/problems/constructing-two-increasing-arrays/) (Premium)

---------

### §7.1 1D DP

*   [3147. Taking Maximum Energy from the Mystic Dungeon](https://leetcode.com/problems/taking-maximum-energy-from-the-mystic-dungeon/) 1460
*   [2944. Minimum Number of Coins for Fruits](https://leetcode.com/problems/minimum-number-of-coins-for-fruits/) 1709
*   [2140. Solving Questions with Brainpower](https://leetcode.com/problems/solving-questions-with-brainpower/) 1709
*   [983. Minimum Cost for Tickets](https://leetcode.com/problems/minimum-cost-for-tickets/) 1786  O(n)
*   [368. Largest Divisible Subset](https://leetcode.com/problems/largest-divisible-subset/) 1800
*   [2901. Longest Unequal Adjacent Groups Subsequence Ii](https://leetcode.com/problems/longest-unequal-adjacent-groups-subsequence-ii/) 1899
*   [650. 2 Keys Keyboard](https://leetcode.com/problems/2-keys-keyboard/) 2000
*   [871. Minimum Number of Refueling Stops](https://leetcode.com/problems/minimum-number-of-refueling-stops/) 2074
*   [32. Longest Valid Parentheses](https://leetcode.com/problems/longest-valid-parentheses/)
*   [2167. Minimum Time to Remove All Cars Containing Illegal Goods](https://leetcode.com/problems/minimum-time-to-remove-all-cars-containing-illegal-goods/) 2219
*   [2188. Minimum Time to Finish the Race](https://leetcode.com/problems/minimum-time-to-finish-the-race/) 2315
*   [2896. Apply Operations to Make Two Strings Equal](https://leetcode.com/problems/apply-operations-to-make-two-strings-equal/)
*   [818. Race Car](https://leetcode.com/problems/race-car/) 2392
*   [3389. Minimum Operations to Make Character Frequencies Equal](https://leetcode.com/problems/minimum-operations-to-make-character-frequencies-equal/) 2940
*   [3464. Maximize the Distance Between Points on a Square](https://leetcode.com/problems/maximize-the-distance-between-points-on-a-square/)
*   [3205. Maximum Array Hopping Score I](https://leetcode.com/problems/maximum-array-hopping-score-i/) (Premium) O(n)
*   [1259. Handshakes that Dont Cross](https://leetcode.com/problems/handshakes-that-dont-cross/) (Premium)
*   [2597. The Number of Beautiful Subsets](https://leetcode.com/problems/the-number-of-beautiful-subsets/) DP
*   [2638. Count the Number of K Free Subsets](https://leetcode.com/problems/count-the-number-of-k-free-subsets/) (Premium)

### §7.2 Non-overlapping Intervals

*   [2830. Maximize the Profit As the Salesman](https://leetcode.com/problems/maximize-the-profit-as-the-salesman/) 1851
*   [2008. Maximum Earnings from Taxi](https://leetcode.com/problems/maximum-earnings-from-taxi/) 1872
*   [2054. Two Best Non Overlapping Events](https://leetcode.com/problems/two-best-non-overlapping-events/) 1883
*   [1235. Maximum Profit in Job Scheduling](https://leetcode.com/problems/maximum-profit-in-job-scheduling/) 2023
*   [1751. Maximum Number of Events that Can Be Attended Ii](https://leetcode.com/problems/maximum-number-of-events-that-can-be-attended-ii/) 2041
*   [3414. Maximum Score of Non Overlapping Intervals](https://leetcode.com/problems/maximum-score-of-non-overlapping-intervals/) 2723

### §7.3 Subarray DP

*   [53. Maximum Subarray](https://leetcode.com/problems/maximum-subarray/)
*   [152. Maximum Product Subarray](https://leetcode.com/problems/maximum-product-subarray/)
*   [1186. Maximum Subarray Sum with One Deletion](https://leetcode.com/problems/maximum-subarray-sum-with-one-deletion/) 1799
*   [3738. Longest Non Decreasing Subarray after Replacing at Most One Element](https://leetcode.com/problems/longest-non-decreasing-subarray-after-replacing-at-most-one-element/) 1811
*   [3524. Find X Value of Array I](https://leetcode.com/problems/find-x-value-of-array-i/) 2008
*   [3448. Count Substrings Divisible by Last Digit](https://leetcode.com/problems/count-substrings-divisible-by-last-digit/) 2387

**Advanced Thinking**:

*   [2262. Total Appeal of a String](https://leetcode.com/problems/total-appeal-of-a-string/) 2033
*   [828. Count Unique Characters of All Substrings of a Given String](https://leetcode.com/problems/count-unique-characters-of-all-substrings-of-a-given-string/) 2034
*   [467. Unique Substrings in Wraparound String](https://leetcode.com/problems/unique-substrings-in-wraparound-string/)

### §7.4 Valid Subsequence DP

*   [2501. Longest Square Streak in an Array](https://leetcode.com/problems/longest-square-streak-in-an-array/) 1480
*   [1218. Longest Arithmetic Subsequence of Given Difference](https://leetcode.com/problems/longest-arithmetic-subsequence-of-given-difference/) 1597
*   [2826. Sorting Three Groups](https://leetcode.com/problems/sorting-three-groups/) 1721
*   [1027. Longest Arithmetic Subsequence](https://leetcode.com/problems/longest-arithmetic-subsequence/) 1759
*   [2370. Longest Ideal Subsequence](https://leetcode.com/problems/longest-ideal-subsequence/) 1835
*   [873. Length of Longest Fibonacci Subsequence](https://leetcode.com/problems/length-of-longest-fibonacci-subsequence/) 1911
*   [3686. Number of Stable Subsequences](https://leetcode.com/problems/number-of-stable-subsequences/) 1969
*   [3202. Find the Maximum Length of Valid Subsequence Ii](https://leetcode.com/problems/find-the-maximum-length-of-valid-subsequence-ii/) 1974
*   [446. Arithmetic Slices Ii Subsequence](https://leetcode.com/problems/arithmetic-slices-ii-subsequence/)
*   [3351. Sum of Good Subsequences](https://leetcode.com/problems/sum-of-good-subsequences/) 2086
*   [3041. Maximize Consecutive Elements in an Array after Modification](https://leetcode.com/problems/maximize-consecutive-elements-in-an-array-after-modification/) 2231
*   [3409. Longest Subsequence with Decreasing Adjacent Difference](https://leetcode.com/problems/longest-subsequence-with-decreasing-adjacent-difference/) 2500
*   [3098. Find the Sum of Subsequence Powers](https://leetcode.com/problems/find-the-sum-of-subsequence-powers/) 2553
*   [2901. Longest Unequal Adjacent Groups Subsequence Ii](https://leetcode.com/problems/longest-unequal-adjacent-groups-subsequence-ii/)
*   [3299. Sum of Consecutive Subsequences](https://leetcode.com/problems/sum-of-consecutive-subsequences/) (Premium)

**Advanced Thinking**:

*   [1048. Longest String Chain](https://leetcode.com/problems/longest-string-chain/) 1599
*   [940. Distinct Subsequences Ii](https://leetcode.com/problems/distinct-subsequences-ii/) 1985
*   [1987. Number of Unique Good Subsequences](https://leetcode.com/problems/number-of-unique-good-subsequences/) 2422
*   [730. Count Different Palindromic Subsequences](https://leetcode.com/problems/count-different-palindromic-subsequences/)

### §7.5 Sub-rectangle DP

*   [3148. Maximum Difference Score in a Grid](https://leetcode.com/problems/maximum-difference-score-in-a-grid/) 1820
*   [221. Maximal Square](https://leetcode.com/problems/maximal-square/)
*   [1277. Count Square Submatrices with All Ones](https://leetcode.com/problems/count-square-submatrices-with-all-ones/)
*   [2088. Count Fertile Pyramids in a Land](https://leetcode.com/problems/count-fertile-pyramids-in-a-land/) 2105
*   [3197. Find the Minimum Area to Cover All Ones Ii](https://leetcode.com/problems/find-the-minimum-area-to-cover-all-ones-ii/)

### §7.6 Multi-dimensional DP

*   [2222. Number of Ways to Select Buildings](https://leetcode.com/problems/number-of-ways-to-select-buildings/) 1657  3  k ？
*   [2826. Sorting Three Groups](https://leetcode.com/problems/sorting-three-groups/) 1721
*   [2400. Number of Ways to Reach a Position after Exactly K Steps](https://leetcode.com/problems/number-of-ways-to-reach-a-position-after-exactly-k-steps/) 1751
*   [1262. Greatest Sum Divisible by Three](https://leetcode.com/problems/greatest-sum-divisible-by-three/) 1762
*   [3332. Maximum Points Tourist Can Earn](https://leetcode.com/problems/maximum-points-tourist-can-earn/) 1828
*   [3176. Find the Maximum Length of a Good Subsequence I](https://leetcode.com/problems/find-the-maximum-length-of-a-good-subsequence-i/) 1849
*   [1269. Number of Ways to Stay in the Same Place after Some Steps](https://leetcode.com/problems/number-of-ways-to-stay-in-the-same-place-after-some-steps/) 1854
*   [3250. Find the Count of Monotonic Pairs I](https://leetcode.com/problems/find-the-count-of-monotonic-pairs-i/) 1898
*   [3218. Minimum Cost for Cutting Cake I](https://leetcode.com/problems/minimum-cost-for-cutting-cake-i/)
*   [3122. Minimum Number of Operations to Satisfy Conditions](https://leetcode.com/problems/minimum-number-of-operations-to-satisfy-conditions/) 1905
*   [576. Out of Boundary Paths](https://leetcode.com/problems/out-of-boundary-paths/)
*   [403. Frog Jump](https://leetcode.com/problems/frog-jump/)
*   [3725. Count Ways to Choose Coprime Integers from Rows](https://leetcode.com/problems/count-ways-to-choose-coprime-integers-from-rows/) 1982
*   [1223. Dice Roll Simulation](https://leetcode.com/problems/dice-roll-simulation/) 2008
*   [1320. Minimum Distance to Type a Word Using Two Fingers](https://leetcode.com/problems/minimum-distance-to-type-a-word-using-two-fingers/) 2028
*   [3366. Minimum Array Sum](https://leetcode.com/problems/minimum-array-sum/) 2040
*   [1575. Count All Possible Routes](https://leetcode.com/problems/count-all-possible-routes/) 2055
*   [3154. Find Number of Ways to Reach the K Th Stair](https://leetcode.com/problems/find-number-of-ways-to-reach-the-k-th-stair/) 2071
*   [2318. Number of Distinct Roll Sequences](https://leetcode.com/problems/number-of-distinct-roll-sequences/) 2090
*   [3469. Find Minimum Cost to Remove Array Elements](https://leetcode.com/problems/find-minimum-cost-to-remove-array-elements/) 2112
*   [2746. Decremental String Concatenation](https://leetcode.com/problems/decremental-string-concatenation/) 2126
*   [1444. Number of Ways of Cutting a Pizza](https://leetcode.com/problems/number-of-ways-of-cutting-a-pizza/) 2127
*   [3320. Count the Number of Winning Sequences](https://leetcode.com/problems/count-the-number-of-winning-sequences/) 2153
*   [3429. Paint House Iv](https://leetcode.com/problems/paint-house-iv/) 2166
*   [2896. Apply Operations to Make Two Strings Equal](https://leetcode.com/problems/apply-operations-to-make-two-strings-equal/) 2172
*   [1420. Build Array Where You Can Find the Maximum Exactly K Comparisons](https://leetcode.com/problems/build-array-where-you-can-find-the-maximum-exactly-k-comparisons/) 2176
*   [3193. Count the Number of Inversions](https://leetcode.com/problems/count-the-number-of-inversions/) 2266
*   [1079. Letter Tile Possibilities](https://leetcode.com/problems/letter-tile-possibilities/) DP，
*   [1866. Number of Ways to Rearrange Sticks with K Sticks Visible](https://leetcode.com/problems/number-of-ways-to-rearrange-sticks-with-k-sticks-visible/) 2333
*   [2312. Selling Pieces of Wood](https://leetcode.com/problems/selling-pieces-of-wood/) 2363
*   [3177. Find the Maximum Length of a Good Subsequence Ii](https://leetcode.com/problems/find-the-maximum-length-of-a-good-subsequence-ii/) 2365
*   [1884. Egg Drop with 2 Eggs and N Floors](https://leetcode.com/problems/egg-drop-with-2-eggs-and-n-floors/)
*   [887. Super Egg Drop](https://leetcode.com/problems/super-egg-drop/) 2377
*   [920. Number of Music Playlists](https://leetcode.com/problems/number-of-music-playlists/) 2400
*   [514. Freedom Trail](https://leetcode.com/problems/freedom-trail/)
*   [3336. Find the Number of Subsequences with Equal Gcd](https://leetcode.com/problems/find-the-number-of-subsequences-with-equal-gcd/) 2403
*   [1388. Pizza with 3n Slices](https://leetcode.com/problems/pizza-with-3n-slices/) 2410
*   [903. Valid Permutations for Di Sequence](https://leetcode.com/problems/valid-permutations-for-di-sequence/) 2433
*   [1900. The Earliest and Latest Rounds Where Players Compete](https://leetcode.com/problems/the-earliest-and-latest-rounds-where-players-compete/) 2455
*   [1531. String Compression Ii](https://leetcode.com/problems/string-compression-ii/) 2576
*   [1883. Minimum Skips to Arrive at Meeting on Time](https://leetcode.com/problems/minimum-skips-to-arrive-at-meeting-on-time/) 2588
*   [964. Least Operators to Express Number](https://leetcode.com/problems/least-operators-to-express-number/) 2594
*   [3343. Count Number of Balanced Permutations](https://leetcode.com/problems/count-number-of-balanced-permutations/) 2615  DP
*   [1787. Make the Xor of All Segments Equal to Zero](https://leetcode.com/problems/make-the-xor-of-all-segments-equal-to-zero/) 2640
*   [3509. Maximum Product of Subsequences with an Alternating Sum Equal to K](https://leetcode.com/problems/maximum-product-of-subsequences-with-an-alternating-sum-equal-to-k/) 2703
*   [3441. Minimum Cost Good Caption](https://leetcode.com/problems/minimum-cost-good-caption/) 2765
*   [3539. Find Sum of Array Product of Magical Sequences](https://leetcode.com/problems/find-sum-of-array-product-of-magical-sequences/) 2694  DP
*   [2060. Check If an Original String Exists Given Two Encoded Strings](https://leetcode.com/problems/check-if-an-original-string-exists-given-two-encoded-strings/) 2804
*   [2809. Minimum Time to Make Array Sum at Most X](https://leetcode.com/problems/minimum-time-to-make-array-sum-at-most-x/) 2979
*   [3003. Maximize the Number of Partitions after Operations](https://leetcode.com/problems/maximize-the-number-of-partitions-after-operations/) 3039
*   [3225. Maximum Score from Grid Operations](https://leetcode.com/problems/maximum-score-from-grid-operations/) 3028 IOI2022
*   [LCP 57. Zbaueh](https://leetcode.com/problems/ZbAuEH/)
*   [LCP 43. Y1vbox](https://leetcode.com/problems/Y1VbOX/)
*   [LCP 65. 3aqs1c](https://leetcode.com/problems/3aqs1c/)
*   [LCP 36. Up5xym](https://leetcode.com/problems/Up5XYM/)
*   [LCP 38. 7rlgcr](https://leetcode.com/problems/7rLGCR/)
*   [256. Paint House](https://leetcode.com/problems/paint-house/) (Premium)
*   [265. Paint House Ii](https://leetcode.com/problems/paint-house-ii/) (Premium)
*   [3339. Find the Number of K Even Arrays](https://leetcode.com/problems/find-the-number-of-k-even-arrays/) (Premium)
*   [568. Maximum Vacation Days](https://leetcode.com/problems/maximum-vacation-days/) (Premium)
*   [1692. Count Ways to Distribute Candies](https://leetcode.com/problems/count-ways-to-distribute-candies/) (Premium)
*   [2143. Choose Numbers from Two Arrays in Range](https://leetcode.com/problems/choose-numbers-from-two-arrays-in-range/) (Premium)
*   [3269. Constructing Two Increasing Arrays](https://leetcode.com/problems/constructing-two-increasing-arrays/) (Premium)

**Advanced Thinking**:

*   [638. Shopping Offers](https://leetcode.com/problems/shopping-offers/)

## Interval DP
-------

### §8.1 Longest Palindromic Subsequence

*   [516. Longest Palindromic Subsequence](https://leetcode.com/problems/longest-palindromic-subsequence/)
*   [1312. Minimum Insertion Steps to Make a String Palindrome](https://leetcode.com/problems/minimum-insertion-steps-to-make-a-string-palindrome/) 1787
*   [3472. Longest Palindromic Subsequence after at Most K Operations](https://leetcode.com/problems/longest-palindromic-subsequence-after-at-most-k-operations/) 1884
*   [1771. Maximize Palindrome Length from Subsequences](https://leetcode.com/problems/maximize-palindrome-length-from-subsequences/) 2182
*   [730. Count Different Palindromic Subsequences](https://leetcode.com/problems/count-different-palindromic-subsequences/)
*   [1682. Longest Palindromic Subsequence Ii](https://leetcode.com/problems/longest-palindromic-subsequence-ii/) (Premium)
*   [1216. Valid Palindrome Iii](https://leetcode.com/problems/valid-palindrome-iii/) (Premium)
*   [1246. Palindrome Removal](https://leetcode.com/problems/palindrome-removal/) (Premium)

### §8.2 Interval DP

*   By property 2, f(i,j) can be reduced to subproblem f(i+1,j−1).
*   By property 3, enumerate the right endpoint of substring B, i.e., k=i+1,i+3,i+5,...,j−2, splitting f(i,j) into f(i,k) and f(k+1,j). Step size is 2 since each elimination removes 2 characters.

Answer: f(0,n−1).

*   [5. Longest Palindromic Substring](https://leetcode.com/problems/longest-palindromic-substring/)
*   [647. Palindromic Substrings](https://leetcode.com/problems/palindromic-substrings/)
*   [3040. Maximum Number of Operations with the Same Score Ii](https://leetcode.com/problems/maximum-number-of-operations-with-the-same-score-ii/) 1709
*   [375. Guess Number Higher or Lower Ii](https://leetcode.com/problems/guess-number-higher-or-lower-ii/)
*   [1130. Minimum Cost Tree from Leaf Values](https://leetcode.com/problems/minimum-cost-tree-from-leaf-values/) 1919
*   [96. Unique Binary Search Trees](https://leetcode.com/problems/unique-binary-search-trees/)
*   [1770. Maximum Score from Performing Multiplication Operations](https://leetcode.com/problems/maximum-score-from-performing-multiplication-operations/) 2068
*   [1547. Minimum Cost to Cut a Stick](https://leetcode.com/problems/minimum-cost-to-cut-a-stick/) 2116
*   [1039. Minimum Score Triangulation of Polygon](https://leetcode.com/problems/minimum-score-triangulation-of-polygon/) 2130
*   [1000. Minimum Cost to Merge Stones](https://leetcode.com/problems/minimum-cost-to-merge-stones/) 2423
*   [2019. The Score of Students Solving Math Expression](https://leetcode.com/problems/the-score-of-students-solving-math-expression/) 2584
*   [Interview 08.14. Boolean Evaluation Lcci](https://leetcode.com/problems/boolean-evaluation-lcci/)
*   [3563. Lexicographically Smallest String after Adjacent Removals](https://leetcode.com/problems/lexicographically-smallest-string-after-adjacent-removals/) 2585
*   [3277. Maximum Xor Score Subarray Queries](https://leetcode.com/problems/maximum-xor-score-subarray-queries/) 2693
*   [87. Scramble String](https://leetcode.com/problems/scramble-string/)
*   [312. Burst Balloons](https://leetcode.com/problems/burst-balloons/)
*   [664. Strange Printer](https://leetcode.com/problems/strange-printer/)
*   [546. Remove Boxes](https://leetcode.com/problems/remove-boxes/) CF1107E
*   [471. Encode String with Shortest Length](https://leetcode.com/problems/encode-string-with-shortest-length/) (Premium)
*   [3018. Maximum Number of Removal Queries that Can Be Processed I](https://leetcode.com/problems/maximum-number-of-removal-queries-that-can-be-processed-i/) (Premium)

----------------

### §9.1 Permutation Bitmask DP ① Adjacent-Independent

*   [From Set Theory to Bit Operations: Common Techniques](https://leetcode.cn/circle/discuss/CaOJ45/)

*   [526. Beautiful Arrangement](https://leetcode.com/problems/beautiful-arrangement/)
*   [3376. Minimum Time to Break Locks I](https://leetcode.com/problems/minimum-time-to-break-locks-i/)
*   [1879. Minimum Xor Sum of Two Arrays](https://leetcode.com/problems/minimum-xor-sum-of-two-arrays/) 2145
*   [2850. Minimum Moves to Spread Stones Over Grid](https://leetcode.com/problems/minimum-moves-to-spread-stones-over-grid/)
*   [1947. Maximum Compatibility Score Sum](https://leetcode.com/problems/maximum-compatibility-score-sum/)
*   [1799. Maximize Score after N Operations](https://leetcode.com/problems/maximize-score-after-n-operations/)
*   [3533. Concatenated Divisibility](https://leetcode.com/problems/concatenated-divisibility/) 2257
*   [3530. Maximum Profit from Valid Topological Order in Dag](https://leetcode.com/problems/maximum-profit-from-valid-topological-order-in-dag/) 2353
*   [2172. Maximum and Sum of Array](https://leetcode.com/problems/maximum-and-sum-of-array/) 2392
*   [2992. Number of Self Divisible Permutations](https://leetcode.com/problems/number-of-self-divisible-permutations/) (Premium)
*   [2403. Minimum Time to Kill All Monsters](https://leetcode.com/problems/minimum-time-to-kill-all-monsters/) (Premium)
*   [1066. Campus Bikes Ii](https://leetcode.com/problems/campus-bikes-ii/) (Premium)

### §9.2 Permutation Bitmask DP ② Adjacent-Dependent

*   [2741. Special Permutations](https://leetcode.com/problems/special-permutations/) 2021
*   [996. Number of Squareful Arrays](https://leetcode.com/problems/number-of-squareful-arrays/)
*   [1681. Minimum Incompatibility](https://leetcode.com/problems/minimum-incompatibility/) 2390
*   [3615. Longest Palindromic Path in Graph](https://leetcode.com/problems/longest-palindromic-path-in-graph/) 2463
*   [3283. Maximum Number of Moves to Kill All Pawns](https://leetcode.com/problems/maximum-number-of-moves-to-kill-all-pawns/) 2473
*   [3149. Find the Minimum Cost Array Permutation](https://leetcode.com/problems/find-the-minimum-cost-array-permutation/) 2642

### §9.3 Traveling Salesman Problem (TSP)

*   [943. Find the Shortest Superstring](https://leetcode.com/problems/find-the-shortest-superstring/) 2186
*   [847. Shortest Path Visiting All Nodes](https://leetcode.com/problems/shortest-path-visiting-all-nodes/) 2201
*   [LCP 13. Xun Bao](https://leetcode.com/problems/xun-bao/)
*   [2247. Maximum Cost of Trip with K Highways](https://leetcode.com/problems/maximum-cost-of-trip-with-k-highways/) (Premium)

**Similar Problems**:

*   [3568. Minimum Moves to Clean the Classroom](https://leetcode.com/problems/minimum-moves-to-clean-the-classroom/) 2143
*   [864. Shortest Path to Get All Keys](https://leetcode.com/problems/shortest-path-to-get-all-keys/) 2259

### §9.4 Subset Bitmask DP

*   [2305. Fair Distribution of Cookies](https://leetcode.com/problems/fair-distribution-of-cookies/) 1887
*   [1986. Minimum Number of Work Sessions to Finish the Tasks](https://leetcode.com/problems/minimum-number-of-work-sessions-to-finish-the-tasks/) 1995
*   [3670. Maximum Product of Two Integers with No Common Bits](https://leetcode.com/problems/maximum-product-of-two-integers-with-no-common-bits/) 2234
*   [1723. Find Minimum Time to Finish All Jobs](https://leetcode.com/problems/find-minimum-time-to-finish-all-jobs/) 2284
*   [1655. Distribute Repeating Integers](https://leetcode.com/problems/distribute-repeating-integers/) 2307
*   [3444. Minimum Increments for Target Multiples in an Array](https://leetcode.com/problems/minimum-increments-for-target-multiples-in-an-array/) 2337
*   [3575. Maximum Good Subtree Score](https://leetcode.com/problems/maximum-good-subtree-score/) 2360
*   [1349. Maximum Students Taking Exam](https://leetcode.com/problems/maximum-students-taking-exam/) 2386
*   [1681. Minimum Incompatibility](https://leetcode.com/problems/minimum-incompatibility/) 2390  O(n2⋅2n)
*   [2572. Count the Number of Square Free Subsets](https://leetcode.com/problems/count-the-number-of-square-free-subsets/) 2420
*   [1994. The Number of Good Subsets](https://leetcode.com/problems/the-number-of-good-subsets/) 2465
*   [1494. Parallel Courses Ii](https://leetcode.com/problems/parallel-courses-ii/)
*   [LCP 04. Broken Board Dominoes](https://leetcode.com/problems/broken-board-dominoes/)
*   [LCP 53. Ejvmw4](https://leetcode.com/problems/EJvmW4/)
*   [465. Optimal Account Balancing](https://leetcode.com/problems/optimal-account-balancing/) (Premium)
*   [2152. Minimum Number of Lines to Cover Points](https://leetcode.com/problems/minimum-number-of-lines-to-cover-points/) (Premium)

**Related Problems**:

*   [3594. Minimum Time to Transport All Individuals](https://leetcode.com/problems/minimum-time-to-transport-all-individuals/) 2604

### §9.5 SOS DP

Python3

Java

C++

Go

    def sos_dp(a: List[int]) -> List[int]:
        mx = max(a)
        u = 1 << w

        f = [0] * u
        for x in a:
            f[x] += 1  # initial value

        for i in range(w):
            bit = 1 << i
            s = 0
            while s < u:
                f[s] += f[s ^ bit]
                s += 1
        return f

Python3

Java

C++

Go

    def sos_dp(a: List[int]) -> List[int]:
        mx = max(a)
        u = 1 << w

        f = [0] * u
        for x in a:
            f[x] += 1  # initial value

        for i in range(w):
            bit = 1 << i
            s = 0
            while s < u:
                f[s ^ bit] += f[s]
                s += 1
        return f

*   [3670. Maximum Product of Two Integers with No Common Bits](https://leetcode.com/problems/maximum-product-of-two-integers-with-no-common-bits/) 2234
*   [2044. Count Number of Maximum Bitwise or Subsets](https://leetcode.com/problems/count-number-of-maximum-bitwise-or-subsets/)
*   [2732. Find a Good Subset of the Matrix](https://leetcode.com/problems/find-a-good-subset-of-the-matrix/)
*   [3757. Number of Effective Subsequences](https://leetcode.com/problems/number-of-effective-subsequences/)

### §9.6 Other Bitmask DP

*   [1411. Number of Ways to Paint N 3 Grid](https://leetcode.com/problems/number-of-ways-to-paint-n-3-grid/) 1845
*   [698. Partition to K Equal Sum Subsets](https://leetcode.com/problems/partition-to-k-equal-sum-subsets/)
*   [2002. Maximum Product of the Length of Two Palindromic Subsequences](https://leetcode.com/problems/maximum-product-of-the-length-of-two-palindromic-subsequences/) 1869
*   [473. Matchsticks to Square](https://leetcode.com/problems/matchsticks-to-square/)
*   [1931. Painting a Grid with Three Different Colors](https://leetcode.com/problems/painting-a-grid-with-three-different-colors/) 2170 ：1411
*   [1125. Smallest Sufficient Team](https://leetcode.com/problems/smallest-sufficient-team/) 2251
*   [1434. Number of Ways to Wear Different Hats to Each Other](https://leetcode.com/problems/number-of-ways-to-wear-different-hats-to-each-other/) 2273
*   [464. Can I Win](https://leetcode.com/problems/can-i-win/)
*   [691. Stickers to Spell Word](https://leetcode.com/problems/stickers-to-spell-word/)
*   [3276. Select Cells in Grid with Maximum Score](https://leetcode.com/problems/select-cells-in-grid-with-maximum-score/) 2403
*   [1595. Minimum Cost to Connect Two Groups of Points](https://leetcode.com/problems/minimum-cost-to-connect-two-groups-of-points/) 2538
*   [1815. Maximum Number of Groups Getting Fresh Donuts](https://leetcode.com/problems/maximum-number-of-groups-getting-fresh-donuts/) 2559
*   [1659. Maximize Grid Happiness](https://leetcode.com/problems/maximize-grid-happiness/) 2655
*   [980. Unique Paths Iii](https://leetcode.com/problems/unique-paths-iii/) ** DP**
*   [LCP 69. Rmert2](https://leetcode.com/problems/rMeRt2/)
*   [LCP 76. 1ybdkd](https://leetcode.com/problems/1ybDKD/)
*   [LCP 82. Cnhox6](https://leetcode.com/problems/cnHoX6/)
*   [351. Android Unlock Patterns](https://leetcode.com/problems/android-unlock-patterns/) (Premium)
*   [2184. Number of Ways to Build Sturdy Brick Wall](https://leetcode.com/problems/number-of-ways-to-build-sturdy-brick-wall/) (Premium)

## Digit DP
-------

### §10.1 Count Valid Elements

Python3

Java

C++

Go

    # e.g., digitDP(0, 10, 1) == 2
    def digitDP(low: int, high: int, target: int) -> int:
        high_s = list(map(int, str(high)))
        n = len(high_s)
        diff_lh = n - len(low_s)

        @cache
        def dfs(i: int, cnt0: int, limit_low: bool, limit_high: bool) -> int:
            if cnt0 > target:
                return 0  # invalid
            if i == n:
                return 1 if cnt0 == target else 0

            lo = low_s[i - diff_lh] if limit_low and i >= diff_lh else 0
            hi = high_s[i] if limit_high else 9

            res = 0
            start = lo

            if limit_low and i < diff_lh:
                res = dfs(i + 1, 0, True, False)
                start = 1

            for d in range(start, hi + 1):
                res += dfs(i + 1,
                           limit_low and d == lo,
                           limit_high and d == hi)

            # res %= MOD
            return res

        return dfs(0, 0, True, True)

*   [3747. Count Distinct Integers after Removing Zeros](https://leetcode.com/problems/count-distinct-integers-after-removing-zeros/) 1848
*   [2719. Count of Integers](https://leetcode.com/problems/count-of-integers/)
*   [1399. Count Largest Group](https://leetcode.com/problems/count-largest-group/)
*   [1742. Maximum Number of Balls in a Box](https://leetcode.com/problems/maximum-number-of-balls-in-a-box/)
*   [788. Rotated Digits](https://leetcode.com/problems/rotated-digits/)
*   [902. Numbers at Most N Given Digit Set](https://leetcode.com/problems/numbers-at-most-n-given-digit-set/) 1990
*   [600. Non Negative Integers Without Consecutive Ones](https://leetcode.com/problems/non-negative-integers-without-consecutive-ones/)
*   [2376. Count Special Integers](https://leetcode.com/problems/count-special-integers/) 2120
*   [357. Count Numbers with Unique Digits](https://leetcode.com/problems/count-numbers-with-unique-digits/)
*   [1012. Numbers with Repeated Digits](https://leetcode.com/problems/numbers-with-repeated-digits/) 2230
*   [3519. Count Numbers with Non Decreasing Digits](https://leetcode.com/problems/count-numbers-with-non-decreasing-digits/) 2246
*   [2827. Number of Beautiful Integers in the Range](https://leetcode.com/problems/number-of-beautiful-integers-in-the-range/) 2324
*   [2999. Count the Number of Powerful Integers](https://leetcode.com/problems/count-the-number-of-powerful-integers/) 2351
*   [2801. Count Stepping Numbers in Range](https://leetcode.com/problems/count-stepping-numbers-in-range/) 2367
*   [2843. Count Symmetric Integers](https://leetcode.com/problems/count-symmetric-integers/)
*   [3352. Count K Reducible Numbers Less than N](https://leetcode.com/problems/count-k-reducible-numbers-less-than-n/) 2451
*   [3621. Number of Integers with Popcount Depth Equal to K I](https://leetcode.com/problems/number-of-integers-with-popcount-depth-equal-to-k-i/)
*   [3490. Count Beautiful Numbers](https://leetcode.com/problems/count-beautiful-numbers/) 2502
*   [1397. Find All Good Strings](https://leetcode.com/problems/find-all-good-strings/) 2667
*   [1215. Stepping Numbers](https://leetcode.com/problems/stepping-numbers/) (Premium)
*   [1067. Digit Count in Range](https://leetcode.com/problems/digit-count-in-range/) (Premium)
*   [3032. Count Numbers with Unique Digits Ii](https://leetcode.com/problems/count-numbers-with-unique-digits-ii/) (Premium)

**From Low to High**:

*   [3704. Count No Zero Pairs that Sum to N](https://leetcode.com/problems/count-no-zero-pairs-that-sum-to-n/) 2419

### §10.2 Sum of Valid Element Values

Python3

Java

C++

Go

    def digitDPContribution(low: int, high: int, k: int) -> int:
        high_s = list(map(int, str(high)))
        n = len(high_s)
        diff_lh = n - len(low_s)

        @cache
        def dfs(i: int, mask: int, limit_low: bool, limit_high: bool) -> Tuple[int, int]:
            if i == n:
                return 1, 0

            lo = low_s[i - diff_lh] if limit_low and i >= diff_lh else 0
            hi = high_s[i] if limit_high else 9

            cnt = res = 0
            start = lo

            if limit_low and i < diff_lh:
                cnt, res = dfs(i + 1, 0, True, False)
                start = 1

            for d in range(start, hi + 1):
                new_mask = mask | 1 << d
                    continue
                sub_cnt, sub_sum = dfs(i + 1,
                                       new_mask,
                                       limit_low and d == lo,
                                       limit_high and d == hi)

            # cnt %= MOD; res %= MOD
            return cnt, res

        return dfs(0, 0, True, True)[1]

*   [233. Number of Digit One](https://leetcode.com/problems/number-of-digit-one/)
*   [Interview 17.06. Number of 2s in Range Lcci](https://leetcode.com/problems/number-of-2s-in-range-lcci/)
*   [3007. Maximum Number that Sum of the Prices is Less than or Equal to K](https://leetcode.com/problems/maximum-number-that-sum-of-the-prices-is-less-than-or-equal-to-k/) 2258
*   [3753. Total Waviness of Numbers in Range Ii](https://leetcode.com/problems/total-waviness-of-numbers-in-range-ii/)

### §10.3 Other Digit DP

*   [3677. Count Binary Palindromic Numbers](https://leetcode.com/problems/count-binary-palindromic-numbers/) 2223
*   [3348. Smallest Divisible Digit Product Ii](https://leetcode.com/problems/smallest-divisible-digit-product-ii/) 3101

### §11.1 Prefix Sum Optimized DP

*   [1871. Jump Game Vii](https://leetcode.com/problems/jump-game-vii/) 1896
*   [2327. Number of People Aware of a Secret](https://leetcode.com/problems/number-of-people-aware-of-a-secret/)
*   [3699. Number of Zigzag Arrays I](https://leetcode.com/problems/number-of-zigzag-arrays-i/) 2123
*   [1997. First Day Where You Have Been in All the Rooms](https://leetcode.com/problems/first-day-where-you-have-been-in-all-the-rooms/) 2260
*   [629. K Inverse Pairs Array](https://leetcode.com/problems/k-inverse-pairs-array/)
*   [3193. Count the Number of Inversions](https://leetcode.com/problems/count-the-number-of-inversions/) 2266
*   [3473. Sum of K Subarrays with Length at Least M](https://leetcode.com/problems/sum-of-k-subarrays-with-length-at-least-m/) 2274
*   [3251. Find the Count of Monotonic Pairs Ii](https://leetcode.com/problems/find-the-count-of-monotonic-pairs-ii/) 2323
*   [2478. Number of Beautiful Partitions](https://leetcode.com/problems/number-of-beautiful-partitions/) 2344
*   [837. New 21 Game](https://leetcode.com/problems/new-21-game/) 2350
*   [3077. Maximum Strength of K Disjoint Subarrays](https://leetcode.com/problems/maximum-strength-of-k-disjoint-subarrays/) 2557
*   [3333. Find the Original Typed String Ii](https://leetcode.com/problems/find-the-original-typed-string-ii/) 2629
*   [2902. Count of Sub Multisets with Bounded Sum](https://leetcode.com/problems/count-of-sub-multisets-with-bounded-sum/) 2759
*   [1977. Number of Ways to Separate Numbers](https://leetcode.com/problems/number-of-ways-to-separate-numbers/) 2817
*   [3130. Find All Possible Stable Binary Arrays Ii](https://leetcode.com/problems/find-all-possible-stable-binary-arrays-ii/) 2825

### §11.2 Monotonic Stack Optimized DP

*   [1335. Minimum Difficulty of a Job Schedule](https://leetcode.com/problems/minimum-difficulty-of-a-job-schedule/) 2035
*   [2866. Beautiful Towers Ii](https://leetcode.com/problems/beautiful-towers-ii/) 2072
*   [2617. Minimum Number of Visited Cells in a Grid](https://leetcode.com/problems/minimum-number-of-visited-cells-in-a-grid/) 2582
*   [2355. Maximum Number of Books You Can Take](https://leetcode.com/problems/maximum-number-of-books-you-can-take/) (Premium)

### §11.3 Monotonic Queue Optimized DP

*   [2944. Minimum Number of Coins for Fruits](https://leetcode.com/problems/minimum-number-of-coins-for-fruits/) 1709
*   [1696. Jump Game Vi](https://leetcode.com/problems/jump-game-vi/) 1954
*   [1425. Constrained Subsequence Sum](https://leetcode.com/problems/constrained-subsequence-sum/) 2032
*   [3578. Count Partitions with Max Min Difference at Most K](https://leetcode.com/problems/count-partitions-with-max-min-difference-at-most-k/) 2033
*   [375. Guess Number Higher or Lower Ii](https://leetcode.com/problems/guess-number-higher-or-lower-ii/)
*   [1687. Delivering Boxes from Storage to Ports](https://leetcode.com/problems/delivering-boxes-from-storage-to-ports/) 2610
*   [2463. Minimum Total Distance Traveled](https://leetcode.com/problems/minimum-total-distance-traveled/) ： O((n+m)log(n+m))
*   [3117. Minimum Sum of Values by Dividing Array](https://leetcode.com/problems/minimum-sum-of-values-by-dividing-array/) 2735
*   [2945. Find Maximum Non Decreasing Array Length](https://leetcode.com/problems/find-maximum-non-decreasing-array-length/) 2943
*   [2969. Minimum Number of Coins for Fruits Ii](https://leetcode.com/problems/minimum-number-of-coins-for-fruits-ii/) (Premium)

### §11.4 BIT/Segment Tree Optimized DP

*   [1626. Best Team with No Conflicts](https://leetcode.com/problems/best-team-with-no-conflicts/) 2027
*   [2407. Longest Increasing Subsequence Ii](https://leetcode.com/problems/longest-increasing-subsequence-ii/) 2280
*   [2770. Maximum Number of Jumps to Reach the Last Index](https://leetcode.com/problems/maximum-number-of-jumps-to-reach-the-last-index/)
*   [2926. Maximum Balanced Subsequence Sum](https://leetcode.com/problems/maximum-balanced-subsequence-sum/) 2448
*   [2547. Minimum Cost to Split an Array](https://leetcode.com/problems/minimum-cost-to-split-an-array/)
*   [3671. Sum of Beautiful Subsequences](https://leetcode.com/problems/sum-of-beautiful-subsequences/) 2647
*   [2916. Subarrays Distinct Element Sum of Squares Ii](https://leetcode.com/problems/subarrays-distinct-element-sum-of-squares-ii/) 2816  2547

### §11.5 Trie Optimized DP

*   [139. Word Break](https://leetcode.com/problems/word-break/)
*   [2707. Extra Characters in a String](https://leetcode.com/problems/extra-characters-in-a-string/)
*   [Interview 17.13. Re Space Lcci](https://leetcode.com/problems/re-space-lcci/)
*   [472. Concatenated Words](https://leetcode.com/problems/concatenated-words/) 2300
*   [2977. Minimum Cost to Convert String Ii](https://leetcode.com/problems/minimum-cost-to-convert-string-ii/) 2696

### §11.6 Matrix Exponentiation Optimized DP

**Advanced Approach**: Use **Berlekamp-Massey algorithm** to find the linear recurrence, then optimize with **Kitamasa algorithm** (or Bostan-Mori algorithm).

*   [70. Climbing Stairs](https://leetcode.com/problems/climbing-stairs/)
*   [509. Fibonacci Number](https://leetcode.com/problems/fibonacci-number/)
*   [1137. N Th Tribonacci Number](https://leetcode.com/problems/n-th-tribonacci-number/)
*   [1220. Count Vowels Permutation](https://leetcode.com/problems/count-vowels-permutation/)
*   [552. Student Attendance Record Ii](https://leetcode.com/problems/student-attendance-record-ii/)
*   [935. Knight Dialer](https://leetcode.com/problems/knight-dialer/)
*   [790. Domino and Tromino Tiling](https://leetcode.com/problems/domino-and-tromino-tiling/)
*   [1411. Number of Ways to Paint N 3 Grid](https://leetcode.com/problems/number-of-ways-to-paint-n-3-grid/)
*   [1931. Painting a Grid with Three Different Colors](https://leetcode.com/problems/painting-a-grid-with-three-different-colors/)
*   [3337. Total Characters in String after Transformations Ii](https://leetcode.com/problems/total-characters-in-string-after-transformations-ii/) 2412
*   [3700. Number of Zigzag Arrays Ii](https://leetcode.com/problems/number-of-zigzag-arrays-ii/) 2435
*   [2851. String Transformation](https://leetcode.com/problems/string-transformation/) 2858
*   [2912. Number of Ways to Reach Destination in the Grid](https://leetcode.com/problems/number-of-ways-to-reach-destination-in-the-grid/) (Premium)

### §11.7 Convex Hull Trick (Slope Optimization) DP

*   [3494. Find the Minimum Amount of Time to Brew Potions](https://leetcode.com/problems/find-the-minimum-amount-of-time-to-brew-potions/)
*   [3500. Minimum Cost to Divide Array Into Subarrays](https://leetcode.com/problems/minimum-cost-to-divide-array-into-subarrays/)
*   [3693. Climbing Stairs Ii](https://leetcode.com/problems/climbing-stairs-ii/) K\=3

### §11.8 WQS Binary Search Optimized DP

*   [188. Best Time to Buy and Sell Stock Iv](https://leetcode.com/problems/best-time-to-buy-and-sell-stock-iv/)
*   [3573. Best Time to Buy and Sell Stock V](https://leetcode.com/problems/best-time-to-buy-and-sell-stock-v/)
*   [2209. Minimum White Tiles after Covering with Carpets](https://leetcode.com/problems/minimum-white-tiles-after-covering-with-carpets/)
*   [3743. Maximize Cyclic Partition Score](https://leetcode.com/problems/maximize-cyclic-partition-score/)

### §11.9 Other Optimized DP

*   [3654. Minimum Sum after Divisible Sum Deletions](https://leetcode.com/problems/minimum-sum-after-divisible-sum-deletions/) 2039
*   [1937. Maximum Number of Points with Cost](https://leetcode.com/problems/maximum-number-of-points-with-cost/) 2106
*   [2713. Maximum Strictly Increasing Cells in a Matrix](https://leetcode.com/problems/maximum-strictly-increasing-cells-in-a-matrix/) 2387
*   [3651. Minimum Cost Path with Teleportations](https://leetcode.com/problems/minimum-cost-path-with-teleportations/) 2411
*   [2318. Number of Distinct Roll Sequences](https://leetcode.com/problems/number-of-distinct-roll-sequences/) CF1943D2
*   [3181. Maximum Total Reward Using Operations Ii](https://leetcode.com/problems/maximum-total-reward-using-operations-ii/) 2688 bitset
*   [2267. Check If There is a Valid Parentheses String Path](https://leetcode.com/problems/check-if-there-is-a-valid-parentheses-string-path/) bitset
*   [3213. Construct String with Minimum Cost](https://leetcode.com/problems/construct-string-with-minimum-cost/) /  / AC
*   [3292. Minimum Number of Valid Strings to Form Target Ii](https://leetcode.com/problems/minimum-number-of-valid-strings-to-form-target-ii/) / AC
*   [3743. Maximize Cyclic Partition Score](https://leetcode.com/problems/maximize-cyclic-partition-score/)
*   [LCP 14. Qie Fen Shu Zu](https://leetcode.com/problems/qie-fen-shu-zu/)
*   [LCP 59. Nfy1m5](https://leetcode.com/problems/NfY1m5/) Slope Trick
*   [2263. Make Array Non Decreasing or Non Increasing](https://leetcode.com/problems/make-array-non-decreasing-or-non-increasing/) (Premium)Slope Trick

### §12.1 Tree Diameter

*   [543. Diameter of Binary Tree](https://leetcode.com/problems/diameter-of-binary-tree/)
*   [687. Longest Univalue Path](https://leetcode.com/problems/longest-univalue-path/)
*   [124. Binary Tree Maximum Path Sum](https://leetcode.com/problems/binary-tree-maximum-path-sum/)
*   [2385. Amount of Time for Binary Tree to Be Infected](https://leetcode.com/problems/amount-of-time-for-binary-tree-to-be-infected/) 1711
*   [2246. Longest Path with Different Adjacent Characters](https://leetcode.com/problems/longest-path-with-different-adjacent-characters/) 2126
*   [3203. Find Minimum Diameter after Merging Two Trees](https://leetcode.com/problems/find-minimum-diameter-after-merging-two-trees/) 2266
*   [1617. Count Subtrees with Max Distance Between Cities](https://leetcode.com/problems/count-subtrees-with-max-distance-between-cities/) 2309
*   [2538. Difference Between Maximum and Minimum Price Sum](https://leetcode.com/problems/difference-between-maximum-and-minimum-price-sum/) 2398
*   [1522. Diameter of N Ary Tree](https://leetcode.com/problems/diameter-of-n-ary-tree/) (Premium)
*   [1245. Tree Diameter](https://leetcode.com/problems/tree-diameter/) (Premium)
*   [549. Binary Tree Longest Consecutive Sequence Ii](https://leetcode.com/problems/binary-tree-longest-consecutive-sequence-ii/) (Premium)
*   [3372. Maximize the Number of Target Nodes after Connecting Trees I](https://leetcode.com/problems/maximize-the-number-of-target-nodes-after-connecting-trees-i/)

### §12.2 Maximum Independent Set on Tree

*   [337. House Robber Iii](https://leetcode.com/problems/house-robber-iii/)
*   [2646. Minimize the Total Price of the Trips](https://leetcode.com/problems/minimize-the-total-price-of-the-trips/) 2238
*   [3544. Subtree Inversion Sum](https://leetcode.com/problems/subtree-inversion-sum/) 2545  /
*   [2378. Choose Edges to Maximize Score in a Tree](https://leetcode.com/problems/choose-edges-to-maximize-score-in-a-tree/) (Premium)

### §12.3 Minimum Dominating Set on Tree

*   [968. Binary Tree Cameras](https://leetcode.com/problems/binary-tree-cameras/) 2124

### §12.4 Rerooting DP

*   [834. Sum of Distances in Tree](https://leetcode.com/problems/sum-of-distances-in-tree/) 2197
*   [2581. Count Number of Possible Root Nodes](https://leetcode.com/problems/count-number-of-possible-root-nodes/) 2228
*   [2858. Minimum Edge Reversals So Every Node is Reachable](https://leetcode.com/problems/minimum-edge-reversals-so-every-node-is-reachable/) 2295
*   [310. Minimum Height Trees](https://leetcode.com/problems/minimum-height-trees/)
*   [3241. Time Taken to Mark All Nodes](https://leetcode.com/problems/time-taken-to-mark-all-nodes/) 2522
*   [3372. Maximize the Number of Target Nodes after Connecting Trees I](https://leetcode.com/problems/maximize-the-number-of-target-nodes-after-connecting-trees-i/) k)， n  m  k

### §12.5 Other Tree DP

*   [2925. Maximum Score after Applying Operations on a Tree](https://leetcode.com/problems/maximum-score-after-applying-operations-on-a-tree/) 1940
*   [3068. Find the Maximum Sum of Node Values](https://leetcode.com/problems/find-the-maximum-sum-of-node-values/) 2268
*   [2920. Maximum Points after Collecting Coins from All Nodes](https://leetcode.com/problems/maximum-points-after-collecting-coins-from-all-nodes/) 2351
*   [3575. Maximum Good Subtree Score](https://leetcode.com/problems/maximum-good-subtree-score/) 2360
*   [3562. Maximum Profit from Trading Stocks with Discounts](https://leetcode.com/problems/maximum-profit-from-trading-stocks-with-discounts/) 2458
*   [1916. Count Ways to Build Rooms in an Ant Colony](https://leetcode.com/problems/count-ways-to-build-rooms-in-an-ant-colony/) 2486
*   [3367. Maximize Sum of Weights after Edge Removals](https://leetcode.com/problems/maximize-sum-of-weights-after-edge-removals/) 2602
*   [LCP 10. Er Cha Shu Ren Wu Diao Du](https://leetcode.com/problems/er-cha-shu-ren-wu-diao-du/)
*   [LCP 34. Er Cha Shu Ran Se UGC](https://leetcode.com/problems/er-cha-shu-ran-se-UGC/)
*   [LCP 64. U7wvvu](https://leetcode.com/problems/U7WvvU/)
*   [2313. Minimum Flips in Binary Tree to Get Result](https://leetcode.com/problems/minimum-flips-in-binary-tree-to-get-result/) (Premium)

## Graph DP
-------

*   [3243. Shortest Distance after Road Addition Queries I](https://leetcode.com/problems/shortest-distance-after-road-addition-queries-i/) 1568
*   [787. Cheapest Flights Within K Stops](https://leetcode.com/problems/cheapest-flights-within-k-stops/) 1786
*   [1786. Number of Restricted Paths from First to Last Node](https://leetcode.com/problems/number-of-restricted-paths-from-first-to-last-node/) 2079
*   [2050. Parallel Courses Iii](https://leetcode.com/problems/parallel-courses-iii/) 2084 **DAG**
*   [3620. Network Recovery Pathways](https://leetcode.com/problems/network-recovery-pathways/) **DAG**
*   [1976. Number of Ways to Arrive at Destination](https://leetcode.com/problems/number-of-ways-to-arrive-at-destination/) 2095
*   [3543. Maximum Weighted K Edge Path](https://leetcode.com/problems/maximum-weighted-k-edge-path/) 2110 **DAG** bitset
*   [1857. Largest Color Value in a Directed Graph](https://leetcode.com/problems/largest-color-value-in-a-directed-graph/) 2313 **DAG**
*   [1928. Minimum Cost to Reach Destination in Time](https://leetcode.com/problems/minimum-cost-to-reach-destination-in-time/) 2413
*   [913. Cat and Mouse](https://leetcode.com/problems/cat-and-mouse/) 2800
*   [1728. Cat and Mouse Ii](https://leetcode.com/problems/cat-and-mouse-ii/) 2849
*   [LCP 07. Chuan Di Xin Xi](https://leetcode.com/problems/chuan-di-xin-xi/)
*   [1548. The Most Similar Path in a Graph](https://leetcode.com/problems/the-most-similar-path-in-a-graph/) (Premium)

*   [1025. Divisor Game](https://leetcode.com/problems/divisor-game/) 1435
*   [877. Stone Game](https://leetcode.com/problems/stone-game/) 1590
*   [486. Predict the Winner](https://leetcode.com/problems/predict-the-winner/)
*   [1510. Stone Game Iv](https://leetcode.com/problems/stone-game-iv/) 1787
*   [1690. Stone Game Vii](https://leetcode.com/problems/stone-game-vii/) 1951
*   [1406. Stone Game Iii](https://leetcode.com/problems/stone-game-iii/) 2027
*   [1140. Stone Game Ii](https://leetcode.com/problems/stone-game-ii/) 2035
*   [1563. Stone Game V](https://leetcode.com/problems/stone-game-v/) 2087
*   [464. Can I Win](https://leetcode.com/problems/can-i-win/)
*   [1872. Stone Game Viii](https://leetcode.com/problems/stone-game-viii/) 2440
*   [913. Cat and Mouse](https://leetcode.com/problems/cat-and-mouse/) 2800
*   [1728. Cat and Mouse Ii](https://leetcode.com/problems/cat-and-mouse-ii/) 2849
*   [294. Flip Game Ii](https://leetcode.com/problems/flip-game-ii/) (Premium)

-----------

*   [688. Knight Probability in Chessboard](https://leetcode.com/problems/knight-probability-in-chessboard/)
*   [837. New 21 Game](https://leetcode.com/problems/new-21-game/) 2350
*   [1467. Probability of a Two Boxes Having the Same Number of Distinct Balls](https://leetcode.com/problems/probability-of-a-two-boxes-having-the-same-number-of-distinct-balls/) 2357
*   [808. Soup Servings](https://leetcode.com/problems/soup-servings/) 2397
*   [LCR 185. Nge Tou Zi De Dian Shu Lcof](https://leetcode.com/problems/nge-tou-zi-de-dian-shu-lcof/)
*   [Ubiquant-04. Chip Game](https://leetcode.com/contest/ubiquant2022/problems/I3Gm2h/)
*   [1230. Toss Strange Coins](https://leetcode.com/problems/toss-strange-coins/) (Premium)

---------------

*   [368. Largest Divisible Subset](https://leetcode.com/problems/largest-divisible-subset/)
*   [1363. Largest Multiple of Three](https://leetcode.com/problems/largest-multiple-of-three/) 1823
*   [1449. Form Largest Integer with Digits that Add Up to Target](https://leetcode.com/problems/form-largest-integer-with-digits-that-add-up-to-target/) 1927
*   [1092. Shortest Common Supersequence](https://leetcode.com/problems/shortest-common-supersequence/) 1977
*   [943. Find the Shortest Superstring](https://leetcode.com/problems/find-the-shortest-superstring/) 2186
*   [1125. Smallest Sufficient Team](https://leetcode.com/problems/smallest-sufficient-team/) 2251
*   [3533. Concatenated Divisibility](https://leetcode.com/problems/concatenated-divisibility/) 2257
*   [3260. Find the Largest Palindrome Divisible by K](https://leetcode.com/problems/find-the-largest-palindrome-divisible-by-k/) 2370
*   [3149. Find the Minimum Cost Array Permutation](https://leetcode.com/problems/find-the-minimum-cost-array-permutation/) 2642
*   [3441. Minimum Cost Good Caption](https://leetcode.com/problems/minimum-cost-good-caption/) 2765
*   [3348. Smallest Divisible Digit Product Ii](https://leetcode.com/problems/smallest-divisible-digit-product-ii/) 3101
*   [656. Coin Path](https://leetcode.com/problems/coin-path/) (Premium)
*   [471. Encode String with Shortest Length](https://leetcode.com/problems/encode-string-with-shortest-length/) (Premium)

*   [724. Find Pivot Index](https://leetcode.com/problems/find-pivot-index/)
*   [1991. Find the Middle Index in Array](https://leetcode.com/problems/find-the-middle-index-in-array/)
*   [3707. Equal Score Substrings](https://leetcode.com/problems/equal-score-substrings/) 1262
*   [2270. Number of Ways to Split Array](https://leetcode.com/problems/number-of-ways-to-split-array/) 1334
*   [2256. Minimum Average Difference](https://leetcode.com/problems/minimum-average-difference/) 1395
*   [1422. Maximum Score after Splitting a String](https://leetcode.com/problems/maximum-score-after-splitting-a-string/)
*   [238. Product of Array Except Self](https://leetcode.com/problems/product-of-array-except-self/)
*   [1493. Longest Subarray of 1s after Deleting One Element](https://leetcode.com/problems/longest-subarray-of-1s-after-deleting-one-element/) 1423
*   [845. Longest Mountain in Array](https://leetcode.com/problems/longest-mountain-in-array/) 1437
*   [2012. Sum of Beauty in the Array](https://leetcode.com/problems/sum-of-beauty-in-the-array/) 1468
*   [2909. Minimum Sum of Mountain Triplets Ii](https://leetcode.com/problems/minimum-sum-of-mountain-triplets-ii/) 1479
*   [2483. Minimum Penalty for a Shop](https://leetcode.com/problems/minimum-penalty-for-a-shop/) 1495
*   [1525. Number of Good Ways to Split a String](https://leetcode.com/problems/number-of-good-ways-to-split-a-string/) 1500
*   [3583. Count Special Triplets](https://leetcode.com/problems/count-special-triplets/) 1510
*   [3354. Make Array Elements Equal to Zero](https://leetcode.com/problems/make-array-elements-equal-to-zero/)
*   [1930. Unique Length 3 Palindromic Subsequences](https://leetcode.com/problems/unique-length-3-palindromic-subsequences/) 1533
*   [2874. Maximum Value of an Ordered Triplet Ii](https://leetcode.com/problems/maximum-value-of-an-ordered-triplet-ii/) 1583
*   [1664. Ways to Make a Fair Array](https://leetcode.com/problems/ways-to-make-a-fair-array/) 1590
*   [123. Best Time to Buy and Sell Stock Iii](https://leetcode.com/problems/best-time-to-buy-and-sell-stock-iii/) 121
*   [3698. Split Array with Minimum Difference](https://leetcode.com/problems/split-array-with-minimum-difference/) 1649
*   [3598. Longest Common Prefix Between Adjacent Strings after Removals](https://leetcode.com/problems/longest-common-prefix-between-adjacent-strings-after-removals/) 1655
*   [2222. Number of Ways to Select Buildings](https://leetcode.com/problems/number-of-ways-to-select-buildings/) 1657
*   [1031. Maximum Sum of Two Non Overlapping Subarrays](https://leetcode.com/problems/maximum-sum-of-two-non-overlapping-subarrays/) 1680
*   [689. Maximum Sum of 3 Non Overlapping Subarrays](https://leetcode.com/problems/maximum-sum-of-3-non-overlapping-subarrays/)
*   [2420. Find All Good Indices](https://leetcode.com/problems/find-all-good-indices/) 1695
*   [2100. Find Good Days to Rob the Bank](https://leetcode.com/problems/find-good-days-to-rob-the-bank/) 1702
*   [926. Flip String to Monotone Increasing](https://leetcode.com/problems/flip-string-to-monotone-increasing/)
*   [334. Increasing Triplet Subsequence](https://leetcode.com/problems/increasing-triplet-subsequence/)
*   [1653. Minimum Deletions to Make String Balanced](https://leetcode.com/problems/minimum-deletions-to-make-string-balanced/) 1794
*   [1186. Maximum Subarray Sum with One Deletion](https://leetcode.com/problems/maximum-subarray-sum-with-one-deletion/) 1799
*   [3738. Longest Non Decreasing Subarray after Replacing at Most One Element](https://leetcode.com/problems/longest-non-decreasing-subarray-after-replacing-at-most-one-element/) 1811
*   [42. Trapping Rain Water](https://leetcode.com/problems/trapping-rain-water/) [](/link/?target=https%3A%2F%2Fwww.bilibili.com%2Fvideo%2FBV1Qg411q7ia%2F%3Ft%3D3m05s)
*   [2711. Difference of Number of Distinct Values on Diagonals](https://leetcode.com/problems/difference-of-number-of-distinct-values-on-diagonals/)
*   [1477. Find Two Non Overlapping Sub Arrays Each with Target Sum](https://leetcode.com/problems/find-two-non-overlapping-sub-arrays-each-with-target-sum/) 1851
*   [2680. Maximum or](https://leetcode.com/problems/maximum-or/) 1912
*   [1671. Minimum Number of Removals to Make Mountain Array](https://leetcode.com/problems/minimum-number-of-removals-to-make-mountain-array/) 1913
*   [2906. Construct Product Matrix](https://leetcode.com/problems/construct-product-matrix/) 2075
*   [3334. Find the Maximum Factor Score of Array](https://leetcode.com/problems/find-the-maximum-factor-score-of-array/)
*   [2167. Minimum Time to Remove All Cars Containing Illegal Goods](https://leetcode.com/problems/minimum-time-to-remove-all-cars-containing-illegal-goods/) 2219
*   [2484. Count Palindromic Subsequences](https://leetcode.com/problems/count-palindromic-subsequences/) 2223
*   [2163. Minimum Difference in Sums after Removal of Elements](https://leetcode.com/problems/minimum-difference-in-sums-after-removal-of-elements/) 2225
*   [2565. Subsequence with the Minimum Score](https://leetcode.com/problems/subsequence-with-the-minimum-score/) 2432
*   [1995. Count Special Quadruplets](https://leetcode.com/problems/count-special-quadruplets/)
*   [2552. Count Increasing Quadruplets](https://leetcode.com/problems/count-increasing-quadruplets/) 2433
*   [3302. Find the Lexicographically Smallest Valid Sequence](https://leetcode.com/problems/find-the-lexicographically-smallest-valid-sequence/) 2474  2565
*   [3404. Count Special Subsequences](https://leetcode.com/problems/count-special-subsequences/) 2445
*   [3303. Find the Occurrence of First Almost Equal Substring](https://leetcode.com/problems/find-the-occurrence-of-first-almost-equal-substring/) 2509
*   [3287. Find the Maximum Sequence Value of Array](https://leetcode.com/problems/find-the-maximum-sequence-value-of-array/) 2545
*   [3257. Maximum Value Sum by Placing Three Rooks Ii](https://leetcode.com/problems/maximum-value-sum-by-placing-three-rooks-ii/) 2553
*   [3410. Maximize Subarray Sum after Removing All Occurrences of One Element](https://leetcode.com/problems/maximize-subarray-sum-after-removing-all-occurrences-of-one-element/) 2844
*   [3003. Maximize the Number of Partitions after Operations](https://leetcode.com/problems/maximize-the-number-of-partitions-after-operations/) 3039
*   [487. Max Consecutive Ones Ii](https://leetcode.com/problems/max-consecutive-ones-ii/) (Premium)
*   [1746. Maximum Subarray Sum after One Operation](https://leetcode.com/problems/maximum-subarray-sum-after-one-operation/) (Premium)


-----------

*   [397. Integer Replacement](https://leetcode.com/problems/integer-replacement/)
*   [2998. Minimum Number of Operations to Make X and Y Equal](https://leetcode.com/problems/minimum-number-of-operations-to-make-x-and-y-equal/) 1795
*   [2059. Minimum Operations to Convert Number](https://leetcode.com/problems/minimum-operations-to-convert-number/) 1850
*   [991. Broken Calculator](https://leetcode.com/problems/broken-calculator/) 1909
*   [1553. Minimum Number of Days to Eat N Oranges](https://leetcode.com/problems/minimum-number-of-days-to-eat-n-oranges/) 2048

*   [3377. Digit Operations to Make Two Integers Equal](https://leetcode.com/problems/digit-operations-to-make-two-integers-equal/) 2186

-------

*   [1306. Jump Game Iii](https://leetcode.com/problems/jump-game-iii/) 1397
*   [2770. Maximum Number of Jumps to Reach the Last Index](https://leetcode.com/problems/maximum-number-of-jumps-to-reach-the-last-index/) 1533
*   [403. Frog Jump](https://leetcode.com/problems/frog-jump/)
*   [1340. Jump Game V](https://leetcode.com/problems/jump-game-v/) 1866
*   [1871. Jump Game Vii](https://leetcode.com/problems/jump-game-vii/) 1896
*   [1696. Jump Game Vi](https://leetcode.com/problems/jump-game-vi/) 1954
*   [975. Odd Even Jump](https://leetcode.com/problems/odd-even-jump/) 2079
*   [1654. Minimum Jumps to Reach Home](https://leetcode.com/problems/minimum-jumps-to-reach-home/) 2124
*   [LCP 09. Zui Xiao Tiao Yue Ci Shu](https://leetcode.com/problems/zui-xiao-tiao-yue-ci-shu/)
*   [LCP 20. Mechtz](https://leetcode.com/problems/meChtZ/)
*   [656. Coin Path](https://leetcode.com/problems/coin-path/) (Premium)
*   [2297. Jump Game Viii](https://leetcode.com/problems/jump-game-viii/) (Premium)

Others

*   [1387. Sort Integers by the Power Value](https://leetcode.com/problems/sort-integers-by-the-power-value/) 1507
*   [823. Binary Trees with Factors](https://leetcode.com/problems/binary-trees-with-factors/) 1900
*   [756. Pyramid Transition Matrix](https://leetcode.com/problems/pyramid-transition-matrix/) 1990
*   [2930. Number of Strings Which Can Be Rearranged to Contain Substring](https://leetcode.com/problems/number-of-strings-which-can-be-rearranged-to-contain-substring/) 2227
*   [1896. Minimum Cost to Change the Final Value of Expression](https://leetcode.com/problems/minimum-cost-to-change-the-final-value-of-expression/) 2532


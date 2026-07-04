# Common Data Structures

Problem list from [0x3F's LeetCode Study Plan](https://leetcode.cn/circle/discuss/mOr1u6/) — Common Data Structures (Prefix Sums/Difference Arrays/Stack/Queue/Heap/Trie/Union-Find/Fenwick Tree/Segment Tree).

## 0. Common Enumeration Techniques

### §0.1 Enumerate Right, Maintain Left

For **two-variable problems** — e.g. two-sum a_i + a_j = t — you can enumerate the right element a_j and reduce it to a **single-variable problem**: check whether there is an a_i = t − a_j to the left of a_j. This can be maintained with a hash table.

This technique is called **enumerate right, maintain left**.

For the problems below, implement them with **a single pass** whenever possible.

#### §0.1.1 Basics

- [1. Two Sum](https://leetcode.com/problems/two-sum/)
- [1512. Number Of Good Pairs](https://leetcode.com/problems/number-of-good-pairs/) 1161 (equivalent to two numbers with a difference of 0)
- [2441. Largest Positive Integer That Exists With Its Negative](https://leetcode.com/problems/largest-positive-integer-that-exists-with-its-negative/) 1168 (equivalent to two numbers summing to 0)
- [121. Best Time To Buy And Sell Stock](https://leetcode.com/problems/best-time-to-buy-and-sell-stock/)
- [2016. Maximum Difference Between Increasing Elements](https://leetcode.com/problems/maximum-difference-between-increasing-elements/) 1246
- [624. Maximum Distance In Arrays](https://leetcode.com/problems/maximum-distance-in-arrays/)
- [3880. Minimum Absolute Difference Between Two Values](https://leetcode.com/problems/minimum-absolute-difference-between-two-values/) 1257
- [2342. Max Sum Of A Pair With Equal Sum Of Digits](https://leetcode.com/problems/max-sum-of-a-pair-with-equal-sum-of-digits/) 1309
- [1128. Number Of Equivalent Domino Pairs](https://leetcode.com/problems/number-of-equivalent-domino-pairs/) 1333
- [1679. Max Number Of K-Sum Pairs](https://leetcode.com/problems/max-number-of-k-sum-pairs/) 1346
- [Interview 16.24. Pair Sums](https://leetcode.com/problems/pairs-with-sum-lcci/)
- [219. Contains Duplicate II](https://leetcode.com/problems/contains-duplicate-ii/)
- [2260. Minimum Consecutive Cards To Pick Up](https://leetcode.com/problems/minimum-consecutive-cards-to-pick-up/) 1365
- [2001. Number Of Pairs Of Interchangeable Rectangles](https://leetcode.com/problems/number-of-pairs-of-interchangeable-rectangles/) 1436
- [2815. Max Pair Sum In An Array](https://leetcode.com/problems/max-pair-sum-in-an-array/) (non-brute-force)
- [3623. Count Number Of Trapezoids I](https://leetcode.com/problems/count-number-of-trapezoids-i/) 1580
- [2364. Count Number Of Bad Pairs](https://leetcode.com/problems/count-number-of-bad-pairs/) 1622
- [3805. Count Caesar Cipher Pairs](https://leetcode.com/problems/count-caesar-cipher-pairs/) 1624
- [3371. Identify The Largest Outlier In An Array](https://leetcode.com/problems/identify-the-largest-outlier-in-an-array/) 1644
- [3761. Minimum Absolute Distance Between Mirror Pairs](https://leetcode.com/problems/minimum-absolute-distance-between-mirror-pairs/) 1669
- [1014. Best Sightseeing Pair](https://leetcode.com/problems/best-sightseeing-pair/) 1730
- [1814. Count Nice Pairs In An Array](https://leetcode.com/problems/count-nice-pairs-in-an-array/) 1738
- [3584. Maximum Product Of First And Last Elements Of A Subsequence](https://leetcode.com/problems/maximum-product-of-first-and-last-elements-of-a-subsequence/) 1763
- [2905. Find Indices With Index And Value Difference II](https://leetcode.com/problems/find-indices-with-index-and-value-difference-ii/) 1764 (thinking question: count the number of index pairs)
- [3837. Delayed Count Of Equal Elements](https://leetcode.com/problems/delayed-count-of-equal-elements/) 🔒
- [3907. Count Smaller Elements With Opposite Parity](https://leetcode.com/problems/count-smaller-elements-with-opposite-parity/) 🔒

#### §0.1.2 Advanced

- [1010. Pairs Of Songs With Total Durations Divisible By 60](https://leetcode.com/problems/pairs-of-songs-with-total-durations-divisible-by-60/)
- [3185. Count Pairs That Form A Complete Day II](https://leetcode.com/problems/count-pairs-that-form-a-complete-day-ii/) (same as 1010)
- [2748. Number Of Beautiful Pairs](https://leetcode.com/problems/number-of-beautiful-pairs/)
- [2506. Count Pairs Of Similar Strings](https://leetcode.com/problems/count-pairs-of-similar-strings/)
- [2874. Maximum Value Of An Ordered Triplet II](https://leetcode.com/problems/maximum-value-of-an-ordered-triplet-ii/) 1583
- [1497. Check If Array Pairs Are Divisible By K](https://leetcode.com/problems/check-if-array-pairs-are-divisible-by-k/) 1787
- [1031. Maximum Sum Of Two Non Overlapping Subarrays](https://leetcode.com/problems/maximum-sum-of-two-non-overlapping-subarrays/) ~2000
- [2555. Maximize Win From Two Segments](https://leetcode.com/problems/maximize-win-from-two-segments/) 2081
- [1995. Count Special Quadruplets](https://leetcode.com/problems/count-special-quadruplets/) (four numbers)
- [3404. Count Special Subsequences](https://leetcode.com/problems/count-special-subsequences/) 2445 (four numbers)
- [3267. Count Almost Equal Pairs II](https://leetcode.com/problems/count-almost-equal-pairs-ii/) 2545
- [3480. Maximize Subarrays After Removing One Conflicting Pair](https://leetcode.com/problems/maximize-subarrays-after-removing-one-conflicting-pair/) 2764
- [1214. Two Sum BSTs](https://leetcode.com/problems/two-sum-bsts/) 🔒
- [2964. Number Of Divisible Triplet Sums](https://leetcode.com/problems/number-of-divisible-triplet-sums/) 🔒

**Mind Extensions**:

- [3917. Count Indices With Opposite Parity](https://leetcode.com/problems/count-indices-with-opposite-parity/) (achieve O(n))
- [2078. Two Furthest Houses With Different Colors](https://leetcode.com/problems/two-furthest-houses-with-different-colors/) (achieve O(n))
- [454. 4Sum II](https://leetcode.com/problems/4sum-ii/)
- [220. Contains Duplicate III](https://leetcode.com/problems/contains-duplicate-iii/)
- [3027. Find The Number Of Ways To Place People II](https://leetcode.com/problems/find-the-number-of-ways-to-place-people-ii/) 2020
- [3548. Equal Sum Grid Partition II](https://leetcode.com/problems/equal-sum-grid-partition-ii/) 2245 (code reuse)
- [3713. Longest Balanced Substring I](https://leetcode.com/problems/longest-balanced-substring-i/) (non-brute-force)

### §0.2 Enumerate the Middle

For problems with three or four variables, enumerating the middle variable is often easier to compute.

Why? Suppose a problem has three indices that must satisfy 0 ≤ i < j < k < n. Compare:

- Enumerate i: the remaining computation still needs j < k.
- Enumerate j: then i and k are automatically separated by j and become independent, so the remaining computation doesn't need to worry about the relative order of i and k.

So enumerating the middle variable is simpler.

- [2909. Minimum Sum Of Mountain Triplets II](https://leetcode.com/problems/minimum-sum-of-mountain-triplets-ii/) 1479
- [3583. Count Special Triplets](https://leetcode.com/problems/count-special-triplets/) 1510 (can also be solved with one pass)
- [1930. Unique Length 3 Palindromic Subsequences](https://leetcode.com/problems/unique-length-3-palindromic-subsequences/) 1533
- [3128. Right Triangles](https://leetcode.com/problems/right-triangles/) 1541
- [2874. Maximum Value Of An Ordered Triplet II](https://leetcode.com/problems/maximum-value-of-an-ordered-triplet-ii/) 1583 (can also be solved with one pass)
- [447. Number Of Boomerangs](https://leetcode.com/problems/number-of-boomerangs/)
- [456. 132 Pattern](https://leetcode.com/problems/132-pattern/)
- [3067. Count Pairs Of Connectable Servers In A Weighted Tree Network](https://leetcode.com/problems/count-pairs-of-connectable-servers-in-a-weighted-tree-network/) 1909
- [1534. Count Good Triplets](https://leetcode.com/problems/count-good-triplets/) (achieve O(n^2))
- [3455. Shortest Matching Substring](https://leetcode.com/problems/shortest-matching-substring/) 2303
- [2242. Maximum Score Of A Node Sequence](https://leetcode.com/problems/maximum-score-of-a-node-sequence/) 2304
- [2867. Count Valid Paths In A Tree](https://leetcode.com/problems/count-valid-paths-in-a-tree/) 2428
- [2552. Count Increasing Quadruplets](https://leetcode.com/problems/count-increasing-quadruplets/) 2433 (more than one approach)
- [3257. Maximum Value Sum By Placing Three Rooks II](https://leetcode.com/problems/maximum-value-sum-by-placing-three-rooks-ii/) 2553
- [3073. Maximum Increasing Triplet Value](https://leetcode.com/problems/maximum-increasing-triplet-value/) 🔒

### §0.3 Traverse Diagonals

- [3446. Sort Matrix By Diagonals](https://leetcode.com/problems/sort-matrix-by-diagonals/) 1373
- [2711. Difference Of Number Of Distinct Values On Diagonals](https://leetcode.com/problems/difference-of-number-of-distinct-values-on-diagonals/) 1429
- [1329. Sort The Matrix Diagonally](https://leetcode.com/problems/sort-the-matrix-diagonally/) 1548
- [498. Diagonal Traverse](https://leetcode.com/problems/diagonal-traverse/)
- [Interview 17.23. Max Black Square](https://leetcode.com/problems/max-black-square-lcci/) (achieve O(n^2 log n); difficulty around 2800)
- [562. Longest Line Of Consecutive One In Matrix](https://leetcode.com/problems/longest-line-of-consecutive-one-in-matrix/) 🔒

**Mind Extensions**:

- [1424. Diagonal Traverse II](https://leetcode.com/problems/diagonal-traverse-ii/) 1780

### §0.4 Prefix/Suffix Decomposition

See **Topic: Prefix/Suffix Decomposition** in [07_dynamic_programming.md](07_dynamic_programming.md).

## I. Prefix Sums

### §1.1 Basics

**Left-closed, right-open formula**: the sum of subarray [left, right) equals sum[right] − sum[left]. Defining index ranges as left-closed, right-open avoids +1/−1 off-by-one adjustments.

- [303. Range Sum Query - Immutable](https://leetcode.com/problems/range-sum-query-immutable/) (template problem)
- [3427. Sum Of Variable Length Subarrays](https://leetcode.com/problems/sum-of-variable-length-subarrays/) (achieve O(n))
- [2559. Count Vowel Strings In Ranges](https://leetcode.com/problems/count-vowel-strings-in-ranges/) 1435
- [1310. XOR Queries Of A Subarray](https://leetcode.com/problems/xor-queries-of-a-subarray/) 1460
- [3152. Special Array II](https://leetcode.com/problems/special-array-ii/) 1523
- [1749. Maximum Absolute Sum Of Any Subarray](https://leetcode.com/problems/maximum-absolute-sum-of-any-subarray/) 1542
- [53. Maximum Subarray](https://leetcode.com/problems/maximum-subarray/)
- [3652. Best Time To Buy And Sell Stock Using Strategy](https://leetcode.com/problems/best-time-to-buy-and-sell-stock-using-strategy/) 1557
- [3361. Shift Distance Between Two Strings](https://leetcode.com/problems/shift-distance-between-two-strings/)
- [3511. Make A Positive Array](https://leetcode.com/problems/make-a-positive-array/) 🔒
- [3540. Minimum Time To Visit All Houses](https://leetcode.com/problems/minimum-time-to-visit-all-houses/) 🔒

**Mind Extensions**:

- [1523. Count Odd Numbers In An Interval Range](https://leetcode.com/problems/count-odd-numbers-in-an-interval-range/) 1209
- [848. Shifting Letters](https://leetcode.com/problems/shifting-letters/) 1353

### §1.2 Prefix Sums and Hash Tables

This usually requires the **enumerate right, maintain left** technique (see §0.1 in this list).

- [560. Subarray Sum Equals K](https://leetcode.com/problems/subarray-sum-equals-k/) (my solution includes a variant problem)
- [930. Binary Subarrays With Sum](https://leetcode.com/problems/binary-subarrays-with-sum/) 1592 (same as 560)
- [1524. Number Of Sub Arrays With Odd Sum](https://leetcode.com/problems/number-of-sub-arrays-with-odd-sum/) 1611
- [974. Subarray Sums Divisible By K](https://leetcode.com/problems/subarray-sums-divisible-by-k/) 1676
- [523. Continuous Subarray Sum](https://leetcode.com/problems/continuous-subarray-sum/) (similar to 974)
- [2588. Count The Number Of Beautiful Subarrays](https://leetcode.com/problems/count-the-number-of-beautiful-subarrays/) 1697
- [525. Contiguous Array](https://leetcode.com/problems/contiguous-array/) (longest subarray with an equal number of 0s and 1s)
- [Interview 17.05. Find Longest Subarray](https://leetcode.com/problems/find-longest-subarray-lcci/) (same as 525)
- [3755. Find Maximum Balanced XOR Subarray Length](https://leetcode.com/problems/find-maximum-balanced-xor-subarray-length/) (pair)
- [3026. Maximum Good Subarray Sum](https://leetcode.com/problems/maximum-good-subarray-sum/) 1817
- [1477. Find Two Non Overlapping Sub Arrays Each With Target Sum](https://leetcode.com/problems/find-two-non-overlapping-sub-arrays-each-with-target-sum/) 1851
- [1546. Maximum Number Of Non Overlapping Subarrays With Sum Equals Target](https://leetcode.com/problems/maximum-number-of-non-overlapping-subarrays-with-sum-equals-target/) 1855
- [1124. Longest Well Performing Interval](https://leetcode.com/problems/longest-well-performing-interval/) 1908
- [3728. Stable Subarrays With Equal Boundary And Interior Sum](https://leetcode.com/problems/stable-subarrays-with-equal-boundary-and-interior-sum/) 1909 (pair; length has a lower bound)
- [3381. Maximum Subarray Sum With Length Divisible By K](https://leetcode.com/problems/maximum-subarray-sum-with-length-divisible-by-k/) 1943
- [2488. Count Subarrays With Median K](https://leetcode.com/problems/count-subarrays-with-median-k/) 1999
- [1590. Make Sum Divisible By P](https://leetcode.com/problems/make-sum-divisible-by-p/) 2039
- [2845. Count Of Interesting Subarrays](https://leetcode.com/problems/count-of-interesting-subarrays/) 2073
- [3739. Count Subarrays With Majority Element II](https://leetcode.com/problems/count-subarrays-with-majority-element-ii/) 2090
- [3900. Longest Balanced Substring After One Swap](https://leetcode.com/problems/longest-balanced-substring-after-one-swap/) 2135
- [1074. Number Of Submatrices That Sum To Target](https://leetcode.com/problems/number-of-submatrices-that-sum-to-target/) 2189 (2D version of 560)
- [1442. Count Triplets That Can Form Two Arrays Of Equal XOR](https://leetcode.com/problems/count-triplets-that-can-form-two-arrays-of-equal-xor/) (achieve O(n))
- [3714. Longest Balanced Substring II](https://leetcode.com/problems/longest-balanced-substring-ii/) 2202 (pair)
- [2025. Maximum Number Of Ways To Partition An Array](https://leetcode.com/problems/maximum-number-of-ways-to-partition-an-array/) 2218
- [3729. Count Distinct Subarrays Divisible By K In Sorted Array](https://leetcode.com/problems/count-distinct-subarrays-divisible-by-k-in-sorted-array/) 2248 (deduplicate subarrays / avoid double counting)
- [3969. Valid Subarrays With Matching Sum Digits I](https://leetcode.com/problems/valid-subarrays-with-matching-sum-digits-i/) (non-brute-force)
- [2949. Count Beautiful Substrings II](https://leetcode.com/problems/count-beautiful-substrings-ii/) 2445 (pair)
- [325. Maximum Size Subarray Sum Equals K](https://leetcode.com/problems/maximum-size-subarray-sum-equals-k/) 🔒
- [548. Split Array With Equal Sum](https://leetcode.com/problems/split-array-with-equal-sum/) 🔒
- [1983. Widest Pair Of Indices With Equal Range Sum](https://leetcode.com/problems/widest-pair-of-indices-with-equal-range-sum/) 🔒
- [2489. Number Of Substrings With Fixed Ratio](https://leetcode.com/problems/number-of-substrings-with-fixed-ratio/) 🔒
- [2031. Count Subarrays With More Ones Than Zeros](https://leetcode.com/problems/count-subarrays-with-more-ones-than-zeros/) 🔒 (achieve O(n))
- [2950. Number Of Divisible Substrings](https://leetcode.com/problems/number-of-divisible-substrings/) 🔒 (achieve O(kn), where k = 9)

**Prefix Sums with an Ordered Set**:

- [3364. Minimum Positive Sum Subarray](https://leetcode.com/problems/minimum-positive-sum-subarray/) (non-brute-force)
- [363. Max Sum Of Rectangle No Larger Than K](https://leetcode.com/problems/max-sum-of-rectangle-no-larger-than-k/)
- [3739. Count Subarrays With Majority Element II](https://leetcode.com/problems/count-subarrays-with-majority-element-ii/) 2090
- [2031. Count Subarrays With More Ones Than Zeros](https://leetcode.com/problems/count-subarrays-with-more-ones-than-zeros/) 🔒 (has an O(n) approach)

**Mind Extensions**:

- [437. Path Sum III](https://leetcode.com/problems/path-sum-iii/)

### §1.3 Sum of Distances

- [1685. Sum Of Absolute Differences In A Sorted Array](https://leetcode.com/problems/sum-of-absolute-differences-in-a-sorted-array/) 1496
- [2615. Sum Of Distances](https://leetcode.com/problems/sum-of-distances/) 1793
- [2602. Minimum Operations To Make All Array Elements Equal](https://leetcode.com/problems/minimum-operations-to-make-all-array-elements-equal/) 1903
- [3937. Minimum Operations To Make Array Modulo Alternating I](https://leetcode.com/problems/minimum-operations-to-make-array-modulo-alternating-i/) (achieve O(n log n))
- [2968. Apply Operations To Maximize Frequency Score](https://leetcode.com/problems/apply-operations-to-maximize-frequency-score/) 2444
- [1703. Minimum Adjacent Swaps For K-Consecutive Ones](https://leetcode.com/problems/minimum-adjacent-swaps-for-k-consecutive-ones/) 2467
- [3086. Minimum Moves To Pick K-Ones](https://leetcode.com/problems/minimum-moves-to-pick-k-ones/) 2673
- [3422. Minimum Operations To Make Subarray Elements Equal](https://leetcode.com/problems/minimum-operations-to-make-subarray-elements-equal/) 🔒

### §1.4 Bitmask Prefix Sums

Recommended reading first: a classification summary of common bit-manipulation tricks, from set theory to bitwise operations.

- [1177. Can Make Palindrome From Substring](https://leetcode.com/problems/can-make-palindrome-from-substring/) 1848
- [1371. Find The Longest Substring Containing Vowels In Even Counts](https://leetcode.com/problems/find-the-longest-substring-containing-vowels-in-even-counts/) 2041
- [1542. Find Longest Awesome Substring](https://leetcode.com/problems/find-longest-awesome-substring/) 2222
- [1915. Number Of Wonderful Substrings](https://leetcode.com/problems/number-of-wonderful-substrings/) 2235
- [2791. Count Paths That Can Form A Palindrome In A Tree](https://leetcode.com/problems/count-paths-that-can-form-a-palindrome-in-a-tree/) 2677

### §1.5 Advanced

- [2389. Longest Subsequence With Limited Sum](https://leetcode.com/problems/longest-subsequence-with-limited-sum/) (non-brute-force)
- [3709. Design Exam Scores Tracker](https://leetcode.com/problems/design-exam-scores-tracker/) 1648
- [3919. Minimum Cost To Move Between Indices](https://leetcode.com/problems/minimum-cost-to-move-between-indices/) 1777
- [1895. Largest Magic Square](https://leetcode.com/problems/largest-magic-square/) 1781 (diagonal prefix sums; can be optimized to O(N^3))
- [2055. Plates Between Candles](https://leetcode.com/problems/plates-between-candles/) 1819
- [1744. Can You Eat Your Favorite Candy On Your Favorite Day](https://leetcode.com/problems/can-you-eat-your-favorite-candy-on-your-favorite-day/) 1859
- [1878. Get Biggest Three Rhombus Sums In A Grid](https://leetcode.com/problems/get-biggest-three-rhombus-sums-in-a-grid/) 1898 (diagonal prefix sums)
- [3756. Concatenate Non Zero Digits And Multiply By Sum II](https://leetcode.com/problems/concatenate-non-zero-digits-and-multiply-by-sum-ii/) 1968
- [1031. Maximum Sum Of Two Non Overlapping Subarrays](https://leetcode.com/problems/maximum-sum-of-two-non-overlapping-subarrays/) (achieve O(n))
- [2245. Maximum Trailing Zeros In A Cornered Path](https://leetcode.com/problems/maximum-trailing-zeros-in-a-cornered-path/) 2037
- [1712. Ways To Split Array Into Three Subarrays](https://leetcode.com/problems/ways-to-split-array-into-three-subarrays/) 2079
- [1862. Sum Of Floored Pairs](https://leetcode.com/problems/sum-of-floored-pairs/) 2170
- [3748. Count Stable Subarrays](https://leetcode.com/problems/count-stable-subarrays/) 2209 (includes an advanced follow-up)
- [2281. Sum Of Total Strength Of Wizards](https://leetcode.com/problems/sum-of-total-strength-of-wizards/) 2621
- [3445. Maximum Difference Between Even And Odd Frequency II](https://leetcode.com/problems/maximum-difference-between-even-and-odd-frequency-ii/) 2694
- [2983. Palindrome Rearrangement Queries](https://leetcode.com/problems/palindrome-rearrangement-queries/) 2780
- [2955. Number Of Same End Substrings](https://leetcode.com/problems/number-of-same-end-substrings/) 🔒
- [1788. Maximize The Beauty Of The Garden](https://leetcode.com/problems/maximize-the-beauty-of-the-garden/) 🔒
- [2819. Minimum Relative Loss After Buying Chocolates](https://leetcode.com/problems/minimum-relative-loss-after-buying-chocolates/) 🔒

**Mind Extensions**:

- [2300. Successful Pairs Of Spells And Potions](https://leetcode.com/problems/successful-pairs-of-spells-and-potions/)
- [1534. Count Good Triplets](https://leetcode.com/problems/count-good-triplets/)

### §1.6 2D Prefix Sums

- [304. Range Sum Query 2D - Immutable](https://leetcode.com/problems/range-sum-query-2d-immutable/)
- [1314. Matrix Block Sum](https://leetcode.com/problems/matrix-block-sum/) 1484
- [3070. Count Submatrices With Top Left Element And Sum Less Than K](https://leetcode.com/problems/count-submatrices-with-top-left-element-and-sum-less-than-k/) 1499
- [1738. Find Kth Largest XOR Coordinate Value](https://leetcode.com/problems/find-kth-largest-xor-coordinate-value/) 1671
- [3212. Count Submatrices With Equal Frequency Of X And Y](https://leetcode.com/problems/count-submatrices-with-equal-frequency-of-x-and-y/) 1673
- [1292. Maximum Side Length Of A Square With Sum Less Than Or Equal To Threshold](https://leetcode.com/problems/maximum-side-length-of-a-square-with-sum-less-than-or-equal-to-threshold/) 1735 (can be optimized to O(mn))

**2D Prefix Minimum**:

- [3148. Maximum Difference Score In A Grid](https://leetcode.com/problems/maximum-difference-score-in-a-grid/) 1820

## II. Difference Arrays

### §2.1 1D Difference Arrays

The relationship between a difference array and a prefix sum is like the relationship between a **derivative** and an **integral**.

The prefix sum of the difference array of array a is array a itself (unchanged).

#### §2.1.1 Basics

- [2848. Points That Intersect With Cars](https://leetcode.com/problems/points-that-intersect-with-cars/) 1230
- [1893. Check If All The Integers In A Range Are Covered](https://leetcode.com/problems/check-if-all-the-integers-in-a-range-are-covered/) 1307
- [1854. Maximum Population Year](https://leetcode.com/problems/maximum-population-year/) 1370
- [Interview 16.10. Living People](https://leetcode.com/problems/living-people-lcci/) (same as 1854)
- [2960. Count Tested Devices After Test Operations](https://leetcode.com/problems/count-tested-devices-after-test-operations/) (difference array idea)
- [1094. Car Pooling](https://leetcode.com/problems/car-pooling/) 1441
- [1109. Corporate Flight Bookings](https://leetcode.com/problems/corporate-flight-bookings/) 1570
- [3964. Minimum Lights To Illuminate A Road](https://leetcode.com/problems/minimum-lights-to-illuminate-a-road/) 1572
- [3355. Zero Array Transformation I](https://leetcode.com/problems/zero-array-transformation-i/) 1591
- [370. Range Addition](https://leetcode.com/problems/range-addition/) 🔒

#### §2.1.2 Advanced

- [3914. Minimum Operations To Make Array Non Decreasing](https://leetcode.com/problems/minimum-operations-to-make-array-non-decreasing/) 1662 (difference array idea)
- [3453. Separate Squares I](https://leetcode.com/problems/separate-squares-i/) 1735
- [2381. Shifting Letters II](https://leetcode.com/problems/shifting-letters-ii/) 1793
- [995. Minimum Number Of K-Consecutive Bit Flips](https://leetcode.com/problems/minimum-number-of-k-consecutive-bit-flips/) 1835
- [1589. Maximum Sum Obtained Of Any Permutation](https://leetcode.com/problems/maximum-sum-obtained-of-any-permutation/) 1871
- [1526. Minimum Number Of Increments On Subarrays To Form A Target Array](https://leetcode.com/problems/minimum-number-of-increments-on-subarrays-to-form-a-target-array/) 1872 (difference array idea)
- [1871. Jump Game VII](https://leetcode.com/problems/jump-game-vii/) 1896 (more than one approach)
- [3356. Zero Array Transformation II](https://leetcode.com/problems/zero-array-transformation-ii/) 1913 (more than one approach)
- [1943. Describe The Painting](https://leetcode.com/problems/describe-the-painting/) 1969
- [3224. Minimum Array Changes To Make Differences Equal](https://leetcode.com/problems/minimum-array-changes-to-make-differences-equal/) 1996 (more than one approach)
- [2327. Number Of People Aware Of A Secret](https://leetcode.com/problems/number-of-people-aware-of-a-secret/) (achieve O(n))
- [2251. Number Of Flowers In Full Bloom](https://leetcode.com/problems/number-of-flowers-in-full-bloom/) 2022
- [2772. Apply Operations To Make All Array Elements Equal To Zero](https://leetcode.com/problems/apply-operations-to-make-all-array-elements-equal-to-zero/) 2029
- [3229. Minimum Operations To Make Array Equal To Target](https://leetcode.com/problems/minimum-operations-to-make-array-equal-to-target/) 2067 (difference array idea)
- [3529. Count Cells In Overlapping Horizontal And Vertical Substrings](https://leetcode.com/problems/count-cells-in-overlapping-horizontal-and-vertical-substrings/) 2105
- [798. Smallest Rotation With Highest Score](https://leetcode.com/problems/smallest-rotation-with-highest-score/) 2130
- [3347. Maximum Frequency Of An Element After Performing Operations II](https://leetcode.com/problems/maximum-frequency-of-an-element-after-performing-operations-ii/) 2156
- [2528. Maximize The Minimum Powered City](https://leetcode.com/problems/maximize-the-minimum-powered-city/) 2236
- [1674. Minimum Moves To Make Array Complementary](https://leetcode.com/problems/minimum-moves-to-make-array-complementary/) 2333
- [3362. Zero Array Transformation III](https://leetcode.com/problems/zero-array-transformation-iii/) 2424
- [3655. XOR After Range Multiplication Queries II](https://leetcode.com/problems/xor-after-range-multiplication-queries-ii/) 2454 (quotient blocking trick)
- [3017. Count The Number Of Houses At A Certain Distance II](https://leetcode.com/problems/count-the-number-of-houses-at-a-certain-distance-ii/) 2709
- [2021. Brightest Position On Street](https://leetcode.com/problems/brightest-position-on-street/) 🔒
- [2015. Average Height Of Buildings In Each Segment](https://leetcode.com/problems/average-height-of-buildings-in-each-segment/) 🔒
- [2237. Count Positions On Street With Required Brightness](https://leetcode.com/problems/count-positions-on-street-with-required-brightness/) 🔒
- [3009. Maximum Number Of Intersections On The Chart](https://leetcode.com/problems/maximum-number-of-intersections-on-the-chart/) 🔒
- [3279. Maximum Total Area Occupied By Pistons](https://leetcode.com/problems/maximum-total-area-occupied-by-pistons/) 🔒

**Mind Extensions**:

- [56. Merge Intervals](https://leetcode.com/problems/merge-intervals/) (see my comment for the approach)
- [57. Insert Interval](https://leetcode.com/problems/insert-interval/)
- [732. My Calendar III](https://leetcode.com/problems/my-calendar-iii/)
- [2406. Divide Intervals Into Minimum Number Of Groups](https://leetcode.com/problems/divide-intervals-into-minimum-number-of-groups/) 1713
- [253. Meeting Rooms II](https://leetcode.com/problems/meeting-rooms-ii/) 🔒
- [759. Employee Free Time](https://leetcode.com/problems/employee-free-time/) 🔒

### §2.2 2D Difference Arrays

- [2536. Increment Submatrices By One](https://leetcode.com/problems/increment-submatrices-by-one/) 1583
- [850. Rectangle Area II](https://leetcode.com/problems/rectangle-area-ii/) 2236 (brute-force approach)
- [2132. Stamping The Grid](https://leetcode.com/problems/stamping-the-grid/) 2364
- [LCP 74. Strongest Blessing Force Field](https://leetcode.cn/problems/xepqZ5/)
- [3888. Minimum Operations To Make All Grid Elements Equal](https://leetcode.com/problems/minimum-operations-to-make-all-grid-elements-equal/) 🔒

## III. Stack

### §3.1 Basics

- [1441. Build An Array With Stack Operations](https://leetcode.com/problems/build-an-array-with-stack-operations/) 1180
- [844. Backspace String Compare](https://leetcode.com/problems/backspace-string-compare/) 1228
- [682. Baseball Game](https://leetcode.com/problems/baseball-game/)
- [2390. Removing Stars From A String](https://leetcode.com/problems/removing-stars-from-a-string/) 1348
- [1472. Design Browser History](https://leetcode.com/problems/design-browser-history/) 1454
- [946. Validate Stack Sequences](https://leetcode.com/problems/validate-stack-sequences/) 1462
- [3412. Find Mirror Score Of A String](https://leetcode.com/problems/find-mirror-score-of-a-string/) 1578
- [71. Simplify Path](https://leetcode.com/problems/simplify-path/)

### §3.2 Advanced

- [3170. Lexicographically Minimum String After Removing Stars](https://leetcode.com/problems/lexicographically-minimum-string-after-removing-stars/) 1772
- [155. Min Stack](https://leetcode.com/problems/min-stack/)
- [1381. Design A Stack With Increment Operation](https://leetcode.com/problems/design-a-stack-with-increment-operation/)
- [636. Exclusive Time Of Functions](https://leetcode.com/problems/exclusive-time-of-functions/)
- [2434. Using A Robot To Print The Lexicographically Smallest String](https://leetcode.com/problems/using-a-robot-to-print-the-lexicographically-smallest-string/) 1953
- [895. Maximum Frequency Stack](https://leetcode.com/problems/maximum-frequency-stack/) 2028
- [1172. Dinner Plate Stacks](https://leetcode.com/problems/dinner-plate-stacks/) 2110
- [2589. Minimum Time To Complete All Tasks](https://leetcode.com/problems/minimum-time-to-complete-all-tasks/) 2381 (more than one approach)
- [2524. Maximum Frequency Score Of A Subarray](https://leetcode.com/problems/maximum-frequency-score-of-a-subarray/) 🔒
- [716. Max Stack](https://leetcode.com/problems/max-stack/) 🔒

### §3.3 Adjacent Element Elimination

- [2696. Minimum String Length After Removing Substrings](https://leetcode.com/problems/minimum-string-length-after-removing-substrings/) 1282
- [1047. Remove All Adjacent Duplicates In String](https://leetcode.com/problems/remove-all-adjacent-duplicates-in-string/) 1286
- [1544. Make The String Great](https://leetcode.com/problems/make-the-string-great/) 1344
- [3561. Resulting String After Adjacent Removals](https://leetcode.com/problems/resulting-string-after-adjacent-removals/) 1397
- [1003. Check If Word Is Valid After Substitutions](https://leetcode.com/problems/check-if-word-is-valid-after-substitutions/) 1427
- [3834. Merge Adjacent Equal Elements](https://leetcode.com/problems/merge-adjacent-equal-elements/) 1429
- [2216. Minimum Deletions To Make Array Beautiful](https://leetcode.com/problems/minimum-deletions-to-make-array-beautiful/) 1510
- [1209. Remove All Adjacent Duplicates In String II](https://leetcode.com/problems/remove-all-adjacent-duplicates-in-string-ii/) 1542
- [3703. Remove K-Balanced Substrings](https://leetcode.com/problems/remove-k-balanced-substrings/) 1802 (related to 1209)
- [1717. Maximum Score From Removing Substrings](https://leetcode.com/problems/maximum-score-from-removing-substrings/) 1868
- [2197. Replace Non Coprime Numbers In Array](https://leetcode.com/problems/replace-non-coprime-numbers-in-array/) 2057
- [735. Asteroid Collision](https://leetcode.com/problems/asteroid-collision/)
- [2751. Robot Collisions](https://leetcode.com/problems/robot-collisions/) 2092 (related to 735)

### §3.4 Valid Bracket Sequences (RBS)

Note: some problems don't need a stack at all — a single counter tracking nesting depth is enough.

- [20. Valid Parentheses](https://leetcode.com/problems/valid-parentheses/)
- [921. Minimum Add To Make Parentheses Valid](https://leetcode.com/problems/minimum-add-to-make-parentheses-valid/) 1242
- [1021. Remove Outermost Parentheses](https://leetcode.com/problems/remove-outermost-parentheses/) 1311
- [1614. Maximum Nesting Depth Of The Parentheses](https://leetcode.com/problems/maximum-nesting-depth-of-the-parentheses/) 1323
- [1190. Reverse Substrings Between Each Pair Of Parentheses](https://leetcode.com/problems/reverse-substrings-between-each-pair-of-parentheses/) 1486
- [856. Score Of Parentheses](https://leetcode.com/problems/score-of-parentheses/) 1563
- [1249. Minimum Remove To Make Valid Parentheses](https://leetcode.com/problems/minimum-remove-to-make-valid-parentheses/) 1657
- [1963. Minimum Number Of Swaps To Make The String Balanced](https://leetcode.com/problems/minimum-number-of-swaps-to-make-the-string-balanced/) 1689
- [678. Valid Parenthesis String](https://leetcode.com/problems/valid-parenthesis-string/) ~1700
- [1111. Maximum Nesting Depth Of Two Valid Parentheses Strings](https://leetcode.com/problems/maximum-nesting-depth-of-two-valid-parentheses-strings/) 1749
- [1541. Minimum Insertions To Balance A Parentheses String](https://leetcode.com/problems/minimum-insertions-to-balance-a-parentheses-string/) 1759
- [2116. Check If A Parentheses String Can Be Valid](https://leetcode.com/problems/check-if-a-parentheses-string-can-be-valid/) 2038 (advanced follow-up: CF1709C)
- [32. Longest Valid Parentheses](https://leetcode.com/problems/longest-valid-parentheses/)

### §3.5 Expression Parsing

- [1006. Clumsy Factorial](https://leetcode.com/problems/clumsy-factorial/) 1408 (introduces the idea of a stack)
- [150. Evaluate Reverse Polish Notation](https://leetcode.com/problems/evaluate-reverse-polish-notation/)
- [394. Decode String](https://leetcode.com/problems/decode-string/) (simulate recursion with a stack)
- [8. String To Integer (Atoi)](https://leetcode.com/problems/string-to-integer-atoi/) (warm-up for the problems below)
- [224. Basic Calculator](https://leetcode.com/problems/basic-calculator/)
- [227. Basic Calculator II](https://leetcode.com/problems/basic-calculator-ii/)
- [726. Number Of Atoms](https://leetcode.com/problems/number-of-atoms/)
- [1106. Parsing A Boolean Expression](https://leetcode.com/problems/parsing-a-boolean-expression/) 1880
- [591. Tag Validator](https://leetcode.com/problems/tag-validator/)
- [736. Parse Lisp Expression](https://leetcode.com/problems/parse-lisp-expression/)
- [1096. Brace Expansion II](https://leetcode.com/problems/brace-expansion-ii/) 2349
- [1896. Minimum Cost To Change The Final Value Of Expression](https://leetcode.com/problems/minimum-cost-to-change-the-final-value-of-expression/) 2532
- [65. Valid Number](https://leetcode.com/problems/valid-number/)
- [770. Basic Calculator IV](https://leetcode.com/problems/basic-calculator-iv/) 2863
- [439. Ternary Expression Parser](https://leetcode.com/problems/ternary-expression-parser/) 🔒
- [3749. Evaluate Valid Expressions](https://leetcode.com/problems/evaluate-valid-expressions/) 🔒
- [772. Basic Calculator III](https://leetcode.com/problems/basic-calculator-iii/) 🔒
- [1087. Brace Expansion](https://leetcode.com/problems/brace-expansion/) 🔒
- [1597. Build Binary Expression Tree From Infix Expression](https://leetcode.com/problems/build-binary-expression-tree-from-infix-expression/) 🔒
- [1628. Design An Expression Tree With Evaluate Function](https://leetcode.com/problems/design-an-expression-tree-with-evaluate-function/) 🔒

### §3.6 Back-to-Back Stacks

- [2296. Design A Text Editor](https://leetcode.com/problems/design-a-text-editor/) 1912 (can also be solved with a Splay tree)

### §3.7 Monotonic Stack

See the **[Monotonic Stack](03_monotonic_stack.md)** list.

## IV. Queue

Queues are commonly used in BFS — see the **[Grid](04_grid.md)** and **[Graph Algorithms](06_graph.md)** lists. By contrast, stacks are commonly used in DFS, but there's no need to maintain them by hand (recursion does it for you).

### §4.1 Basics

- [933. Number Of Recent Calls](https://leetcode.com/problems/number-of-recent-calls/) 1338
- [3829. Design Ride Sharing System](https://leetcode.com/problems/design-ride-sharing-system/) 1594
- [950. Reveal Cards In Increasing Order](https://leetcode.com/problems/reveal-cards-in-increasing-order/) 1686
- [649. Dota2 Senate](https://leetcode.com/problems/dota2-senate/)
- [346. Moving Average From Data Stream](https://leetcode.com/problems/moving-average-from-data-stream/) 🔒
- [362. Design Hit Counter](https://leetcode.com/problems/design-hit-counter/) 🔒
- [3851. Maximum Requests Without Violating The Limit](https://leetcode.com/problems/maximum-requests-without-violating-the-limit/) 🔒
- [379. Design Phone Directory](https://leetcode.com/problems/design-phone-directory/) 🔒
- [1429. First Unique Number](https://leetcode.com/problems/first-unique-number/) 🔒
- [2534. Time Taken To Cross The Door](https://leetcode.com/problems/time-taken-to-cross-the-door/) 🔒

### §4.2 Design

- [1670. Design Front Middle Back Queue](https://leetcode.com/problems/design-front-middle-back-queue/) 1610
- [3508. Implement Router](https://leetcode.com/problems/implement-router/) 1851
- [225. Implement Stack Using Queues](https://leetcode.com/problems/implement-stack-using-queues/)
- [232. Implement Queue Using Stacks](https://leetcode.com/problems/implement-queue-using-stacks/)
- [622. Design Circular Queue](https://leetcode.com/problems/design-circular-queue/)
- [641. Design Circular Deque](https://leetcode.com/problems/design-circular-deque/)

### §4.3 Deque

- [2810. Faulty Keyboard](https://leetcode.com/problems/faulty-keyboard/) (achieve O(n))
- [2071. Maximum Number Of Tasks You Can Assign](https://leetcode.com/problems/maximum-number-of-tasks-you-can-assign/) 2648

### §4.4 Monotonic Queue

Personally, I think **monotonic deque** is a more accurate name than "monotonic queue".

Monotonic queue = sliding window + monotonic stack. Master sliding windows and monotonic stacks first, then learn monotonic queues.

**Q**: Enqueue, dequeue, update the answer — in what order should you think about these three steps?

**A**: There are two cases. If updating the answer uses data that includes the current element, enqueue first, then update the answer. If the data used doesn't include the current element, update the answer first, then enqueue. Dequeuing is generally written first: each time you visit a new element, check whether the front of the queue has become invalid (no longer satisfies the requirement), and pop it if so.

- [239. Sliding Window Maximum](https://leetcode.com/problems/sliding-window-maximum/)
- [LCR 184. Design a Self-Checkout System](https://leetcode.cn/problems/dui-lie-de-zui-da-zhi-lcof/)
- [1438. Longest Continuous Subarray With Absolute Diff Less Than Or Equal To Limit](https://leetcode.com/problems/longest-continuous-subarray-with-absolute-diff-less-than-or-equal-to-limit/) 1672
- [2762. Continuous Subarrays](https://leetcode.com/problems/continuous-subarrays/) (same as 1438)
- [3835. Count Subarrays With Cost Less Than Or Equal To K](https://leetcode.com/problems/count-subarrays-with-cost-less-than-or-equal-to-k/) 1759
- [2398. Maximum Number Of Robots Within Budget](https://leetcode.com/problems/maximum-number-of-robots-within-budget/) 1917
- [3589. Count Prime Gap Balanced Subarrays](https://leetcode.com/problems/count-prime-gap-balanced-subarrays/) 2235
- [862. Shortest Subarray With Sum At Least K](https://leetcode.com/problems/shortest-subarray-with-sum-at-least-k/) 2307
- [1499. Max Value Of Equation](https://leetcode.com/problems/max-value-of-equation/) 2456

For monotonic-queue-optimized DP, see **§11.3 Monotonic-Queue-Optimized DP** in [07_dynamic_programming.md](07_dynamic_programming.md).

## V. Heap (Priority Queue)

### §5.1 Basics

- [1046. Last Stone Weight](https://leetcode.com/problems/last-stone-weight/) 1173
- [3264. Final Array State After K Multiplication Operations I](https://leetcode.com/problems/final-array-state-after-k-multiplication-operations-i/) 1178
- [2558. Take Gifts From The Richest Pile](https://leetcode.com/problems/take-gifts-from-the-richest-pile/) 1277
- [2336. Smallest Number In Infinite Set](https://leetcode.com/problems/smallest-number-in-infinite-set/) 1375
- [2530. Maximal Score After Applying K Operations](https://leetcode.com/problems/maximal-score-after-applying-k-operations/) 1386
- [3066. Minimum Operations To Exceed Threshold Value II](https://leetcode.com/problems/minimum-operations-to-exceed-threshold-value-ii/) 1400
- [1962. Remove Stones To Minimize The Total](https://leetcode.com/problems/remove-stones-to-minimize-the-total/) 1419
- [703. Kth Largest Element In A Stream](https://leetcode.com/problems/kth-largest-element-in-a-stream/) (classic problem)
- [3275. K-Th Nearest Obstacle Queries](https://leetcode.com/problems/k-th-nearest-obstacle-queries/) 1420
- [1845. Seat Reservation Manager](https://leetcode.com/problems/seat-reservation-manager/) 1429 (can you achieve a complexity independent of n?)
- [2208. Minimum Operations To Halve Array Sum](https://leetcode.com/problems/minimum-operations-to-halve-array-sum/) 1550
- [2233. Maximum Product After K Increments](https://leetcode.com/problems/maximum-product-after-k-increments/) 1686
- [3296. Minimum Number Of Seconds To Make Mountain Height Zero](https://leetcode.com/problems/minimum-number-of-seconds-to-make-mountain-height-zero/) 1695
- [1942. The Number Of The Smallest Unoccupied Chair](https://leetcode.com/problems/the-number-of-the-smallest-unoccupied-chair/) 1695
- [1801. Number Of Orders In The Backlog](https://leetcode.com/problems/number-of-orders-in-the-backlog/) 1711
- [2406. Divide Intervals Into Minimum Number Of Groups](https://leetcode.com/problems/divide-intervals-into-minimum-number-of-groups/) 1713 (classic problem)
- [3478. Choose K Elements With Maximum Sum](https://leetcode.com/problems/choose-k-elements-with-maximum-sum/) 1753
- [2462. Total Cost To Hire K Workers](https://leetcode.com/problems/total-cost-to-hire-k-workers/) 1764
- [1834. Single Threaded CPU](https://leetcode.com/problems/single-threaded-cpu/) 1798
- [1792. Maximum Average Pass Ratio](https://leetcode.com/problems/maximum-average-pass-ratio/) 1818
- [1167. Minimum Cost To Connect Sticks](https://leetcode.com/problems/minimum-cost-to-connect-sticks/) 🔒
- [253. Meeting Rooms II](https://leetcode.com/problems/meeting-rooms-ii/) 🔒 (classic problem)

### §5.2 Advanced

- [23. Merge K Sorted Lists](https://leetcode.com/problems/merge-k-sorted-lists/)
- [2931. Maximum Spending After Buying Items](https://leetcode.com/problems/maximum-spending-after-buying-items/) 1822
- [3781. Maximum Score After Binary Swaps](https://leetcode.com/problems/maximum-score-after-binary-swaps/) 1823 (two approaches)
- [502. IPO](https://leetcode.com/problems/ipo/)
- [1705. Maximum Number Of Eaten Apples](https://leetcode.com/problems/maximum-number-of-eaten-apples/) 1930
- [778. Swim In Rising Water](https://leetcode.com/problems/swim-in-rising-water/)
- [1631. Path With Minimum Effort](https://leetcode.com/problems/path-with-minimum-effort/) 1948
- [1882. Process Tasks Using Servers](https://leetcode.com/problems/process-tasks-using-servers/) 1979
- [1354. Construct Target Array With Multiple Sums](https://leetcode.com/problems/construct-target-array-with-multiple-sums/) 2015
- [1353. Maximum Number Of Events That Can Be Attended](https://leetcode.com/problems/maximum-number-of-events-that-can-be-attended/) 2016
- [1235. Maximum Profit In Job Scheduling](https://leetcode.com/problems/maximum-profit-in-job-scheduling/) 2023 (more than one approach)
- [632. Smallest Range Covering Elements From K Lists](https://leetcode.com/problems/smallest-range-covering-elements-from-k-lists/) (more than one approach)
- [2542. Maximum Subsequence Score](https://leetcode.com/problems/maximum-subsequence-score/) 2056
- [1383. Maximum Performance Of A Team](https://leetcode.com/problems/maximum-performance-of-a-team/) 2091
- [2402. Meeting Rooms III](https://leetcode.com/problems/meeting-rooms-iii/) 2093
- [2503. Maximum Number Of Points From Grid Queries](https://leetcode.com/problems/maximum-number-of-points-from-grid-queries/) 2196
- [2163. Minimum Difference In Sums After Removal Of Elements](https://leetcode.com/problems/minimum-difference-in-sums-after-removal-of-elements/) 2225
- [857. Minimum Cost To Hire K Workers](https://leetcode.com/problems/minimum-cost-to-hire-k-workers/) 2260
- [1606. Find Servers That Handled Most Number Of Requests](https://leetcode.com/problems/find-servers-that-handled-most-number-of-requests/) 2276
- [1851. Minimum Interval To Include Each Query](https://leetcode.com/problems/minimum-interval-to-include-each-query/) 2286
- [407. Trapping Rain Water II](https://leetcode.com/problems/trapping-rain-water-ii/)
- [2940. Find Building Where Alice And Bob Can Meet](https://leetcode.com/problems/find-building-where-alice-and-bob-can-meet/) 2327
- [3399. Smallest Substring With Identical Characters II](https://leetcode.com/problems/smallest-substring-with-identical-characters-ii/) 2376
- [3266. Final Array State After K Multiplication Operations II](https://leetcode.com/problems/final-array-state-after-k-multiplication-operations-ii/) 2509
- [1675. Minimize Deviation In Array](https://leetcode.com/problems/minimize-deviation-in-array/) 2533
- [2617. Minimum Number Of Visited Cells In A Grid](https://leetcode.com/problems/minimum-number-of-visited-cells-in-a-grid/) 2582
- [2532. Time To Cross A Bridge](https://leetcode.com/problems/time-to-cross-a-bridge/) 2589
- [LCP 33. Water Storage](https://leetcode.cn/problems/o8SXZn/) (thinking question: a faster approach)
- [1500. Design A File Sharing System](https://leetcode.com/problems/design-a-file-sharing-system/) 🔒
- [1199. Minimum Time To Build Blocks](https://leetcode.com/problems/minimum-time-to-build-blocks/) 🔒
- [3506. Find Time Required To Eliminate Bacterial Strains](https://leetcode.com/problems/find-time-required-to-eliminate-bacterial-strains/) 🔒

**Ordered Set**:

- [1348. Tweet Counts Per Frequency](https://leetcode.com/problems/tweet-counts-per-frequency/) 2037
- [855. Exam Room](https://leetcode.com/problems/exam-room/) 2067
- [1912. Design Movie Rental System](https://leetcode.com/problems/design-movie-rental-system/) 2182

### §5.3 Kth Smallest/Largest

Some of these problems can also be solved with binary search.

- [264. Ugly Number II](https://leetcode.com/problems/ugly-number-ii/)
- [378. Kth Smallest Element In A Sorted Matrix](https://leetcode.com/problems/kth-smallest-element-in-a-sorted-matrix/)
- [23. Merge K Sorted Lists](https://leetcode.com/problems/merge-k-sorted-lists/)
- [373. Find K Pairs With Smallest Sums](https://leetcode.com/problems/find-k-pairs-with-smallest-sums/)
- [1439. Find The Kth Smallest Sum Of A Matrix With Sorted Rows](https://leetcode.com/problems/find-the-kth-smallest-sum-of-a-matrix-with-sorted-rows/) 2134
- [786. K-Th Smallest Prime Fraction](https://leetcode.com/problems/k-th-smallest-prime-fraction/) 2169
- [3691. Maximum Total Subarray Value II](https://leetcode.com/problems/maximum-total-subarray-value-ii/) 2469
- [2386. Find The K-Sum Of An Array](https://leetcode.com/problems/find-the-k-sum-of-an-array/) 2648

### §5.4 Rearranging Elements

- [984. String Without AAA Or BBB](https://leetcode.com/problems/string-without-aaa-or-bbb/) 1474 (no heap needed; this problem introduces the greedy idea)
- [767. Reorganize String](https://leetcode.com/problems/reorganize-string/) 1681
- [1054. Distant Barcodes](https://leetcode.com/problems/distant-barcodes/) 1702
- [1405. Longest Happy String](https://leetcode.com/problems/longest-happy-string/) 1821
- [3081. Replace Question Marks In String To Minimize Its Value](https://leetcode.com/problems/replace-question-marks-in-string-to-minimize-its-value/) 1905
- [621. Task Scheduler](https://leetcode.com/problems/task-scheduler/)
- [358. Rearrange String K-Distance Apart](https://leetcode.com/problems/rearrange-string-k-distance-apart/) 🔒

### §5.5 Regret Heap

Heap-based regret greedy.

- [LCP 30. Magic Tower Game](https://leetcode.cn/problems/p0NxJO/)
- [1642. Furthest Building You Can Reach](https://leetcode.com/problems/furthest-building-you-can-reach/) 1962
- [630. Course Schedule III](https://leetcode.com/problems/course-schedule-iii/)
- [871. Minimum Number Of Refueling Stops](https://leetcode.com/problems/minimum-number-of-refueling-stops/) 2074
- [3362. Zero Array Transformation III](https://leetcode.com/problems/zero-array-transformation-iii/) 2424 (no regret step, but the idea is similar to 871)
- [2813. Maximum Elegance Of A K-Length Subsequence](https://leetcode.com/problems/maximum-elegance-of-a-k-length-subsequence/) 2582 (can also be solved without a heap)
- [1388. Pizza With 3N Slices](https://leetcode.com/problems/pizza-with-3n-slices/) (achieve O(n log n))
- [3892. Minimum Operations To Achieve At Least K Peaks](https://leetcode.com/problems/minimum-operations-to-achieve-at-least-k-peaks/) (achieve O(n log n))
- [3049. Earliest Second To Mark Indices II](https://leetcode.com/problems/earliest-second-to-mark-indices-ii/) 3111
- [3711. Maximum Transactions Without Negative Balance](https://leetcode.com/problems/maximum-transactions-without-negative-balance/) 🔒
- [2599. Make The Prefix Sum Non Negative](https://leetcode.com/problems/make-the-prefix-sum-non-negative/) 🔒

### §5.6 Lazy-Deletion Heap

Supports deleting an arbitrary element from the heap.

- [2349. Design A Number Container System](https://leetcode.com/problems/design-a-number-container-system/) 1540
- [3885. Design Event Manager](https://leetcode.com/problems/design-event-manager/) 1548
- [3607. Power Grid Maintenance](https://leetcode.com/problems/power-grid-maintenance/) 1700
- [2353. Design A Food Rating System](https://leetcode.com/problems/design-a-food-rating-system/) 1782
- [3092. Most Frequent IDs](https://leetcode.com/problems/most-frequent-ids/) 1793
- [3408. Design Task Manager](https://leetcode.com/problems/design-task-manager/) 1807
- [2034. Stock Price Fluctuation](https://leetcode.com/problems/stock-price-fluctuation/) 1832
- [3815. Design Auction System](https://leetcode.com/problems/design-auction-system/) 1854
- [1172. Dinner Plate Stacks](https://leetcode.com/problems/dinner-plate-stacks/) 2110
- [218. The Skyline Problem](https://leetcode.com/problems/the-skyline-problem/) (sweep line)
- [3510. Minimum Pair Removal To Sort Array II](https://leetcode.com/problems/minimum-pair-removal-to-sort-array-ii/) 2608
- [3672. Sum Of Weighted Modes In Subarrays](https://leetcode.com/problems/sum-of-weighted-modes-in-subarrays/) 🔒
- [3391. Design A 3D Binary Matrix With Efficient Layer Tracking](https://leetcode.com/problems/design-a-3d-binary-matrix-with-efficient-layer-tracking/) 🔒
- [716. Max Stack](https://leetcode.com/problems/max-stack/) 🔒

### §5.7 Dual Heaps (Dynamic Kth Smallest/Largest)

Some problems need to be combined with a lazy-deletion heap.

More than one approach works; some problems can also be solved with an ordered set / value-range Fenwick tree — see Template 2 of **§8.1 Fenwick Tree** in this list.

- [2102. Sequentially Ordinal Rank Tracker](https://leetcode.com/problems/sequentially-ordinal-rank-tracker/) 2159
- [295. Find Median From Data Stream](https://leetcode.com/problems/find-median-from-data-stream/)
- [480. Sliding Window Median](https://leetcode.com/problems/sliding-window-median/)
- [2653. Sliding Subarray Beauty](https://leetcode.com/problems/sliding-subarray-beauty/) (non-brute-force)
- [1825. Finding MK Average](https://leetcode.com/problems/finding-mk-average/) 2396
- [3505. Minimum Operations To Make Elements Within K-Subarrays Equal](https://leetcode.com/problems/minimum-operations-to-make-elements-within-k-subarrays-equal/) 2539 (sum of distances to the sliding window median)
- [3013. Divide An Array Into Subarrays With Minimum Cost II](https://leetcode.com/problems/divide-an-array-into-subarrays-with-minimum-cost-ii/) 2540
- [3321. Find X-Sum Of All K-Long Subarrays II](https://leetcode.com/problems/find-x-sum-of-all-k-long-subarrays-ii/) 2598
- [3962. Maximum Subarray Sum After At Most K Swaps](https://leetcode.com/problems/maximum-subarray-sum-after-at-most-k-swaps/) 2672
- [LCP 24. Number Game](https://leetcode.cn/problems/5TxKeK/)
- [3369. Design An Array Statistics Tracker](https://leetcode.com/problems/design-an-array-statistics-tracker/) 🔒
- [3422. Minimum Operations To Make Subarray Elements Equal](https://leetcode.com/problems/minimum-operations-to-make-subarray-elements-equal/) 🔒

See also **Dijkstra's algorithm** in the **[Graph Algorithms](06_graph.md)** list.

## VI. Trie

### §6.1 Basics

- [208. Implement Trie (Prefix Tree)](https://leetcode.com/problems/implement-trie-prefix-tree/)
- [3597. Partition String](https://leetcode.com/problems/partition-string/) (non-brute-force)
- [3043. Find The Length Of The Longest Common Prefix](https://leetcode.com/problems/find-the-length-of-the-longest-common-prefix/) (non-brute-force)
- [648. Replace Words](https://leetcode.com/problems/replace-words/)
- [720. Longest Word In Dictionary](https://leetcode.com/problems/longest-word-in-dictionary/)
- [2416. Sum Of Prefix Scores Of Strings](https://leetcode.com/problems/sum-of-prefix-scores-of-strings/) 1725
- [677. Map Sum Pairs](https://leetcode.com/problems/map-sum-pairs/)
- [1268. Search Suggestions System](https://leetcode.com/problems/search-suggestions-system/)
- [1233. Remove Sub Folders From The Filesystem](https://leetcode.com/problems/remove-sub-folders-from-the-filesystem/)
- [820. Short Encoding Of Words](https://leetcode.com/problems/short-encoding-of-words/)
- [2261. K-Divisible Elements Subarrays](https://leetcode.com/problems/k-divisible-elements-subarrays/) (achieve O(n^2))
- [1804. Implement Trie II (Prefix Tree)](https://leetcode.com/problems/implement-trie-ii-prefix-tree/) 🔒
- [2168. Unique Substrings With Equal Digit Frequency](https://leetcode.com/problems/unique-substrings-with-equal-digit-frequency/) 🔒 (same as 2261)

### §6.2 Advanced

- [211. Design Add And Search Words Data Structure](https://leetcode.com/problems/design-add-and-search-words-data-structure/)
- [676. Implement Magic Dictionary](https://leetcode.com/problems/implement-magic-dictionary/)
- [212. Word Search II](https://leetcode.com/problems/word-search-ii/)
- [3093. Longest Common Suffix Queries](https://leetcode.com/problems/longest-common-suffix-queries/) 2118
- [745. Prefix And Suffix Search](https://leetcode.com/problems/prefix-and-suffix-search/)
- [3045. Count Prefix And Suffix Pairs II](https://leetcode.com/problems/count-prefix-and-suffix-pairs-ii/) 2328
- [336. Palindrome Pairs](https://leetcode.com/problems/palindrome-pairs/)
- [1948. Delete Duplicate Folders In System](https://leetcode.com/problems/delete-duplicate-folders-in-system/) 2534
- [425. Word Squares](https://leetcode.com/problems/word-squares/) 🔒
- [527. Word Abbreviation](https://leetcode.com/problems/word-abbreviation/) 🔒
- [588. Design In Memory File System](https://leetcode.com/problems/design-in-memory-file-system/) 🔒
- [616. Add Bold Tag In String](https://leetcode.com/problems/add-bold-tag-in-string/) 🔒
- [758. Bold Words In String](https://leetcode.com/problems/bold-words-in-string/) 🔒
- [642. Design Search Autocomplete System](https://leetcode.com/problems/design-search-autocomplete-system/) 🔒
- [1065. Index Pairs Of A String](https://leetcode.com/problems/index-pairs-of-a-string/) 🔒
- [1166. Design File System](https://leetcode.com/problems/design-file-system/) 🔒
- [1858. Longest Word With All Prefixes](https://leetcode.com/problems/longest-word-with-all-prefixes/) 🔒

**Mind Extensions**:

- [440. K-Th Smallest In Lexicographical Order](https://leetcode.com/problems/k-th-smallest-in-lexicographical-order/)

### §6.3 Trie-Optimized DP

- [139. Word Break](https://leetcode.com/problems/word-break/)
- [140. Word Break II](https://leetcode.com/problems/word-break-ii/)
- [Interview 17.13. Re-Space](https://leetcode.cn/problems/re-space-lcci/)
- [472. Concatenated Words](https://leetcode.com/problems/concatenated-words/) ~2300
- [2977. Minimum Cost To Convert String II](https://leetcode.com/problems/minimum-cost-to-convert-string-ii/) 2696

### §6.4 0-1 Trie (XOR Trie)

Some problems can also be solved with the trial-and-fill method.

- [421. Maximum XOR Of Two Numbers In An Array](https://leetcode.com/problems/maximum-xor-of-two-numbers-in-an-array/) ~2000
- [2935. Maximum Strong Pair XOR II](https://leetcode.com/problems/maximum-strong-pair-xor-ii/) 2349
- [3845. Maximum Subarray XOR With Bounded Range](https://leetcode.com/problems/maximum-subarray-xor-with-bounded-range/)
- [1707. Maximum XOR With An Element From Array](https://leetcode.com/problems/maximum-xor-with-an-element-from-array/) 2359
- [1803. Count Pairs With XOR In A Range](https://leetcode.com/problems/count-pairs-with-xor-in-a-range/) 2479
- [1938. Maximum Genetic Difference Query](https://leetcode.com/problems/maximum-genetic-difference-query/) 2503
- [3632. Subarrays With XOR At Least K](https://leetcode.com/problems/subarrays-with-xor-at-least-k/) 🔒
- [2479. Maximum XOR Of Two Non Overlapping Subtrees](https://leetcode.com/problems/maximum-xor-of-two-non-overlapping-subtrees/) 🔒

## VII. Union-Find

### §7.1 Basics

- [684. Redundant Connection](https://leetcode.com/problems/redundant-connection/)
- [3493. Properties Graph](https://leetcode.com/problems/properties-graph/) 1565
- [990. Satisfiability Of Equality Equations](https://leetcode.com/problems/satisfiability-of-equality-equations/) 1638
- [721. Accounts Merge](https://leetcode.com/problems/accounts-merge/)
- [3532. Path Existence Queries In A Graph I](https://leetcode.com/problems/path-existence-queries-in-a-graph-i/) (there is a simpler approach)
- [737. Sentence Similarity II](https://leetcode.com/problems/sentence-similarity-ii/) 🔒
- [1101. The Earliest Moment When Everyone Become Friends](https://leetcode.com/problems/the-earliest-moment-when-everyone-become-friends/) 🔒
- [1258. Synonymous Sentences](https://leetcode.com/problems/synonymous-sentences/) 🔒

For more basic problems, see the DFS sections of the **[Grid](04_grid.md)** and **[Graph Algorithms](06_graph.md)** lists — most of those can also be implemented with Union-Find.

### §7.2 Advanced

- [3551. Minimum Swaps To Sort By Digit Sum](https://leetcode.com/problems/minimum-swaps-to-sort-by-digit-sum/) 1507 (permutation cycles)
- [2471. Minimum Number Of Operations To Sort A Binary Tree By Level](https://leetcode.com/problems/minimum-number-of-operations-to-sort-a-binary-tree-by-level/) 1635 (permutation cycles)
- [1202. Smallest String With Swaps](https://leetcode.com/problems/smallest-string-with-swaps/) 1855
- [1061. Lexicographically Smallest Equivalent String](https://leetcode.com/problems/lexicographically-smallest-equivalent-string/)
- [1722. Minimize Hamming Distance After Swap Operations](https://leetcode.com/problems/minimize-hamming-distance-after-swap-operations/) 1892
- [3608. Minimum Time For K-Connected Components](https://leetcode.com/problems/minimum-time-for-k-connected-components/) 1893
- [3613. Minimize Maximum Component Cost](https://leetcode.com/problems/minimize-maximum-component-cost/) (similar to 3608)
- [778. Swim In Rising Water](https://leetcode.com/problems/swim-in-rising-water/)
- [3695. Maximize Alternating Sum Using Swaps](https://leetcode.com/problems/maximize-alternating-sum-using-swaps/) 1984 (proof)
- [765. Couples Holding Hands](https://leetcode.com/problems/couples-holding-hands/) 1999
- [2092. Find All People With Secret](https://leetcode.com/problems/find-all-people-with-secret/) 2004
- [839. Similar String Groups](https://leetcode.com/problems/similar-string-groups/) 2054
- [685. Redundant Connection II](https://leetcode.com/problems/redundant-connection-ii/) (non-brute-force)
- [1970. Last Day Where You Can Still Cross](https://leetcode.com/problems/last-day-where-you-can-still-cross/) 2124
- [2076. Process Restricted Friend Requests](https://leetcode.com/problems/process-restricted-friend-requests/) 2131
- [1579. Remove Max Number Of Edges To Keep Graph Fully Traversable](https://leetcode.com/problems/remove-max-number-of-edges-to-keep-graph-fully-traversable/) 2132
- [959. Regions Cut By Slashes](https://leetcode.com/problems/regions-cut-by-slashes/) 2136
- [2812. Find The Safest Path In A Grid](https://leetcode.com/problems/find-the-safest-path-in-a-grid/) 2154
- [2503. Maximum Number Of Points From Grid Queries](https://leetcode.com/problems/maximum-number-of-points-from-grid-queries/) 2196
- [3600. Maximize Spanning Tree Stability With Upgrades](https://leetcode.com/problems/maximize-spanning-tree-stability-with-upgrades/) 2301
- [2867. Count Valid Paths In A Tree](https://leetcode.com/problems/count-valid-paths-in-a-tree/) 2428
- [2421. Number Of Good Paths](https://leetcode.com/problems/number-of-good-paths/) 2445
- [2157. Groups Of Strings](https://leetcode.com/problems/groups-of-strings/) 2499
- [803. Bricks Falling When Hit](https://leetcode.com/problems/bricks-falling-when-hit/) 2765
- [3235. Check If The Rectangle Corner Is Reachable](https://leetcode.com/problems/check-if-the-rectangle-corner-is-reachable/)
- [LCP 71. Water Collector](https://leetcode.cn/problems/kskhHQ/)
- [2459. Sort Array By Moving Items To Empty Space](https://leetcode.com/problems/sort-array-by-moving-items-to-empty-space/) 🔒 (permutation)

See also **Minimum Spanning Tree** in the **[Graph Algorithms](06_graph.md)** list.

### §7.3 Intermediary Union-Find

Connecting n elements pairwise requires O(n^2) edges — too slow. Connecting elements through an intermediary node instead usually needs only O(n) edges.

- [947. Most Stones Removed With Same Row Or Column](https://leetcode.com/problems/most-stones-removed-with-same-row-or-column/) 2035
- [3873. Maximum Points Activated With One Addition](https://leetcode.com/problems/maximum-points-activated-with-one-addition/) (similar to 947)
- [2709. Greatest Common Divisor Traversal](https://leetcode.com/problems/greatest-common-divisor-traversal/) 2172
- [1627. Graph Connectivity With Threshold](https://leetcode.com/problems/graph-connectivity-with-threshold/) 2221
- [952. Largest Component Size By Common Factor](https://leetcode.com/problems/largest-component-size-by-common-factor/) 2272
- [1998. GCD Sort Of An Array](https://leetcode.com/problems/gcd-sort-of-an-array/) 2429
- [1632. Rank Transform Of A Matrix](https://leetcode.com/problems/rank-transform-of-a-matrix/) 2530
- [3378. Count Connected Components In LCM Graph](https://leetcode.com/problems/count-connected-components-in-lcm-graph/) 2532 (similar idea to 1627)
- [2371. Minimize Maximum Value In A Grid](https://leetcode.com/problems/minimize-maximum-value-in-a-grid/) 🔒 (same as 1632)

### §7.4 Union-Find on Arrays

- [1562. Find Latest Group Of Size M](https://leetcode.com/problems/find-latest-group-of-size-m/) 1928
- [1488. Avoid Flood In The City](https://leetcode.com/problems/avoid-flood-in-the-city/) 1974
- [1353. Maximum Number Of Events That Can Be Attended](https://leetcode.com/problems/maximum-number-of-events-that-can-be-attended/) 2016
- [2382. Maximum Segment Sum After Removals](https://leetcode.com/problems/maximum-segment-sum-after-removals/) 2136
- [2334. Subarray With Elements Greater Than Varying Threshold](https://leetcode.com/problems/subarray-with-elements-greater-than-varying-threshold/) 2381
- [3666. Minimum Operations To Equalize Binary String](https://leetcode.com/problems/minimum-operations-to-equalize-binary-string/) 2477
- [2612. Minimum Reverse Operations](https://leetcode.com/problems/minimum-reverse-operations/) 2824

### §7.5 Interval Union-Find

- [3244. Shortest Distance After Road Addition Queries II](https://leetcode.com/problems/shortest-distance-after-road-addition-queries-ii/) 2270
- [1851. Minimum Interval To Include Each Query](https://leetcode.com/problems/minimum-interval-to-include-each-query/) 2286
- [LCP 52. Coloring a BST](https://leetcode.cn/problems/QO5KpG/)
- [2158. Amount Of New Area Painted Each Day](https://leetcode.com/problems/amount-of-new-area-painted-each-day/) 🔒

### §7.6 Weighted Union-Find (Edge-Weighted)

- [399. Evaluate Division](https://leetcode.com/problems/evaluate-division/) (template problem)
- [3887. Incremental Even Weighted Cycle Queries](https://leetcode.com/problems/incremental-even-weighted-cycle-queries/) 2128
- [3710. Maximum Partition Factor](https://leetcode.com/problems/maximum-partition-factor/) 2135
- [2307. Check For Contradictions In Equations](https://leetcode.com/problems/check-for-contradictions-in-equations/) 🔒

Additional template problem: CF1850H.

## VIII. Fenwick Tree and Segment Tree

Any problem solvable with a Fenwick tree can also be solved with a segment tree (the converse isn't always true). But a Fenwick tree is simpler to implement and its code is shorter.

For practice purposes, problems well-suited to a Fenwick tree are placed under Fenwick Tree, and the rest are placed under Segment Tree.

### §8.1 Fenwick Tree (BIT)

**Template 1: Standard Fenwick Tree**

**Template 2: Value-Range Fenwick Tree**

- [307. Range Sum Query - Mutable](https://leetcode.com/problems/range-sum-query-mutable/)
- [3072. Distribute Elements Into Two Arrays II](https://leetcode.com/problems/distribute-elements-into-two-arrays-ii/) 2053 (coordinate compression)
- [3624. Number Of Integers With Popcount Depth Equal To K II](https://leetcode.com/problems/number-of-integers-with-popcount-depth-equal-to-k-ii/) 2086
- [3187. Peaks In Array](https://leetcode.com/problems/peaks-in-array/) 2154
- [3777. Minimum Deletions To Make Alternating Substring](https://leetcode.com/problems/minimum-deletions-to-make-alternating-substring/) 2202 (more than one approach)
- [1649. Create Sorted Array Through Instructions](https://leetcode.com/problems/create-sorted-array-through-instructions/) 2208
- [1626. Best Team With No Conflicts](https://leetcode.com/problems/best-team-with-no-conflicts/)
- [1409. Queries On A Permutation With Key](https://leetcode.com/problems/queries-on-a-permutation-with-key/)
- [2250. Count Number Of Rectangles Containing Each Point](https://leetcode.com/problems/count-number-of-rectangles-containing-each-point/)
- [2179. Count Good Triplets In An Array](https://leetcode.com/problems/count-good-triplets-in-an-array/) 2272
- [1395. Count Number Of Teams](https://leetcode.com/problems/count-number-of-teams/)
- [2659. Make Array Empty](https://leetcode.com/problems/make-array-empty/) 2282
- [3915. Maximum Sum Of Alternating Subsequence With Distance At Least K](https://leetcode.com/problems/maximum-sum-of-alternating-subsequence-with-distance-at-least-k/) 2288
- [2653. Sliding Subarray Beauty](https://leetcode.com/problems/sliding-subarray-beauty/) (binary search on a Fenwick tree)
- [3515. Shortest Path In A Weighted Tree](https://leetcode.com/problems/shortest-path-in-a-weighted-tree/) 2312 (difference Fenwick tree)
- [LCP 05. Distribute LeetCoin](https://leetcode.cn/problems/coin-bonus/) (same as 3515)
- [1505. Minimum Possible Integer After At Most K Adjacent Swaps On Digits](https://leetcode.com/problems/minimum-possible-integer-after-at-most-k-adjacent-swaps-on-digits/) 2337
- [3841. Palindromic Path Queries In A Tree](https://leetcode.com/problems/palindromic-path-queries-in-a-tree/) 2384 (difference Fenwick tree)
- [2926. Maximum Balanced Subsequence Sum](https://leetcode.com/problems/maximum-balanced-subsequence-sum/) 2448
- [2736. Maximum Sum Queries](https://leetcode.com/problems/maximum-sum-queries/) 2533
- [3671. Sum Of Beautiful Subsequences](https://leetcode.com/problems/sum-of-beautiful-subsequences/) 2647 (timestamp-based lazy initialization)
- [3962. Maximum Subarray Sum After At Most K Swaps](https://leetcode.com/problems/maximum-subarray-sum-after-at-most-k-swaps/) 2672 (sum of the smallest k)
- [3382. Maximum Area Rectangle With Point Constraints II](https://leetcode.com/problems/maximum-area-rectangle-with-point-constraints-ii/) 2723 (static 2D point counting)
- [3590. Kth Smallest Path XOR Sum](https://leetcode.com/problems/kth-smallest-path-xor-sum/) (kth smallest)
- [3245. Alternating Groups III](https://leetcode.com/problems/alternating-groups-iii/) 3112 (circular array)
- [3027. Find The Number Of Ways To Place People II](https://leetcode.com/problems/find-the-number-of-ways-to-place-people-ii/) (CDQ divide and conquer)
- [1756. Design Most Recently Used Queue](https://leetcode.com/problems/design-most-recently-used-queue/) 🔒
- [60. Permutation Sequence](https://leetcode.com/problems/permutation-sequence/) (Cantor expansion; can achieve O(n log n))
- [3109. Find The Index Of Permutation](https://leetcode.com/problems/find-the-index-of-permutation/) 🔒 (strengthened data version of 60)
- [2519. Count The Number Of K-Big Indices](https://leetcode.com/problems/count-the-number-of-k-big-indices/) 🔒
- [2613. Beautiful Pairs](https://leetcode.com/problems/beautiful-pairs/) 🔒 (closest pair by Manhattan distance)
- [2921. Maximum Profitable Triplets With Increasing Prices II](https://leetcode.com/problems/maximum-profitable-triplets-with-increasing-prices-ii/) 🔒
- [308. Range Sum Query 2D - Mutable](https://leetcode.com/problems/range-sum-query-2d-mutable/) 🔒 (2D Fenwick tree)

See also **§5.7 Dual Heaps** in this list — some problems can also be solved with a value-range Fenwick tree to find the kth smallest.

### §8.2 Inversion Count

Besides a Fenwick tree, some problems can also be computed alongside **merge sort**.

- [LCR 170. Count of Reverse Pairs in a Transaction](https://leetcode.cn/problems/shu-zu-zhong-de-ni-xu-dui-lcof/)
- [315. Count Of Smaller Numbers After Self](https://leetcode.com/problems/count-of-smaller-numbers-after-self/)
- [493. Reverse Pairs](https://leetcode.com/problems/reverse-pairs/)
- [327. Count Of Range Sum](https://leetcode.com/problems/count-of-range-sum/)
- [2426. Number Of Pairs Satisfying Inequality](https://leetcode.com/problems/number-of-pairs-satisfying-inequality/) 2030
- [3768. Minimum Inversion Count In Subarrays Of Fixed Length](https://leetcode.com/problems/minimum-inversion-count-in-subarrays-of-fixed-length/) 2158
- [1850. Minimum Adjacent Swaps To Reach The Kth Smallest Number](https://leetcode.com/problems/minimum-adjacent-swaps-to-reach-the-kth-smallest-number/) (non-brute-force)
- [2193. Minimum Number Of Moves To Make Palindrome](https://leetcode.com/problems/minimum-number-of-moves-to-make-palindrome/) (non-brute-force)
- [1885. Count Pairs In Two Arrays](https://leetcode.com/problems/count-pairs-in-two-arrays/) 🔒

### §8.3 Segment Tree (No Range Updates)

A segment tree is fundamentally a binary tree. Before learning it, warm up with [104. Maximum Depth of Binary Tree](https://leetcode.com/problems/maximum-depth-of-binary-tree/) and [111. Minimum Depth of Binary Tree](https://leetcode.com/problems/minimum-depth-of-binary-tree/) (bottom-up approach).

Any range can be represented by O(log n) segment-tree ranges; each segment-tree node stores information about its corresponding range.

- **Query**: split the query range into O(log n) ranges, corresponding to O(log n) segment-tree nodes; merge the information from these O(log n) nodes to get the answer.
- **Point update**: O(log n) ranges contain the modified position, so O(log n) nodes need their information updated.

- [3479. Fruits Into Baskets III](https://leetcode.com/problems/fruits-into-baskets-iii/) 2178 (binary search on a segment tree)
- [2940. Find Building Where Alice And Bob Can Meet](https://leetcode.com/problems/find-building-where-alice-and-bob-can-meet/) 2327 (binary search on a segment tree)
- [2286. Booking Concert Tickets In Groups](https://leetcode.com/problems/booking-concert-tickets-in-groups/) 2470 (binary search on a segment tree)
- [3161. Block Placement Queries](https://leetcode.com/problems/block-placement-queries/) 2513
- [3901. Good Subsequence Queries](https://leetcode.com/problems/good-subsequence-queries/) 2545
- [2213. Longest Substring Of One Repeating Character](https://leetcode.com/problems/longest-substring-of-one-repeating-character/) 2629
- [3777. Minimum Deletions To Make Alternating Substring](https://leetcode.com/problems/minimum-deletions-to-make-alternating-substring/)
- [3525. Find X-Value Of Array II](https://leetcode.com/problems/find-x-value-of-array-ii/) 2645
- [3165. Maximum Sum Of Subsequence With Non Adjacent Elements](https://leetcode.com/problems/maximum-sum-of-subsequence-with-non-adjacent-elements/) 2697
- [3410. Maximize Subarray Sum After Removing All Occurrences Of One Element](https://leetcode.com/problems/maximize-subarray-sum-after-removing-all-occurrences-of-one-element/) 2844 (more than one approach)
- [3501. Maximize Active Section With Trade II](https://leetcode.com/problems/maximize-active-section-with-trade-ii/) 2941 (can also be solved with a Sparse Table)
- [LCP 81. The NAND Puzzle](https://leetcode.cn/problems/ryfUiz/)

**Mind Extensions**:

- [1157. Online Majority Element In Subarray](https://leetcode.com/problems/online-majority-element-in-subarray/) 2205
- [2407. Longest Increasing Subsequence II](https://leetcode.com/problems/longest-increasing-subsequence-ii/) 2280
- [2770. Maximum Number Of Jumps To Reach The Last Index](https://leetcode.com/problems/maximum-number-of-jumps-to-reach-the-last-index/) (achieve O(n log n))

### §8.4 Lazy Segment Tree (Range Updates)

Any range can be represented by O(log n) segment-tree ranges; each segment-tree node stores information about its corresponding range.

- **Query**: split the query range into O(log n) ranges, corresponding to O(log n) segment-tree nodes; merge the information from these O(log n) nodes to get the answer.
- **Range update**: also split into O(log n) ranges, corresponding to O(log n) segment-tree nodes. But for non-leaf nodes among them, instead of immediately pushing the update down to child nodes, record "an update happened, with content xxx" as a lazy tag. Only when a later query or update needs to access or modify the information of nodes further down is the recorded update pushed down.

- [2569. Handling Sum Queries After Update](https://leetcode.com/problems/handling-sum-queries-after-update/) 2398
- [1622. Fancy Sequence](https://leetcode.com/problems/fancy-sequence/) 2476 (more than one approach)
- [2502. Design Memory Allocator](https://leetcode.com/problems/design-memory-allocator/)
- [2589. Minimum Time To Complete All Tasks](https://leetcode.com/problems/minimum-time-to-complete-all-tasks/) (non-brute-force)
- [2547. Minimum Cost To Split An Array](https://leetcode.com/problems/minimum-cost-to-split-an-array/) (non-brute-force)
- [850. Rectangle Area II](https://leetcode.com/problems/rectangle-area-ii/) (union of rectangle areas; sweep line; coordinate compression)
- [3454. Separate Squares II](https://leetcode.com/problems/separate-squares-ii/) 2671 (same as 850)
- [3569. Maximize Count Of Distinct Primes After Split](https://leetcode.com/problems/maximize-count-of-distinct-primes-after-split/) 2697
- [3721. Longest Balanced Subarray II](https://leetcode.com/problems/longest-balanced-subarray-ii/) 2724 (HH's Necklace trick)
- [2916. Subarrays Distinct Element Sum Of Squares II](https://leetcode.com/problems/subarrays-distinct-element-sum-of-squares-ii/) 2816
- [LCP 52. Coloring a BST](https://leetcode.cn/problems/QO5KpG/) (can also be solved with a Chtholly tree or Union-Find)

### §8.5 Dynamic Segment Tree

Some problems can also be solved with a **Chtholly tree**.

- [699. Falling Squares](https://leetcode.com/problems/falling-squares/)
- [715. Range Module](https://leetcode.com/problems/range-module/)
- [729. My Calendar I](https://leetcode.com/problems/my-calendar-i/)
- [731. My Calendar II](https://leetcode.com/problems/my-calendar-ii/)
- [732. My Calendar III](https://leetcode.com/problems/my-calendar-iii/)
- [2276. Count Integers In Intervals](https://leetcode.com/problems/count-integers-in-intervals/) 2222
- [3590. Kth Smallest Path XOR Sum](https://leetcode.com/problems/kth-smallest-path-xor-sum/) 2646 (segment tree merging)

### §8.6 Persistent Segment Tree

- [3762. Minimum Operations To Equalize Subarrays](https://leetcode.com/problems/minimum-operations-to-equalize-subarrays/) 2497

### §8.7 Sparse Table (ST)

A **Sparse Table (ST)** supports range min/max queries (RMQ) but does not support updates.

Its advantage is short code and O(1) query time, so it is included here as supplementary material.

- [3691. Maximum Total Subarray Value II](https://leetcode.com/problems/maximum-total-subarray-value-ii/) 2469
- [3501. Maximize Active Section With Trade II](https://leetcode.com/problems/maximize-active-section-with-trade-ii/) 2941

**2D Sparse Table**:

- [3933. Largest Local Values In A Matrix II](https://leetcode.com/problems/largest-local-values-in-a-matrix-ii/) (template problem)

## IX. Splay Tree

- [2296. Design A Text Editor](https://leetcode.com/problems/design-a-text-editor/)
- [3526. Range XOR Queries With Subarray Reversals](https://leetcode.com/problems/range-xor-queries-with-subarray-reversals/) 🔒

## X. Sqrt Decomposition Algorithms

### §10.1 Block Decomposition

Note: the Fenwick tree and segment tree problems above can also be attempted with **block decomposition**, e.g. [307. Range Sum Query - Mutable](https://leetcode.com/problems/range-sum-query-mutable/).

- [3943. Number Of Pairs After Increment](https://leetcode.com/problems/number-of-pairs-after-increment/) 2410

### §10.2 Sqrt Decomposition

- [3655. XOR After Range Multiplication Queries II](https://leetcode.com/problems/xor-after-range-multiplication-queries-ii/) 2454
- [LCP 16. Sightseeing Plan for a Park](https://leetcode.cn/problems/you-le-yuan-de-you-lan-ji-hua/)
- [1714. Sum Of Special Evenly Spaced Elements In Array](https://leetcode.com/problems/sum-of-special-evenly-spaced-elements-in-array/) 🔒
- [3400. Maximum Number Of Matching Indices After Right Shifts](https://leetcode.com/problems/maximum-number-of-matching-indices-after-right-shifts/) 🔒 (non-brute-force)

### §10.3 Mo's Algorithm

This is a form of offline algorithm.

- [3636. Threshold Majority Queries](https://leetcode.com/problems/threshold-majority-queries/) 2451 (rollback Mo's algorithm)
- [3590. Kth Smallest Path XOR Sum](https://leetcode.com/problems/kth-smallest-path-xor-sum/) 2646 (more than one approach)
- [2846. Minimum Edge Weight Equilibrium Queries In A Tree](https://leetcode.com/problems/minimum-edge-weight-equilibrium-queries-in-a-tree/) (Mo's algorithm on trees; an approach independent of the edge-weight range)

### §10.4 Other

- [3234. Count The Number Of Substrings With Dominant Ones](https://leetcode.com/problems/count-the-number-of-substrings-with-dominant-ones/) 2557

## Topic: Offline Algorithms

By changing the order in which queries are answered, the problem becomes easier to handle.

> Correspondingly, an **online algorithm** processes queries one by one in the given order.

- [2343. Query Kth Smallest Trimmed Number](https://leetcode.com/problems/query-kth-smallest-trimmed-number/) 1652
- [3607. Power Grid Maintenance](https://leetcode.com/problems/power-grid-maintenance/) 1700
- [2070. Most Beautiful Item For Each Query](https://leetcode.com/problems/most-beautiful-item-for-each-query/) 1724
- [1847. Closest Room](https://leetcode.com/problems/closest-room/) 2082
- [2503. Maximum Number Of Points From Grid Queries](https://leetcode.com/problems/maximum-number-of-points-from-grid-queries/) 2196
- [1851. Minimum Interval To Include Each Query](https://leetcode.com/problems/minimum-interval-to-include-each-query/) 2286
- [1697. Checking Existence Of Edge Length Limited Paths](https://leetcode.com/problems/checking-existence-of-edge-length-limited-paths/) 2300
- [2940. Find Building Where Alice And Bob Can Meet](https://leetcode.com/problems/find-building-where-alice-and-bob-can-meet/) 2327
- [2747. Count Zero Request Servers](https://leetcode.com/problems/count-zero-request-servers/) 2405
- [1938. Maximum Genetic Difference Query](https://leetcode.com/problems/maximum-genetic-difference-query/) 2503
- [2736. Maximum Sum Queries](https://leetcode.com/problems/maximum-sum-queries/) 2533
- [3590. Kth Smallest Path XOR Sum](https://leetcode.com/problems/kth-smallest-path-xor-sum/) 2646
- [3382. Maximum Area Rectangle With Point Constraints II](https://leetcode.com/problems/maximum-area-rectangle-with-point-constraints-ii/) 2723 (static 2D point counting)

## Programming Ability Reinforcement Training

Problems where you roughly know the approach but implementation is tricky. Some are simulation problems.

### Part A

- [12. Integer To Roman](https://leetcode.com/problems/integer-to-roman/)
- [13. Roman To Integer](https://leetcode.com/problems/roman-to-integer/)
- [273. Integer To English Words](https://leetcode.com/problems/integer-to-english-words/)
- [68. Text Justification](https://leetcode.com/problems/text-justification/)
- [420. Strong Password Checker](https://leetcode.com/problems/strong-password-checker/)
- [8. String To Integer (Atoi)](https://leetcode.com/problems/string-to-integer-atoi/) (warm-up for 65)
- [65. Valid Number](https://leetcode.com/problems/valid-number/)

See also **§3.5 Expression Parsing** in this list.

### Part B

- [146. LRU Cache](https://leetcode.com/problems/lru-cache/)
- [460. LFU Cache](https://leetcode.com/problems/lfu-cache/)
- [432. All O(1) Data Structure](https://leetcode.com/problems/all-oone-data-structure/)
- [1206. Design Skiplist](https://leetcode.com/problems/design-skiplist/)

### Part C

- [3197. Find The Minimum Area To Cover All Ones II](https://leetcode.com/problems/find-the-minimum-area-to-cover-all-ones-ii/) 2541
- [2532. Time To Cross A Bridge](https://leetcode.com/problems/time-to-cross-a-bridge/) 2589
- [2056. Number Of Valid Move Combinations On Chessboard](https://leetcode.com/problems/number-of-valid-move-combinations-on-chessboard/) 2611
- [LCP 48. Infinite Chess Game](https://leetcode.cn/problems/fsa7oZ/)
- [LCP 21. Chasing Game](https://leetcode.cn/problems/Za25hA/)
- [LCP 58. Assembling Building Blocks](https://leetcode.cn/problems/De4qBB/)
- [LCP 13. Treasure Hunt](https://leetcode.cn/problems/xun-bao/)
- [LCP 69. Hello LeetCode!](https://leetcode.cn/problems/rMeRt2/)
- [LCP 76. Magic Chessboard](https://leetcode.cn/problems/1ybDKD/)
- [LCP 82. Tree of All Spirits](https://leetcode.cn/problems/cnHoX6/)

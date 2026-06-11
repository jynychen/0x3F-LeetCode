# Binary Search

> Problem list from [0x3F's LeetCode Problem Lists](https://leetcode.cn/circle/discuss/SqopEo/)

**刷题建议**：初次刷题可以只刷难度低于 1700 分的题目。难度更高的题目常常结合其他算法（数据结构、图论等），等学会其他算法再来刷本题单。

## Binary Search
------

**需求**

**写法**

**如果不存在**

lowerBound(nums,x)

结果为 n

lowerBound(nums,x+1)

结果为 n

lowerBound(nums,x)−1

结果为 −1

lowerBound(nums,x+1)−1

结果为 −1

**需求**

**写法**

lowerBound(nums,x)

lowerBound(nums,x+1)

n−lowerBound(nums,x)

n−lowerBound(nums,x+1)

### §1.1 Basics

*   [34. Find First and Last Position of Element in Sorted Array](https://leetcode.com/problems/find-first-and-last-position-of-element-in-sorted-array/)
*   [35. Search Insert Position](https://leetcode.com/problems/search-insert-position/)
*   [704. Binary Search](https://leetcode.com/problems/binary-search/)
*   [744. Find Smallest Letter Greater than Target](https://leetcode.com/problems/find-smallest-letter-greater-than-target/)
*   [2529. Maximum Count of Positive Integer and Negative Integer](https://leetcode.com/problems/maximum-count-of-positive-integer-and-negative-integer/)

### §1.2 Advanced

*   [2300. Successful Pairs of Spells and Potions](https://leetcode.com/problems/successful-pairs-of-spells-and-potions/) 1477
*   [1385. Find the Distance Value Between Two Arrays](https://leetcode.com/problems/find-the-distance-value-between-two-arrays/)
*   [2389. Longest Subsequence with Limited Sum](https://leetcode.com/problems/longest-subsequence-with-limited-sum/)
*   [1170. Compare Strings by Frequency of the Smallest Character](https://leetcode.com/problems/compare-strings-by-frequency-of-the-smallest-character/)
*   [2080. Range Frequency Queries](https://leetcode.com/problems/range-frequency-queries/) 1702
*   [3488. Closest Equal Element Queries](https://leetcode.com/problems/closest-equal-element-queries/)
*   [2563. Count the Number of Fair Pairs](https://leetcode.com/problems/count-the-number-of-fair-pairs/) 1721
*   [2070. Most Beautiful Item for Each Query](https://leetcode.com/problems/most-beautiful-item-for-each-query/) 1724
*   [1146. Snapshot Array](https://leetcode.com/problems/snapshot-array/) 1771
*   [981. Time Based Key Value Store](https://leetcode.com/problems/time-based-key-value-store/)
*   [3508. Implement Router](https://leetcode.com/problems/implement-router/) 1851
*   [658. Find K Closest Elements](https://leetcode.com/problems/find-k-closest-elements/)
*   [1818. Minimum Absolute Sum Difference](https://leetcode.com/problems/minimum-absolute-sum-difference/) 1934
*   [911. Online Election](https://leetcode.com/problems/online-election/) 2001
*   [LCP 08. Ju Qing Hong Fa Shi Jian](https://leetcode.com/problems/ju-qing-hong-fa-shi-jian/)
*   [1182. Shortest Distance to Target Color](https://leetcode.com/problems/shortest-distance-to-target-color/) (Premium)
*   [2819. Minimum Relative Loss after Buying Chocolates](https://leetcode.com/problems/minimum-relative-loss-after-buying-chocolates/) (Premium)

**思维扩展**：

*   [1287. Element Appearing More than 25 in Sorted Array](https://leetcode.com/problems/element-appearing-more-than-25-in-sorted-array/)
*   [2476. Closest Nodes Queries in a Binary Search Tree](https://leetcode.com/problems/closest-nodes-queries-in-a-binary-search-tree/) 1597
*   [1150. Check If a Number is Majority Element in a Sorted Array](https://leetcode.com/problems/check-if-a-number-is-majority-element-in-a-sorted-array/) (Premium)

## Binary Search on Answer
------

### §2.1 求最小

#### 答疑

**问**：如何把二分答案与数组上的二分查找联系起来？

**答**：假设答案在区间 \[2,5\] 中，我们相当于在一个**虚拟数组** \[check(2),check(3),check(4),check(5)\] 中二分找第一个（或者最后一个）值为 true 的 check(x)。这同样可以用红蓝染色法思考。

**问**：有些题目，明明 m 可以是答案，但却不在初始二分区间中。比如闭区间二分初始化 right\=m−1（或者开区间 right\=m），这不会算错吗？

**答**：不会算错。注意「答案所在区间」和「二分区间」是两个概念。想一想，如果二分的 while 循环每次更新的都是 left，那么最终答案是什么？正好就是 m。一般地，如果一开始就能确定 m 一定可以满足题目要求，那么 m 是不需要在二分区间中的。换句话说，二分区间是「尚未确定是否满足题目要求」的数的范围。那些在区间外面的数，都是已确定的满足（不满足）题目要求的数。

**问**：什么是循环不变量？

**答**：想一想，对于求最小的题目，**开区间二分**的写法，为什么最终返回的是 right，而不是别的数？在初始化（循环之前）、循环中、循环结束后，都时时刻刻保证 `check(right) == true` 和 `check(left) == false`，这就叫**循环不变量**。根据循环不变量，循环结束时 left+1\=right，那么 right 就是最小的满足要求的数（因为再 −1 就不满足要求了），所以答案是 right。

Python3

Java

C++

Go

    class Solution:
        def binarySearchMin(self, nums: List[int]) -> int:
            def check(mid: int) -> bool:
                # TODO

                mid = (left + right) // 2
            # 此时 check(left) == False 而 check(left+1) == check(right) == True
            return right

*   [1283. Find the Smallest Divisor Given a Threshold](https://leetcode.com/problems/find-the-smallest-divisor-given-a-threshold/) 1542
*   [2187. Minimum Time to Complete Trips](https://leetcode.com/problems/minimum-time-to-complete-trips/) 1641
*   [1011. Capacity to Ship Packages Within D Days](https://leetcode.com/problems/capacity-to-ship-packages-within-d-days/) 1725
*   [875. Koko Eating Bananas](https://leetcode.com/problems/koko-eating-bananas/) 1766
*   [3296. Minimum Number of Seconds to Make Mountain Height Zero](https://leetcode.com/problems/minimum-number-of-seconds-to-make-mountain-height-zero/) ：，， 1850
*   [3639. Minimum Time to Activate String](https://leetcode.com/problems/minimum-time-to-activate-string/) 1853
*   [475. Heaters](https://leetcode.com/problems/heaters/)
*   [2594. Minimum Time to Repair Cars](https://leetcode.com/problems/minimum-time-to-repair-cars/) 1915
*   [1482. Minimum Number of Days to Make M Bouquets](https://leetcode.com/problems/minimum-number-of-days-to-make-m-bouquets/) 1946
*   [3048. Earliest Second to Mark Indices I](https://leetcode.com/problems/earliest-second-to-mark-indices-i/) 2263
*   [2604. Minimum Time to Eat All Grains](https://leetcode.com/problems/minimum-time-to-eat-all-grains/) (Premium)
*   [2702. Minimum Operations to Make Numbers Non Positive](https://leetcode.com/problems/minimum-operations-to-make-numbers-non-positive/) (Premium)

**思维扩展**：

*   [1870. Minimum Speed to Arrive on Time](https://leetcode.com/problems/minimum-speed-to-arrive-on-time/) 1676
*   [3453. Separate Squares I](https://leetcode.com/problems/separate-squares-i/) 1735

### §2.2 求最大

*   求最小：`check(mid) == true` 时更新 `right = mid`，反之更新 `left = mid`，最后返回 `right`。
*   求最大：`check(mid) == true` 时更新 `left = mid`，反之更新 `right = mid`，最后返回 `left`。

Python3

Java

C++

Go

    class Solution:
        def binarySearchMax(self, nums: List[int]) -> int:
            def check(mid: int) -> bool:
                # TODO

            while left + 1 < right:
                mid = (left + right) // 2
                if check(mid):
                else:
                    right = mid
            # 此时 check(left) == True 而 check(left+1) == check(right) == False

*   [275. H Index Ii](https://leetcode.com/problems/h-index-ii/)
*   [2226. Maximum Candies Allocated to K Children](https://leetcode.com/problems/maximum-candies-allocated-to-k-children/) 1646
*   [2982. Find Longest Special Substring that Occurs Thrice Ii](https://leetcode.com/problems/find-longest-special-substring-that-occurs-thrice-ii/) 1773
*   [2576. Find the Maximum Number of Marked Indices](https://leetcode.com/problems/find-the-maximum-number-of-marked-indices/) 1843
*   [1898. Maximum Number of Removable Characters](https://leetcode.com/problems/maximum-number-of-removable-characters/) 1913
*   [1802. Maximum Value at a Given Index in a Bounded Array](https://leetcode.com/problems/maximum-value-at-a-given-index-in-a-bounded-array/) 1929
*   [1642. Furthest Building You Can Reach](https://leetcode.com/problems/furthest-building-you-can-reach/) 1962
*   [2861. Maximum Number of Alloys](https://leetcode.com/problems/maximum-number-of-alloys/) 1981
*   [3007. Maximum Number that Sum of the Prices is Less than or Equal to K](https://leetcode.com/problems/maximum-number-that-sum-of-the-prices-is-less-than-or-equal-to-k/) 2258
*   [2141. Maximum Running Time of N Computers](https://leetcode.com/problems/maximum-running-time-of-n-computers/) 2265
*   [2258. Escape the Spreading Fire](https://leetcode.com/problems/escape-the-spreading-fire/) 2347
*   [2071. Maximum Number of Tasks You Can Assign](https://leetcode.com/problems/maximum-number-of-tasks-you-can-assign/) 2648
*   [LCP 78. Nsibyl](https://leetcode.com/problems/Nsibyl/)
*   [1618. Maximum Font to Fit a Sentence in a Screen](https://leetcode.com/problems/maximum-font-to-fit-a-sentence-in-a-screen/) (Premium)
*   [1891. Cutting Ribbons](https://leetcode.com/problems/cutting-ribbons/) (Premium)
*   [2137. Pour Water Between Buckets to Make Water Levels Equal](https://leetcode.com/problems/pour-water-between-buckets-to-make-water-levels-equal/) (Premium)
*   [3344. Maximum Sized Array](https://leetcode.com/problems/maximum-sized-array/) (Premium)
*   [644. Maximum Average Subarray Ii](https://leetcode.com/problems/maximum-average-subarray-ii/) (Premium)

### §2.3 二分间接值

*   [3143. Maximum Points Inside the Square](https://leetcode.com/problems/maximum-points-inside-the-square/) 1697
*   [1648. Sell Diminishing Valued Colored Balls](https://leetcode.com/problems/sell-diminishing-valued-colored-balls/) 2050

### §2.4 最小化最大值

*   [410. Split Array Largest Sum](https://leetcode.com/problems/split-array-largest-sum/)
*   [2064. Minimized Maximum of Products Distributed to Any Store](https://leetcode.com/problems/minimized-maximum-of-products-distributed-to-any-store/) 1886
*   [3613. Minimize Maximum Component Cost](https://leetcode.com/problems/minimize-maximum-component-cost/) 1900
*   [1760. Minimum Limit of Balls in a Bag](https://leetcode.com/problems/minimum-limit-of-balls-in-a-bag/) 1940
*   [1631. Path with Minimum Effort](https://leetcode.com/problems/path-with-minimum-effort/) 1948
*   [2439. Minimize Maximum of Array](https://leetcode.com/problems/minimize-maximum-of-array/) 1965
*   [2560. House Robber Iv](https://leetcode.com/problems/house-robber-iv/) 2081
*   [778. Swim in Rising Water](https://leetcode.com/problems/swim-in-rising-water/) 2097
*   [2616. Minimize the Maximum Difference of Pairs](https://leetcode.com/problems/minimize-the-maximum-difference-of-pairs/) 2155
*   [3419. Minimize the Maximum Edge Weight of Graph](https://leetcode.com/problems/minimize-the-maximum-edge-weight-of-graph/) 2243
*   [2513. Minimize the Maximum of Two Arrays](https://leetcode.com/problems/minimize-the-maximum-of-two-arrays/) 2302
*   [3733. Minimum Time to Complete All Deliveries](https://leetcode.com/problems/minimum-time-to-complete-all-deliveries/)
*   [3399. Smallest Substring with Identical Characters Ii](https://leetcode.com/problems/smallest-substring-with-identical-characters-ii/) 2376
*   [3605. Minimum Stability Factor of Array](https://leetcode.com/problems/minimum-stability-factor-of-array/) 2410
*   [LCP 12. Xiao Zhang Shua Ti Ji Hua](https://leetcode.com/problems/xiao-zhang-shua-ti-ji-hua/)
*   [774. Minimize Max Distance to Gas Station](https://leetcode.com/problems/minimize-max-distance-to-gas-station/) (Premium)

### §2.5 最大化最小值

*   [3281. Maximize Score of Numbers in Ranges](https://leetcode.com/problems/maximize-score-of-numbers-in-ranges/) 1768
*   [3620. Network Recovery Pathways](https://leetcode.com/problems/network-recovery-pathways/) 1998
*   [2517. Maximum Tastiness of Candy Basket](https://leetcode.com/problems/maximum-tastiness-of-candy-basket/) 2021
*   [1552. Magnetic Force Between Two Balls](https://leetcode.com/problems/magnetic-force-between-two-balls/)
*   [3710. Maximum Partition Factor](https://leetcode.com/problems/maximum-partition-factor/) 2135
*   [2812. Find the Safest Path in a Grid](https://leetcode.com/problems/find-the-safest-path-in-a-grid/) 2154
*   [2528. Maximize the Minimum Powered City](https://leetcode.com/problems/maximize-the-minimum-powered-city/) 2236
*   [3600. Maximize Spanning Tree Stability with Upgrades](https://leetcode.com/problems/maximize-spanning-tree-stability-with-upgrades/) 2301
*   [3449. Maximize the Minimum Game Score](https://leetcode.com/problems/maximize-the-minimum-game-score/) 2748
*   [3464. Maximize the Distance Between Points on a Square](https://leetcode.com/problems/maximize-the-distance-between-points-on-a-square/) 2806
*   [1102. Path with Maximum Minimum Value](https://leetcode.com/problems/path-with-maximum-minimum-value/) (Premium)
*   [1231. Divide Chocolate](https://leetcode.com/problems/divide-chocolate/) (Premium)

### §2.6 第 K 小/大

*   第 k 小等价于：求**最小**的 x，满足 ≤x 的数**至少**有 k 个。
*   第 k 大等价于：求**最大**的 x，满足 ≥x 的数**至少**有 k 个。

> 

*   [668. Kth Smallest Number in Multiplication Table](https://leetcode.com/problems/kth-smallest-number-in-multiplication-table/)
*   [378. Kth Smallest Element in a Sorted Matrix](https://leetcode.com/problems/kth-smallest-element-in-a-sorted-matrix/)
*   [719. Find K Th Smallest Pair Distance](https://leetcode.com/problems/find-k-th-smallest-pair-distance/)
*   [878. Nth Magical Number](https://leetcode.com/problems/nth-magical-number/) 1897
*   [1201. Ugly Number Iii](https://leetcode.com/problems/ugly-number-iii/) 2039
*   [793. Preimage Size of Factorial Zeroes Function](https://leetcode.com/problems/preimage-size-of-factorial-zeroes-function/) 2100
*   [373. Find K Pairs with Smallest Sums](https://leetcode.com/problems/find-k-pairs-with-smallest-sums/)
*   [1439. Find the Kth Smallest Sum of a Matrix with Sorted Rows](https://leetcode.com/problems/find-the-kth-smallest-sum-of-a-matrix-with-sorted-rows/) 2134
*   [786. K Th Smallest Prime Fraction](https://leetcode.com/problems/k-th-smallest-prime-fraction/) 2169
*   [3116. Kth Smallest Amount with Single Denomination Combination](https://leetcode.com/problems/kth-smallest-amount-with-single-denomination-combination/) 2387
*   [3134. Find the Median of the Uniqueness Array](https://leetcode.com/problems/find-the-median-of-the-uniqueness-array/) 2451
*   [2040. Kth Smallest Product of Two Sorted Arrays](https://leetcode.com/problems/kth-smallest-product-of-two-sorted-arrays/) 2518
*   [2386. Find the K Sum of an Array](https://leetcode.com/problems/find-the-k-sum-of-an-array/) 2648
*   [1508. Range Sum of Sorted Subarray Sums](https://leetcode.com/problems/range-sum-of-sorted-subarray-sums/)
*   [3691. Maximum Total Subarray Value Ii](https://leetcode.com/problems/maximum-total-subarray-value-ii/) k
*   [3520. Minimum Threshold for Inversion Pairs Count](https://leetcode.com/problems/minimum-threshold-for-inversion-pairs-count/) (Premium)
*   [1918. Kth Smallest Subarray Sum](https://leetcode.com/problems/kth-smallest-subarray-sum/) (Premium)

-----

*   [1515. Best Position for a Service Centre](https://leetcode.com/problems/best-position-for-a-service-centre/) 2157

四、其他
----

*   [69. Sqrtx](https://leetcode.com/problems/sqrtx/) m， m2≤x m2\>x  m，
*   [74. Search a 2d Matrix](https://leetcode.com/problems/search-a-2d-matrix/)
*   [278. First Bad Version](https://leetcode.com/problems/first-bad-version/)
*   [374. Guess Number Higher or Lower](https://leetcode.com/problems/guess-number-higher-or-lower/)
*   [162. Find Peak Element](https://leetcode.com/problems/find-peak-element/)
*   [1901. Find a Peak Element Ii](https://leetcode.com/problems/find-a-peak-element-ii/)
*   [852. Peak Index in a Mountain Array](https://leetcode.com/problems/peak-index-in-a-mountain-array/)
*   [1095. Find in Mountain Array](https://leetcode.com/problems/find-in-mountain-array/) 1827
*   [153. Find Minimum in Rotated Sorted Array](https://leetcode.com/problems/find-minimum-in-rotated-sorted-array/)
*   [154. Find Minimum in Rotated Sorted Array Ii](https://leetcode.com/problems/find-minimum-in-rotated-sorted-array-ii/)
*   [33. Search in Rotated Sorted Array](https://leetcode.com/problems/search-in-rotated-sorted-array/)
*   [81. Search in Rotated Sorted Array Ii](https://leetcode.com/problems/search-in-rotated-sorted-array-ii/)
*   [222. Count Complete Tree Nodes](https://leetcode.com/problems/count-complete-tree-nodes/)
*   [1539. Kth Missing Positive Number](https://leetcode.com/problems/kth-missing-positive-number/)
*   [540. Single Element in a Sorted Array](https://leetcode.com/problems/single-element-in-a-sorted-array/)
*   [4. Median of Two Sorted Arrays](https://leetcode.com/problems/median-of-two-sorted-arrays/)
*   [1064. Fixed Point](https://leetcode.com/problems/fixed-point/) (Premium)
*   [702. Search in a Sorted Array of Unknown Size](https://leetcode.com/problems/search-in-a-sorted-array-of-unknown-size/) (Premium)
*   [2936. Number of Equal Numbers Blocks](https://leetcode.com/problems/number-of-equal-numbers-blocks/) (Premium)
*   [1060. Missing Element in Sorted Array](https://leetcode.com/problems/missing-element-in-sorted-array/) (Premium)
*   [1198. Find Smallest Common Element in All Rows](https://leetcode.com/problems/find-smallest-common-element-in-all-rows/) (Premium)
*   [1428. Leftmost Column with at Least a One](https://leetcode.com/problems/leftmost-column-with-at-least-a-one/) (Premium)
*   [1533. Find the Index of the Large Integer](https://leetcode.com/problems/find-the-index-of-the-large-integer/) (Premium)
*   [2387. Median of a Row Wise Sorted Matrix](https://leetcode.com/problems/median-of-a-row-wise-sorted-matrix/) (Premium)
*   [302. Smallest Rectangle Enclosing Black Pixels](https://leetcode.com/problems/smallest-rectangle-enclosing-black-pixels/) (Premium)


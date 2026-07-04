# Greedy

Problem list from [0x3F's LeetCode Study Plan](https://leetcode.cn/circle/discuss/g6KTKL/) — Greedy Algorithms (Basic Strategies / Regret / Intervals / Lexicographic Order / Math / Thinking / Construction).

> Sometimes it's hard to tell at a glance whether a problem is greedy or DP.

## Preface

To make practicing easier, I've put the more formulaic greedy problems first, and the more flexible thinking/construction problems later. Within each subsection, problems are sorted from easy to hard.

**If you're stuck with no idea how to approach a problem, check out the "Thinking Checklist" in Chapter V of this list.**

## I. Greedy Strategies

There are two **basic greedy strategies**:

- Greedily start from the **smallest/largest** value, prioritizing the smallest/largest number, and proceed from small to large / large to small. Building on this, we get **regret greedy** (greedy with backtracking/exchange).
- Greedily start from the **leftmost/rightmost** element, thinking about the greedy choice for the first/last element, which converts the original problem on n numbers into a subproblem on n−1 numbers (or fewer).

### §1.1 Greedy From the Smallest/Largest Value

Prioritize the smallest/largest number, and proceed greedily from small to large / large to small.

If the answer doesn't depend on the order of the array elements, you generally need to **sort** first. After sorting, you can compute with a single pass.

- [3074. Apple Redistribution into Boxes](https://leetcode.com/problems/apple-redistribution-into-boxes/) 1198
- [3545. Minimum Deletions for At Most K Distinct Characters](https://leetcode.com/problems/minimum-deletions-for-at-most-k-distinct-characters/) 1211
- [3745. Maximize Expression of Three Elements](https://leetcode.com/problems/maximize-expression-of-three-elements/) 1218
- [2279. Maximum Bags With Full Capacity of Rocks](https://leetcode.com/problems/maximum-bags-with-full-capacity-of-rocks/) 1249
- [1833. Maximum Ice Cream Bars](https://leetcode.com/problems/maximum-ice-cream-bars/) 1253
- [1005. Maximize Sum Of Array After K Negations](https://leetcode.com/problems/maximize-sum-of-array-after-k-negations/) 1275
- [1481. Least Number of Unique Integers after K Removals](https://leetcode.com/problems/least-number-of-unique-integers-after-k-removals/) 1284
- [1403. Minimum Subsequence in Non-Increasing Order](https://leetcode.com/problems/minimum-subsequence-in-non-increasing-order/) 1288
- [3010. Divide an Array Into Subarrays With Minimum Cost I](https://leetcode.com/problems/divide-an-array-into-subarrays-with-minimum-cost-i/) 1292
- [1338. Reduce Array Size to The Half](https://leetcode.com/problems/reduce-array-size-to-the-half/) 1303
- [1710. Maximum Units on a Truck](https://leetcode.com/problems/maximum-units-on-a-truck/) 1310
- [3075. Maximize Happiness of Selected Children](https://leetcode.com/problems/maximize-happiness-of-selected-children/) 1326
- [2554. Maximum Number of Integers to Choose From a Range I](https://leetcode.com/problems/maximum-number-of-integers-to-choose-from-a-range-i/) 1333
- [2126. Destroying Asteroids](https://leetcode.com/problems/destroying-asteroids/) 1335
- [2587. Rearrange Array to Maximize Prefix Score](https://leetcode.com/problems/rearrange-array-to-maximize-prefix-score/) 1337
- [976. Largest Perimeter Triangle](https://leetcode.com/problems/largest-perimeter-triangle/) 1341
- [1561. Maximum Number of Coins You Can Get](https://leetcode.com/problems/maximum-number-of-coins-you-can-get/) 1406
- [3627. Maximum Median Sum of Subsequences of Size 3](https://leetcode.com/problems/maximum-median-sum-of-subsequences-of-size-3/) (same as 1561)
- [3462. Maximum Sum With at Most K Elements](https://leetcode.com/problems/maximum-sum-with-at-most-k-elements/) 1416
- [2099. Find Subsequence of Length K With the Largest Sum](https://leetcode.com/problems/find-subsequence-of-length-k-with-the-largest-sum/) 1447
- [3301. Maximize the Total Height of Unique Towers](https://leetcode.com/problems/maximize-the-total-height-of-unique-towers/) 1448
- [945. Minimum Increment to Make Array Unique](https://leetcode.com/problems/minimum-increment-to-make-array-unique/) 1448
- [1846. Maximum Element After Decreasing and Rearranging](https://leetcode.com/problems/maximum-element-after-decreasing-and-rearranging/) 1454
- [3727. Maximum Alternating Sum of Squares](https://leetcode.com/problems/maximum-alternating-sum-of-squares/) 1455
- [1647. Minimum Deletions to Make Character Frequencies Unique](https://leetcode.com/problems/minimum-deletions-to-make-character-frequencies-unique/) 1510
- [2971. Find Polygon With the Largest Perimeter](https://leetcode.com/problems/find-polygon-with-the-largest-perimeter/) 1521
- [2178. Maximum Split of Positive Even Integers](https://leetcode.com/problems/maximum-split-of-positive-even-integers/) 1538
- [1578. Minimum Time to Make Rope Colorful](https://leetcode.com/problems/minimum-time-to-make-rope-colorful/) 1574
- [2567. Minimum Score by Changing Two Elements](https://leetcode.com/problems/minimum-score-by-changing-two-elements/) 1609
- [1509. Minimum Difference Between Largest and Smallest Value in Three Moves](https://leetcode.com/problems/minimum-difference-between-largest-and-smallest-value-in-three-moves/) 1653
- [2611. Mice and Cheese](https://leetcode.com/problems/mice-and-cheese/) 1663
- [3397. Maximum Number of Distinct Elements After Operations](https://leetcode.com/problems/maximum-number-of-distinct-elements-after-operations/) 1687
- [3457. Eat Pizzas](https://leetcode.com/problems/eat-pizzas/) 1704 (what if we change max to min?)
- [3767. Maximize Points After Choosing K Tasks](https://leetcode.com/problems/maximize-points-after-choosing-k-tasks/) 1704
- [LCP 40. Mental Calculation Challenge](https://leetcode.cn/problems/uOAnQW/) (do this together with the problem below)
- [1262. Greatest Sum Divisible by Three](https://leetcode.com/problems/greatest-sum-divisible-by-three/) 1762
- [948. Bag of Tokens](https://leetcode.com/problems/bag-of-tokens/) 1762
- [1775. Equal Sum Arrays With Minimum Number of Operations](https://leetcode.com/problems/equal-sum-arrays-with-minimum-number-of-operations/) 1850
- [2333. Minimum Sum of Squared Difference](https://leetcode.com/problems/minimum-sum-of-squared-difference/) 2011 (batch reduction)
- [3645. Maximum Total from Optimal Activation Order](https://leetcode.com/problems/maximum-total-from-optimal-activation-order/) 2019
- [2141. Maximum Running Time of N Computers](https://leetcode.com/problems/maximum-running-time-of-n-computers/) 2265
- [1196. How Many Apples Can You Put into the Basket](https://leetcode.com/problems/how-many-apples-can-you-put-into-the-basket/) 🔒
- [2214. Minimum Health to Beat Game](https://leetcode.com/problems/minimum-health-to-beat-game/) 🔒
- [3763. Maximum Total Sum With Threshold Constraints](https://leetcode.com/problems/maximum-total-sum-with-threshold-constraints/) 🔒
- [3730. Maximum Calories Burnt From Jumps](https://leetcode.com/problems/maximum-calories-burnt-from-jumps/) 🔒
- [3476. Maximize Profit from Task Assignment](https://leetcode.com/problems/maximize-profit-from-task-assignment/) 🔒
- [2098. Subsequence of Size K With the Largest Even Sum](https://leetcode.com/problems/subsequence-of-size-k-with-the-largest-even-sum/) 🔒 (same as LCP 40)
- [2548. Maximum Price to Fill a Bag](https://leetcode.com/problems/maximum-price-to-fill-a-bag/) 🔒
- [3119. Maximum Number of Potholes That Can Be Fixed](https://leetcode.com/problems/maximum-number-of-potholes-that-can-be-fixed/) 🔒
- [2557. Maximum Number of Integers to Choose From a Range II](https://leetcode.com/problems/maximum-number-of-integers-to-choose-from-a-range-ii/) 🔒
- [LCS 02. Finish Half of the Problems](https://leetcode.cn/problems/WqXACV/)

**Mind Extensions**:

- [1984. Minimum Difference Between Highest and Lowest of K Scores](https://leetcode.com/problems/minimum-difference-between-highest-and-lowest-of-k-scores/) 1306
- [624. Maximum Distance in Arrays](https://leetcode.com/problems/maximum-distance-in-arrays/)
- [910. Smallest Range II](https://leetcode.com/problems/smallest-range-ii/) 2135
- [2835. Minimum Operations to Form Subsequence With Target Sum](https://leetcode.com/problems/minimum-operations-to-form-subsequence-with-target-sum/) 2207
- [3366. Minimum Array Sum](https://leetcode.com/problems/minimum-array-sum/) (greedy approach estimated ~2900)

### §1.2 Single-Sequence Pairing

Same as above: greedy from the smallest/largest element.

- [2144. Minimum Cost of Buying Candies With Discount](https://leetcode.com/problems/minimum-cost-of-buying-candies-with-discount/) 1261
- [561. Array Partition](https://leetcode.com/problems/array-partition/) ~1300
- [1877. Minimize Maximum Pair Sum in Array](https://leetcode.com/problems/minimize-maximum-pair-sum-in-array/) 1301
- [881. Boats to Save People](https://leetcode.com/problems/boats-to-save-people/) 1530 (classic problem)
- [2592. Maximize Greatness of an Array](https://leetcode.com/problems/maximize-greatness-of-an-array/) 1569 (Tian Ji's horse racing strategy)
- [2576. Find the Maximum Number of Marked Indices](https://leetcode.com/problems/find-the-maximum-number-of-marked-indices/) 1843

### §1.3 Two-Sequence Pairing

Same as above: greedy from the smallest/largest element.

- [2037. Minimum Number of Moves to Seat Everyone](https://leetcode.com/problems/minimum-number-of-moves-to-seat-everyone/) 1357
- [455. Assign Cookies](https://leetcode.com/problems/assign-cookies/) 1381
- [2410. Maximum Matching of Players With Trainers](https://leetcode.com/problems/maximum-matching-of-players-with-trainers/) 1381 (same as 455)
- [1433. Check If a String Can Break Another String](https://leetcode.com/problems/check-if-a-string-can-break-another-string/) 1436
- [870. Advantage Shuffle](https://leetcode.com/problems/advantage-shuffle/) 1648 (Tian Ji's horse racing strategy)
- [826. Most Profit Assigning Work](https://leetcode.com/problems/most-profit-assigning-work/) 1709
- [2449. Minimum Number of Operations to Make Arrays Similar](https://leetcode.com/problems/minimum-number-of-operations-to-make-arrays-similar/) 2076
- [1889. Minimum Space Wasted From Packaging](https://leetcode.com/problems/minimum-space-wasted-from-packaging/) 2214
- [2561. Rearranging Fruits](https://leetcode.com/problems/rearranging-fruits/) 2222
- [2071. Maximum Number of Tasks You Can Assign](https://leetcode.com/problems/maximum-number-of-tasks-you-can-assign/) 2648
- [2323. Find Minimum Time to Finish All Jobs II](https://leetcode.com/problems/find-minimum-time-to-finish-all-jobs-ii/) 🔒

### §1.4 Greedy From the Leftmost/Rightmost Element

For problems that can't simply be sorted, try greedy from left to right / right to left. Think about the greedy choice for the first/last element, converting the original n-number problem into an (n−1)-number (or smaller) subproblem.

Readers can compare the problems below with the linear DP and state machine DP sections in the [Dynamic Programming list](https://leetcode.cn/circle/discuss/tXLS3i/), and think about when only DP works but greedy doesn't — this deepens the understanding of "local optimum" vs. "global optimum".

- [3402. Minimum Operations to Make Columns Strictly Increasing](https://leetcode.com/problems/minimum-operations-to-make-columns-strictly-increasing/) 1246
- [3191. Minimum Operations to Make Binary Array Elements Equal to One I](https://leetcode.com/problems/minimum-operations-to-make-binary-array-elements-equal-to-one-i/) 1312
- [1827. Minimum Operations to Make the Array Increasing](https://leetcode.com/problems/minimum-operations-to-make-the-array-increasing/) 1315
- [2027. Minimum Moves to Convert String](https://leetcode.com/problems/minimum-moves-to-convert-string/) 1346
- [605. Can Place Flowers](https://leetcode.com/problems/can-place-flowers/) ~1400
- [3111. Minimum Rectangles to Cover Points](https://leetcode.com/problems/minimum-rectangles-to-cover-points/) 1401
- [2957. Remove Adjacent Almost-Equal Characters](https://leetcode.com/problems/remove-adjacent-almost-equal-characters/) 1430
- [3192. Minimum Operations to Make Binary Array Elements Equal to One II](https://leetcode.com/problems/minimum-operations-to-make-binary-array-elements-equal-to-one-ii/) 1433
- [1529. Minimum Suffix Flips](https://leetcode.com/problems/minimum-suffix-flips/) (same as 3192)
- [2789. Largest Element in an Array after Merge Operations](https://leetcode.com/problems/largest-element-in-an-array-after-merge-operations/) 1485
- [3576. Transform Array to All Equal Elements](https://leetcode.com/problems/transform-array-to-all-equal-elements/) 1489
- [3849. Maximum Bitwise XOR After Rearrangement](https://leetcode.com/problems/maximum-bitwise-xor-after-rearrangement/) 1556
- [1144. Decrease Elements To Make Array Zigzag](https://leetcode.com/problems/decrease-elements-to-make-array-zigzag/) 1559
- [3228. Maximum Number of Operations to Move Ones to the End](https://leetcode.com/problems/maximum-number-of-operations-to-move-ones-to-the-end/) 1593
- [2086. Minimum Number of Food Buckets to Feed the Hamsters](https://leetcode.com/problems/minimum-number-of-food-buckets-to-feed-the-hamsters/) 1623
- [2571. Minimum Operations to Reduce an Integer to 0](https://leetcode.com/problems/minimum-operations-to-reduce-an-integer-to-0/) 1649
- [3776. Minimum Moves to Balance Circular Array](https://leetcode.com/problems/minimum-moves-to-balance-circular-array/) 1740
- [861. Score After Flipping Matrix](https://leetcode.com/problems/score-after-flipping-matrix/) 1818
- [3326. Minimum Division Operations to Make Array Non-decreasing](https://leetcode.com/problems/minimum-division-operations-to-make-array-non-decreasing/) 1864
- [955. Delete Columns to Make Sorted II](https://leetcode.com/problems/delete-columns-to-make-sorted-ii/) 1876
- [1536. Minimum Swaps to Arrange a Binary Grid](https://leetcode.com/problems/minimum-swaps-to-arrange-a-binary-grid/) 1881
- [2673. Make Costs of Paths Equal in a Binary Tree](https://leetcode.com/problems/make-costs-of-paths-equal-in-a-binary-tree/) 1917
- [1488. Avoid Flood in The City](https://leetcode.com/problems/avoid-flood-in-the-city/) 1974
- [2366. Minimum Replacements to Sort the Array](https://leetcode.com/problems/minimum-replacements-to-sort-the-array/) 2060
- [2528. Maximize the Minimum Powered City](https://leetcode.com/problems/maximize-the-minimum-powered-city/) 2236
- [3449. Maximize the Minimum Game Score](https://leetcode.com/problems/maximize-the-minimum-game-score/) 2748
- [2422. Merge Operations to Turn Array Into a Palindrome](https://leetcode.com/problems/merge-operations-to-turn-array-into-a-palindrome/) 🔒

See also "§3.1 Lexicographically Smallest/Largest" in this list.

### §1.5 Partition Greedy

Split an array/string into segments satisfying certain requirements, minimizing/maximizing the number of segments.

Same approach as above: try greedy from left to right / right to left.

Readers can compare the problems below with the partition DP section in the [Dynamic Programming list](https://leetcode.cn/circle/discuss/tXLS3i/), and think about when only DP works but greedy doesn't — this deepens the understanding of "local optimum" vs. "global optimum".

- [1221. Split a String in Balanced Strings](https://leetcode.com/problems/split-a-string-in-balanced-strings/) 1220
- [2405. Optimal Partition of String](https://leetcode.com/problems/optimal-partition-of-string/) 1355
- [2294. Partition Array Such That Maximum Difference Is K](https://leetcode.com/problems/partition-array-such-that-maximum-difference-is-k/) 1416
- [2358. Maximum Number of Groups Entering a Competition](https://leetcode.com/problems/maximum-number-of-groups-entering-a-competition/) 1503
- [2522. Partition String Into Substrings With Values at Most K](https://leetcode.com/problems/partition-string-into-substrings-with-values-at-most-k/) 1605
- [3557. Find Maximum Number of Non Intersecting Substrings](https://leetcode.com/problems/find-maximum-number-of-non-intersecting-substrings/) 1720
- [1546. Maximum Number of Non-Overlapping Subarrays With Sum Equals Target](https://leetcode.com/problems/maximum-number-of-non-overlapping-subarrays-with-sum-equals-target/) 1855
- [2436. Minimum Split Into Subarrays With GCD Greater Than One](https://leetcode.com/problems/minimum-split-into-subarrays-with-gcd-greater-than-one/) 🔒
- [2892. Minimizing Array After Replacing Pairs With Their Product](https://leetcode.com/problems/minimizing-array-after-replacing-pairs-with-their-product/) 🔒

### §1.6 Enumerate, Then Apply Greedy

Enumerate one of the problem's variables, treat it as a known condition, then apply a greedy strategy on top of that.

You can also enumerate the answer and check whether it satisfies the requirement (similar to binary search on the answer).

- [2171. Removing Minimum Number of Magic Beans](https://leetcode.com/problems/removing-minimum-number-of-magic-beans/) 1748
- [3085. Minimum Deletions to Make String K-Special](https://leetcode.com/problems/minimum-deletions-to-make-string-k-special/) 1765
- [1727. Largest Submatrix With Rearrangements](https://leetcode.com/problems/largest-submatrix-with-rearrangements/) 1927 (can be optimized to O(mn) time)
- [2749. Minimum Operations to Make the Integer Zero](https://leetcode.com/problems/minimum-operations-to-make-the-integer-zero/) 2132
- [2910. Minimum Number of Groups to Create a Valid Assignment](https://leetcode.com/problems/minimum-number-of-groups-to-create-a-valid-assignment/) 2132
- [2234. Maximum Total Beauty of the Gardens](https://leetcode.com/problems/maximum-total-beauty-of-the-gardens/) 2562

### §1.7 Exchange Argument

The exchange argument is used to prove the correctness of a class of greedy algorithms, and can also be used to inspire the approach. Method:

- Guess that processing the data in "some order" gives the optimal solution.
- Swap two elements a_i and a_j in that order, and compute the resulting answer.
- Compare the answers before and after the swap. If the answer never improves after swapping, the guess holds.

Alternatively, without guessing, you can directly compute the answer for "a_i before a_j" and "a_j before a_i", and compare the two to determine which processing order is correct.

[Explanation (using problem 2895 as an example)](https://leetcode.com/problems/minimum-processing-time/solution/tan-xin-pythonjavacgo-by-endlesscheng-8fzf/)

- [1877. Minimize Maximum Pair Sum in Array](https://leetcode.com/problems/minimize-maximum-pair-sum-in-array/) 1301
- [2895. Minimum Processing Time](https://leetcode.com/problems/minimum-processing-time/) 1352
- [3457. Eat Pizzas](https://leetcode.com/problems/eat-pizzas/) 1704
- [1665. Minimum Initial Energy to Finish Tasks](https://leetcode.com/problems/minimum-initial-energy-to-finish-tasks/) 1901
- [3273. Minimum Amount of Damage Dealt to Bob](https://leetcode.com/problems/minimum-amount-of-damage-dealt-to-bob/) 2013
- [2136. Earliest Possible Day of Full Bloom](https://leetcode.com/problems/earliest-possible-day-of-full-bloom/) 2033
- [2561. Rearranging Fruits](https://leetcode.com/problems/rearranging-fruits/) 2222

**Mind Extensions**:

- [179. Largest Number](https://leetcode.com/problems/largest-number/)
- [3309. Maximum Possible Number by Binary Concatenation](https://leetcode.com/problems/maximum-possible-number-by-binary-concatenation/) (non-brute-force)

**Similar Problems**:

- [2412. Minimum Money Required Before Transactions](https://leetcode.com/problems/minimum-money-required-before-transactions/) 2092

### §1.8 Adjacent Elements Different

In the problems below, let n be the length of array a, and m be the count of the most frequent element.

**Problem 1**: Given array a, can its elements be rearranged so that all adjacent elements are different? If so, output the rearranged array.

**Answer**: Possible if m ≤ n−m+1, otherwise impossible.

**Problem 2**: Given array a, each operation removes two different elements from a. What's the maximum number of operations?

**Answer**: At most min(⌊n/2⌋, n−m) operations.

**Problem 3**: Given array a, each operation removes **at most** two different elements from a. What's the minimum number of operations needed to remove all elements?

**Answer**: At least max(⌈n/2⌉, m) operations.

[Proof + concrete construction](https://zhuanlan.zhihu.com/p/1945782212176909162)

- [2335. Minimum Amount of Time to Fill Cups](https://leetcode.com/problems/minimum-amount-of-time-to-fill-cups/) 1360
- [3659. Partition Array Into K Distinct Groups](https://leetcode.com/problems/partition-array-into-k-distinct-groups/) 1440
- [1753. Maximum Score From Removing Stones](https://leetcode.com/problems/maximum-score-from-removing-stones/) 1488 (same as 2335, but with larger constraints)
- [767. Reorganize String](https://leetcode.com/problems/reorganize-string/)
- [1054. Distant Barcodes](https://leetcode.com/problems/distant-barcodes/) 1702 (same as 767)
- [2856. Minimum Array Length After Pair Removals](https://leetcode.com/problems/minimum-array-length-after-pair-removals/) 1750 (an O(log n) approach exists)
- [1953. Maximum Number of Weeks for Which You Can Work](https://leetcode.com/problems/maximum-number-of-weeks-for-which-you-can-work/) 1804
- [3785. Minimum Swaps to Avoid Forbidden Values](https://leetcode.com/problems/minimum-swaps-to-avoid-forbidden-values/) 2052
- [3664. Two Letter Card Game](https://leetcode.com/problems/two-letter-card-game/) 2158
- [3495. Minimum Operations to Make Array Elements Zero](https://leetcode.com/problems/minimum-operations-to-make-array-elements-zero/) 2206 (has an O(1) formula)
- [3139. Minimum Cost to Equalize Array](https://leetcode.com/problems/minimum-cost-to-equalize-array/) 2666
- [621. Task Scheduler](https://leetcode.com/problems/task-scheduler/) (identical elements must be spaced at least n apart)
- [358. Rearrange String k Distance Apart](https://leetcode.com/problems/rearrange-string-k-distance-apart/) 🔒

**Mind Extensions**:

- [984. String Without AAA or BBB](https://leetcode.com/problems/string-without-aaa-or-bbb/)
- [1405. Longest Happy String](https://leetcode.com/problems/longest-happy-string/) 1821

### §1.9 Regret Greedy

Usually requires a **heap**.

[Explanation](https://leetcode.cn/problems/p0NxJO/solution/fan-hui-tan-xin-fu-ti-dan-pythonjavacgoj-hxup/)

- [LCP 30. Magic Tower](https://leetcode.cn/problems/p0NxJO/) ~1900
- [1642. Furthest Building You Can Reach](https://leetcode.com/problems/furthest-building-you-can-reach/) 1962
- [630. Course Schedule III](https://leetcode.com/problems/course-schedule-iii/) ~2000
- [871. Minimum Number of Refueling Stops](https://leetcode.com/problems/minimum-number-of-refueling-stops/) 2074
- [3362. Zero Array Transformation III](https://leetcode.com/problems/zero-array-transformation-iii/) 2424 (no actual "regret" step, but the idea is similar to 871)
- [2813. Maximum Elegance of a K-Length Subsequence](https://leetcode.com/problems/maximum-elegance-of-a-k-length-subsequence/) 2582 (a heap-free approach also exists)
- [3049. Earliest Second to Mark Indices II](https://leetcode.com/problems/earliest-second-to-mark-indices-ii/) 3111
- [3711. Maximum Transactions Without Negative Balance](https://leetcode.com/problems/maximum-transactions-without-negative-balance/) 🔒
- [2599. Make the Prefix Sum Non-negative](https://leetcode.com/problems/make-the-prefix-sum-non-negative/) 🔒

## II. Interval Greedy

Interval greedy has these classic problems:

- **Non-overlapping intervals** (single-machine scheduling / activity selection): given some intervals, select the maximum number of pairwise non-overlapping intervals.
- **Interval grouping** (task scheduling / meeting rooms): given some intervals, split them into the minimum number of groups so that intervals within each group don't overlap.
- **Interval point cover** (shooting balloons, interval stabbing): given some intervals, place the minimum number of points on the number line so that every interval contains at least one point. How many points are needed at minimum?
- **Interval covering** (watering a garden): given some intervals, select the minimum number of intervals that cover a specified segment [s, t].

Generally, the interval merging problem (§2.5) sorts by left endpoint, while most of the other interval greedy problems sort by right endpoint. After practicing these, think carefully about why this sort order is used.

### §2.1 Non-Overlapping Intervals

- [435. Non-overlapping Intervals](https://leetcode.com/problems/non-overlapping-intervals/) ~1700
- [646. Maximum Length of Pair Chain](https://leetcode.com/problems/maximum-length-of-pair-chain/) (same as 435)
- [1520. Maximum Number of Non-Overlapping Substrings](https://leetcode.com/problems/maximum-number-of-non-overlapping-substrings/) 2363
- [3458. Select K Disjoint Special Substrings](https://leetcode.com/problems/select-k-disjoint-special-substrings/) (same as 1520)

**Variant**: each interval has its own score; choose some pairwise non-overlapping intervals to maximize the total score. See "§7.2 Non-overlapping Intervals" in the [Dynamic Programming list](https://leetcode.cn/circle/discuss/tXLS3i/).

### §2.2 Interval Grouping

- [2406. Divide Intervals Into Minimum Number of Groups](https://leetcode.com/problems/divide-intervals-into-minimum-number-of-groups/) 1713
- [253. Meeting Rooms II](https://leetcode.com/problems/meeting-rooms-ii/) 🔒

### §2.3 Interval Point Cover

Essentially the same as non-overlapping intervals.

- [452. Minimum Number of Arrows to Burst Balloons](https://leetcode.com/problems/minimum-number-of-arrows-to-burst-balloons/) ~1700
- [757. Set Intersection Size At Least Two](https://leetcode.com/problems/set-intersection-size-at-least-two/) 2379
- [2589. Minimum Time to Complete All Tasks](https://leetcode.com/problems/minimum-time-to-complete-all-tasks/) 2381
- [LCP 32. Batch Processing Tasks](https://leetcode.cn/problems/t3fKg1/)

### §2.4 Interval Covering

[Illustrated explanation](https://leetcode.com/problems/jump-game-ii/solutions/2926993/tu-jie-yi-zhang-tu-miao-dong-tiao-yue-yo-h2d4/)

- [45. Jump Game II](https://leetcode.com/problems/jump-game-ii/) ~1700
- [1024. Video Stitching](https://leetcode.com/problems/video-stitching/) 1746
- [1326. Minimum Number of Taps to Open to Water a Garden](https://leetcode.com/problems/minimum-number-of-taps-to-open-to-water-a-garden/) 1885

### §2.5 Merging Intervals

> Might not strictly be greedy, but included here for the completeness of this list.

- [56. Merge Intervals](https://leetcode.com/problems/merge-intervals/)
- [57. Insert Interval](https://leetcode.com/problems/insert-interval/)
- [2848. Points That Intersect With Cars](https://leetcode.com/problems/points-that-intersect-with-cars/) (non-brute-force)
- [55. Jump Game](https://leetcode.com/problems/jump-game/)
- [763. Partition Labels](https://leetcode.com/problems/partition-labels/) 1443
- [3169. Count Days Without Meetings](https://leetcode.com/problems/count-days-without-meetings/) 1483
- [2580. Count Ways to Group Overlapping Ranges](https://leetcode.com/problems/count-ways-to-group-overlapping-ranges/) 1632
- [3394. Check if Grid Can Be Cut Into Sections](https://leetcode.com/problems/check-if-grid-can-be-cut-into-sections/) 1916
- [2963. Count the Number of Good Partitions](https://leetcode.com/problems/count-the-number-of-good-partitions/) 1985
- [2584. Split the Array to Make Coprime Products](https://leetcode.com/problems/split-the-array-to-make-coprime-products/) 2159
- [616. Add Bold Tag in String](https://leetcode.com/problems/add-bold-tag-in-string/) 🔒
- [758. Bold Words in String](https://leetcode.com/problems/bold-words-in-string/) 🔒
- [3323. Minimize Connected Groups by Inserting Interval](https://leetcode.com/problems/minimize-connected-groups-by-inserting-interval/) 🔒
- [759. Employee Free Time](https://leetcode.com/problems/employee-free-time/) 🔒
- [2655. Find Maximal Uncovered Ranges](https://leetcode.com/problems/find-maximal-uncovered-ranges/) 🔒

### §2.6 Other Interval Greedy

- [1288. Remove Covered Intervals](https://leetcode.com/problems/remove-covered-intervals/) (non-brute-force)
- [2054. Two Best Non-Overlapping Events](https://leetcode.com/problems/two-best-non-overlapping-events/) 1883
- [1705. Maximum Number of Eaten Apples](https://leetcode.com/problems/maximum-number-of-eaten-apples/) 1930
- [1353. Maximum Number of Events That Can Be Attended](https://leetcode.com/problems/maximum-number-of-events-that-can-be-attended/) 2016

## III. String Greedy

### §3.1 Lexicographically Smallest/Largest

The definition of **lexicographic order**:

- For two strings a and b, compare characters a[i] and b[i] by their character value (code point), from left to right.
- At the first position where a[i]≠b[i]: if a[i]<b[i], then a is lexicographically smaller, otherwise b is smaller.
- If no such position exists, the shorter string is lexicographically smaller.
- If both strings have the same length and content, they have the same lexicographic order.

This definition also generalizes to arrays, comparing them the same way.

- [1323. Maximum 69 Number](https://leetcode.com/problems/maximum-69-number/) 1194
- [3216. Lexicographically Smallest String After a Swap](https://leetcode.com/problems/lexicographically-smallest-string-after-a-swap/) 1243
- [2697. Lexicographically Smallest Palindrome](https://leetcode.com/problems/lexicographically-smallest-palindrome/) 1304
- [3517. Smallest Palindromic Rearrangement I](https://leetcode.com/problems/smallest-palindromic-rearrangement-i/) 1357
- [1881. Maximum Value after Insertion](https://leetcode.com/problems/maximum-value-after-insertion/) 1381
- [2734. Lexicographically Smallest String After Substring Operation](https://leetcode.com/problems/lexicographically-smallest-string-after-substring-operation/) 1405
- [1432. Max Difference You Can Get From Changing an Integer](https://leetcode.com/problems/max-difference-you-can-get-from-changing-an-integer/) 1427
- [1946. Largest Number After Mutating Substring](https://leetcode.com/problems/largest-number-after-mutating-substring/) 1445
- [1663. Smallest String With A Given Numeric Value](https://leetcode.com/problems/smallest-string-with-a-given-numeric-value/) 1461
- [1328. Break a Palindrome](https://leetcode.com/problems/break-a-palindrome/) 1474
- [2259. Remove Digit From Number to Maximize Result](https://leetcode.com/problems/remove-digit-from-number-to-maximize-result/) (non-brute-force)
- [2566. Maximum Difference by Remapping a Digit](https://leetcode.com/problems/maximum-difference-by-remapping-a-digit/) (non-brute-force)
- [670. Maximum Swap](https://leetcode.com/problems/maximum-swap/) (non-brute-force)
- [3106. Lexicographically Smallest String After Operations With Constraint](https://leetcode.com/problems/lexicographically-smallest-string-after-operations-with-constraint/) 1515
- [3723. Maximize Sum of Squares of Digits](https://leetcode.com/problems/maximize-sum-of-squares-of-digits/) 1537
- [1053. Previous Permutation With One Swap](https://leetcode.com/problems/previous-permutation-with-one-swap/) 1633
- [2375. Construct Smallest Number From DI String](https://leetcode.com/problems/construct-smallest-number-from-di-string/) 1642
- [2182. Construct String With Repeat Limit](https://leetcode.com/problems/construct-string-with-repeat-limit/) 1680
- [738. Monotone Increasing Digits](https://leetcode.com/problems/monotone-increasing-digits/) ~1700
- [3403. Find the Lexicographically Largest String From the Box I](https://leetcode.com/problems/find-the-lexicographically-largest-string-from-the-box-i/) 1762
- [3170. Lexicographically Minimum String After Removing Stars](https://leetcode.com/problems/lexicographically-minimum-string-after-removing-stars/) 1772
- [1363. Largest Multiple of Three](https://leetcode.com/problems/largest-multiple-of-three/) 1823
- [3752. Lexicographically Smallest Negated Permutation That Sums to Target](https://leetcode.com/problems/lexicographically-smallest-negated-permutation-that-sums-to-target/) 1827
- [1754. Largest Merge Of Two Strings](https://leetcode.com/problems/largest-merge-of-two-strings/) 1829
- [1202. Smallest String With Swaps](https://leetcode.com/problems/smallest-string-with-swaps/) 1855
- [2434. Using a Robot to Print the Lexicographically Smallest String](https://leetcode.com/problems/using-a-robot-to-print-the-lexicographically-smallest-string/) 1953
- [2948. Make Lexicographically Smallest Array by Swapping Elements](https://leetcode.com/problems/make-lexicographically-smallest-array-by-swapping-elements/) 2047
- [1505. Minimum Possible Integer After at Most K Adjacent Swaps On Digits](https://leetcode.com/problems/minimum-possible-integer-after-at-most-k-adjacent-swaps-on-digits/) 2337
- [3474. Lexicographically Smallest Generated String](https://leetcode.com/problems/lexicographically-smallest-generated-string/) 2605 (the conclusion is easy to guess — how do you prove it?)
- [555. Split Concatenated Strings](https://leetcode.com/problems/split-concatenated-strings/) 🔒
- [3088. Make String Anti-palindrome](https://leetcode.com/problems/make-string-anti-palindrome/) 🔒

**Reverse-Order Greedy**:

- [3720. Lexicographically Smallest Permutation Greater Than Target](https://leetcode.com/problems/lexicographically-smallest-permutation-greater-than-target/) 1958
- [3734. Lexicographically Smallest Palindromic Permutation Greater Than Target](https://leetcode.com/problems/lexicographically-smallest-palindromic-permutation-greater-than-target/) 2330
- [2663. Lexicographically Smallest Beautiful String](https://leetcode.com/problems/lexicographically-smallest-beautiful-string/) 2416
- [2048. Next Greater Numerically Balanced Number](https://leetcode.com/problems/next-greater-numerically-balanced-number/) (non-brute-force)
- [3646. Next Special Palindrome Number](https://leetcode.com/problems/next-special-palindrome-number/) (non-brute-force)
- [3348. Smallest Divisible Digit Product II](https://leetcode.com/problems/smallest-divisible-digit-product-ii/) 3101

See also "IV. Lexicographically Smallest" in the [Monotonic Stack list](https://leetcode.cn/circle/discuss/9oZFK9/).

### §3.2 Palindrome Greedy

> Some of these problems also appear in other greedy categories; they're gathered here for the completeness of this list.

- [409. Longest Palindrome](https://leetcode.com/problems/longest-palindrome/) ~1250
- [2697. Lexicographically Smallest Palindrome](https://leetcode.com/problems/lexicographically-smallest-palindrome/) 1304
- [3517. Smallest Palindromic Rearrangement I](https://leetcode.com/problems/smallest-palindromic-rearrangement-i/) 1357
- [680. Valid Palindrome II](https://leetcode.com/problems/valid-palindrome-ii/) ~1400 (follow-up: how many valid schemes are there?)
- [1328. Break a Palindrome](https://leetcode.com/problems/break-a-palindrome/) 1474
- [1400. Construct K Palindrome Strings](https://leetcode.com/problems/construct-k-palindrome-strings/) 1530
- [2131. Longest Palindrome by Concatenating Two Letter Words](https://leetcode.com/problems/longest-palindrome-by-concatenating-two-letter-words/) 1557
- [2384. Largest Palindromic Number](https://leetcode.com/problems/largest-palindromic-number/) 1636
- [3035. Maximum Palindromes After Operations](https://leetcode.com/problems/maximum-palindromes-after-operations/) 1857
- [1616. Split Two Strings to Make Palindrome](https://leetcode.com/problems/split-two-strings-to-make-palindrome/) 1868
- [1147. Longest Chunked Palindrome Decomposition](https://leetcode.com/problems/longest-chunked-palindrome-decomposition/) 1912
- [2193. Minimum Number of Moves to Make Palindrome](https://leetcode.com/problems/minimum-number-of-moves-to-make-palindrome/) 2091
- [3734. Lexicographically Smallest Palindromic Permutation Greater Than Target](https://leetcode.com/problems/lexicographically-smallest-palindromic-permutation-greater-than-target/) 2330
- [3646. Next Special Palindrome Number](https://leetcode.com/problems/next-special-palindrome-number/) (non-brute-force)
- [266. Palindrome Permutation](https://leetcode.com/problems/palindrome-permutation/) 🔒
- [2422. Merge Operations to Turn Array Into a Palindrome](https://leetcode.com/problems/merge-operations-to-turn-array-into-a-palindrome/) 🔒
- [1842. Next Palindrome Using Same Digits](https://leetcode.com/problems/next-palindrome-using-same-digits/) 🔒
- [3088. Make String Anti-palindrome](https://leetcode.com/problems/make-string-anti-palindrome/) 🔒

See also "§7.1 Palindrome Numbers" in the [Math list](https://leetcode.cn/circle/discuss/IYT3ss/).

### §3.3 Valid Parenthesis Strings

See "§3.4 Valid Parenthesis Strings" in the [Data Structures list](https://leetcode.cn/circle/discuss/mOr1u6/).

## IV. Math Greedy

### §4.1 Basics

- [2160. Minimum Sum of Four Digit Number After Splitting Digits](https://leetcode.com/problems/minimum-sum-of-four-digit-number-after-splitting-digits/) 1314
- [2578. Split With Minimum Sum](https://leetcode.com/problems/split-with-minimum-sum/) 1351
- [2244. Minimum Rounds to Complete All Tasks](https://leetcode.com/problems/minimum-rounds-to-complete-all-tasks/) 1372
- [2870. Minimum Number of Operations to Make Array Empty](https://leetcode.com/problems/minimum-number-of-operations-to-make-array-empty/) 1392
- [1217. Minimum Cost to Move Chips to The Same Position](https://leetcode.com/problems/minimum-cost-to-move-chips-to-the-same-position/) 1408
- [3091. Apply Operations to Make Sum of Array Greater Than or Equal to K](https://leetcode.com/problems/apply-operations-to-make-sum-of-array-greater-than-or-equal-to-k/) 1522
- [LCS 01. Download Plugins](https://leetcode.cn/problems/Ju9Xwi/)
- [397. Integer Replacement](https://leetcode.com/problems/integer-replacement/)

### §4.2 Product Greedy

- [628. Maximum Product of Three Numbers](https://leetcode.com/problems/maximum-product-of-three-numbers/)
- [3732. Maximum Product of Three Elements After One Replacement](https://leetcode.com/problems/maximum-product-of-three-elements-after-one-replacement/) 1529
- [1567. Maximum Length of Subarray With Positive Product](https://leetcode.com/problems/maximum-length-of-subarray-with-positive-product/) 1710

### §4.3 Rearrangement Inequality

Given two arrays a and b, both of length n. You may permute elements within the same array. Minimize/maximize

a[0]·b[0] + a[1]·b[1] + ... + a[n−1]·b[n−1]

Sorting both a and b in ascending order maximizes the sum above.

Sorting a in ascending order and b in descending order minimizes the sum above.

- [2285. Maximum Total Importance of Roads](https://leetcode.com/problems/maximum-total-importance-of-roads/) 1496
- [3016. Minimum Number of Pushes to Type Word II](https://leetcode.com/problems/minimum-number-of-pushes-to-type-word-ii/) 1534
- [1402. Reducing Dishes](https://leetcode.com/problems/reducing-dishes/) 1679
- [2931. Maximum Spending After Buying Items](https://leetcode.com/problems/maximum-spending-after-buying-items/) 1822
- [1589. Maximum Sum Obtained of Any Permutation](https://leetcode.com/problems/maximum-sum-obtained-of-any-permutation/) 1871
- [1874. Minimize Product Sum of Two Arrays](https://leetcode.com/problems/minimize-product-sum-of-two-arrays/) 🔒
- [2268. Minimum Number of Keypresses](https://leetcode.com/problems/minimum-number-of-keypresses/) 🔒 (same as 3016)

**Mind Extensions**:

- [2561. Rearranging Fruits](https://leetcode.com/problems/rearranging-fruits/) 2222 (a min-based rearrangement inequality)
- [3547. Maximum Sum of Edge Values in a Graph](https://leetcode.com/problems/maximum-sum-of-edge-values-in-a-graph/) (chain / cycle)

### §4.4 AM–GM Inequality

**Fence problem**: an n-meter-long fence is used to enclose a rectangle. What's the maximum possible area?

**Variant**: the n-meter-long fence is divided into k pieces, each enclosing a square. What's the minimum possible total area?

- [3081. Replace Question Marks in String to Minimize Its Value](https://leetcode.com/problems/replace-question-marks-in-string-to-minimize-its-value/) 1905
- [1969. Minimum Non-Zero Product of the Array Elements](https://leetcode.com/problems/minimum-non-zero-product-of-the-array-elements/) 1967
- [2939. Maximum Xor Product](https://leetcode.com/problems/maximum-xor-product/) 2128
- [3723. Maximize Sum of Squares of Digits](https://leetcode.com/problems/maximize-sum-of-squares-of-digits/) 1537
- [2897. Apply Operations on Array to Maximize Sum of Squares](https://leetcode.com/problems/apply-operations-on-array-to-maximize-sum-of-squares/) 2301

### §4.5 Median Greedy

Given array nums, each operation can increment or decrement one element by one. Make all elements of nums equal — what's the minimum number of operations?

Making all elements equal to the **median** of nums is optimal.

[Proof](https://zhuanlan.zhihu.com/p/1922938031687595039)

- [462. Minimum Moves to Equal Array Elements II](https://leetcode.com/problems/minimum-moves-to-equal-array-elements-ii/)
- [2033. Minimum Operations to Make a Uni-Value Grid](https://leetcode.com/problems/minimum-operations-to-make-a-uni-value-grid/) 1672
- [2448. Minimum Cost to Make Array Equal](https://leetcode.com/problems/minimum-cost-to-make-array-equal/) 2005 (weighted median)
- [2607. Make K-Subarray Sums Equal](https://leetcode.com/problems/make-k-subarray-sums-equal/) 2071
- [2967. Minimum Cost to Make Array Equalindromic](https://leetcode.com/problems/minimum-cost-to-make-array-equalindromic/) 2116
- [1478. Allocate Mailboxes](https://leetcode.com/problems/allocate-mailboxes/) 2190
- [2968. Apply Operations to Maximize Frequency Score](https://leetcode.com/problems/apply-operations-to-maximize-frequency-score/) 2444
- [1703. Minimum Adjacent Swaps for K Consecutive Ones](https://leetcode.com/problems/minimum-adjacent-swaps-for-k-consecutive-ones/) 2467
- [3762. Minimum Operations to Equalize Subarrays](https://leetcode.com/problems/minimum-operations-to-equalize-subarrays/) 2497
- [3086. Minimum Moves to Pick K Ones](https://leetcode.com/problems/minimum-moves-to-pick-k-ones/) 2673
- [LCP 24. Number Game](https://leetcode.cn/problems/5TxKeK/)
- [3441. Minimum Cost Good Caption](https://leetcode.com/problems/minimum-cost-good-caption/) (advanced approach)
- [Chessboard Reorganization](https://leetcode.cn/contest/2025_pudong_ai/problems/1Hxnb6/) (2D)
- [296. Best Meeting Point](https://leetcode.com/problems/best-meeting-point/) 🔒 (2D)

### §4.6 Induction

- [2952. Minimum Number of Coins to be Added](https://leetcode.com/problems/minimum-number-of-coins-to-be-added/) 1784
- [330. Patching Array](https://leetcode.com/problems/patching-array/) (same as 2952)
- [1798. Maximum Number of Consecutive Values You Can Make](https://leetcode.com/problems/maximum-number-of-consecutive-values-you-can-make/) 1931

### §4.7 Other Math Greedy

- [1414. Find the Minimum Number of Fibonacci Numbers Whose Sum Is K](https://leetcode.com/problems/find-the-minimum-number-of-fibonacci-numbers-whose-sum-is-k/) 1466 (the hard part is the proof)
- [3107. Minimum Operations to Make Median of Array Equal to K](https://leetcode.com/problems/minimum-operations-to-make-median-of-array-equal-to-k/) 1605
- [754. Reach a Number](https://leetcode.com/problems/reach-a-number/) ~2000
- [1058. Minimize Rounding Error to Meet Target](https://leetcode.com/problems/minimize-rounding-error-to-meet-target/) 🔒

## V. Thinking Problems

Recall the last question on a college entrance exam math paper — it usually has three parts: the first two ask you to compute special cases, and the third asks you to compute/prove a general conclusion. This is really the way of thinking **from special cases to the general case**. When solving algorithm problems (especially thinking and construction problems), we can likewise start from the simplest, most special cases to explore the properties of the problem, and gradually work up to the general case.

**Thinking Checklist**

- **Small arrays**: what if nums has only 1 element? Only 2? Only 3?
- **One in a million**: what if all elements of nums are the same? Only one element differs? Two elements differ? One element is especially large?
- **Black and white world**: what if there are only two distinct values? E.g. [0,1,0,1,0,1] or "ababab".
- **Think in reverse**: if the answer is 1, what could the input look like? If the answer is 2? If it's nums[0]? If it's nums[1]?
- **Enumerate and induct**: try building a table for small cases, brute-force enumerate all possibilities, and look for a pattern.

Thinking about these special cases can sometimes spark the **insight** needed to solve the original problem.

### §5.1 From Special Cases to the General Case

- [2745. Construct the Longest New String](https://leetcode.com/problems/construct-the-longest-new-string/) 1607 (think about how to solve it when z=0, z=1, z=2)
- [2611. Mice and Cheese](https://leetcode.com/problems/mice-and-cheese/) 1663 (think about how to solve it when k=1, k=2)
- [1029. Two City Scheduling](https://leetcode.com/problems/two-city-scheduling/) (same as 2611)
- [2645. Minimum Additions to Make Valid String](https://leetcode.com/problems/minimum-additions-to-make-valid-string/) (consider all cases where word has length 2, and the case where the answer is 1)
- [2202. Maximize the Topmost Element After K Moves](https://leetcode.com/problems/maximize-the-topmost-element-after-k-moves/) 1717
- [2568. Minimum Impossible OR](https://leetcode.com/problems/minimum-impossible-or/) 1754
- [1702. Maximum Binary String After Change](https://leetcode.com/problems/maximum-binary-string-after-change/) 1825
- [3012. Minimize Length of Array Using Operations](https://leetcode.com/problems/minimize-length-of-array-using-operations/) 1833
- [2350. Shortest Impossible Sequence of Rolls](https://leetcode.com/problems/shortest-impossible-sequence-of-rolls/) 1961
- [3660. Jump Game IX](https://leetcode.com/problems/jump-game-ix/) 2187
- [517. Super Washing Machines](https://leetcode.com/problems/super-washing-machines/)
- [2499. Minimum Total Cost to Make Arrays Unequal](https://leetcode.com/problems/minimum-total-cost-to-make-arrays-unequal/) 2633
- [3357. Minimize the Maximum Adjacent Element Difference](https://leetcode.com/problems/minimize-the-maximum-adjacent-element-difference/) 3077
- [3431. Minimum Unlocked Indices to Sort Nums](https://leetcode.com/problems/minimum-unlocked-indices-to-sort-nums/) 🔒

### §5.2 Brain Teasers

From the general case to special cases.

- [2733. Neither Minimum nor Maximum](https://leetcode.com/problems/neither-minimum-nor-maximum/) 1148
- [3432. Count Partitions With Even Sum Difference](https://leetcode.com/problems/count-partitions-with-even-sum-difference/) 1200
- [3875. Construct Uniform Parity Array I](https://leetcode.com/problems/construct-uniform-parity-array-i/) 1200
- [1903. Largest Odd Number in String](https://leetcode.com/problems/largest-odd-number-in-string/) 1249
- [2549. Count Distinct Numbers on Board](https://leetcode.com/problems/count-distinct-numbers-on-board/) 1266
- [3746. Maximum Substrings With Distinct Start](https://leetcode.com/problems/maximum-substrings-with-distinct-start/) 1327
- [2396. Strictly Palindromic Number](https://leetcode.com/problems/strictly-palindromic-number/) 1329
- [1689. Partitioning Into Minimum Number Of Deci-Binary Numbers](https://leetcode.com/problems/partitioning-into-minimum-number-of-deci-binary-numbers/) 1355
- [3760. Minimum String Length After Balanced Removals](https://leetcode.com/problems/minimum-string-length-after-balanced-removals/) 1364
- [3674. Minimum Operations to Equalize Array](https://leetcode.com/problems/minimum-operations-to-equalize-array/) 1369
- [3689. Maximum Total Subarray Value I](https://leetcode.com/problems/maximum-total-subarray-value-i/) 1371
- [598. Range Addition II](https://leetcode.com/problems/range-addition-ii/) ~1400
- [521. Longest Uncommon Subsequence I](https://leetcode.com/problems/longest-uncommon-subsequence-i/) ~1400
- [3675. Minimum Operations to Transform String](https://leetcode.com/problems/minimum-operations-to-transform-string/) 1414
- [3227. Vowels Game in a String](https://leetcode.com/problems/vowels-game-in-a-string/) 1452
- [3638. Maximum Balanced Shipments](https://leetcode.com/problems/maximum-balanced-shipments/) 1463
- [3702. Longest Subsequence With Non-Zero Bitwise XOR](https://leetcode.com/problems/longest-subsequence-with-non-zero-bitwise-xor/) 1489
- [3810. Minimum Operations to Reach Target Array](https://leetcode.com/problems/minimum-operations-to-reach-target-array/) 1492
- [2419. Longest Subarray With Maximum Bitwise AND](https://leetcode.com/problems/longest-subarray-with-maximum-bitwise-and/) 1496
- [3424. Minimum Cost to Make Arrays Identical](https://leetcode.com/problems/minimum-cost-to-make-arrays-identical/) 1503
- [1992. Find All Groups of Farmland](https://leetcode.com/problems/find-all-groups-of-farmland/) 1539
- [1007. Minimum Domino Rotations For Equal Row](https://leetcode.com/problems/minimum-domino-rotations-for-equal-row/) 1541
- [2811. Check if it is Possible to Split Array](https://leetcode.com/problems/check-if-it-is-possible-to-split-array/) 1543
- [463. Island Perimeter](https://leetcode.com/problems/island-perimeter/)
- [2211. Count Collisions on a Road](https://leetcode.com/problems/count-collisions-on-a-road/) 1581
- [877. Stone Game](https://leetcode.com/problems/stone-game/) 1590
- [3207. Maximum Points After Enemy Battles](https://leetcode.com/problems/maximum-points-after-enemy-battles/) 1591
- [3828. Final Element After Subarray Deletions](https://leetcode.com/problems/final-element-after-subarray-deletions/) 1591
- [3471. Find the Largest Almost Missing Integer](https://leetcode.com/problems/find-the-largest-almost-missing-integer/) (achieve O(n))
- [2546. Apply Bitwise Operations to Make Strings Equal](https://leetcode.com/problems/apply-bitwise-operations-to-make-strings-equal/) 1605
- [1503. Last Moment Before All Ants Fall Out of a Plank](https://leetcode.com/problems/last-moment-before-all-ants-fall-out-of-a-plank/) 1619
- [2860. Happy Students](https://leetcode.com/problems/happy-students/) 1626
- [1332. Remove Palindromic Subsequences](https://leetcode.com/problems/remove-palindromic-subsequences/) 1629
- [1975. Maximum Matrix Sum](https://leetcode.com/problems/maximum-matrix-sum/) 1648
- [1145. Binary Tree Coloring Game](https://leetcode.com/problems/binary-tree-coloring-game/) 1741
- [2087. Minimum Cost Homecoming of a Robot in a Grid](https://leetcode.com/problems/minimum-cost-homecoming-of-a-robot-in-a-grid/) 1744
- [1297. Maximum Number of Occurrences of a Substring](https://leetcode.com/problems/maximum-number-of-occurrences-of-a-substring/) 1748
- [3577. Count the Number of Computer Unlocking Permutations](https://leetcode.com/problems/count-the-number-of-computer-unlocking-permutations/) 1750
- [3282. Reach End of Array With Max Score](https://leetcode.com/problems/reach-end-of-array-with-max-score/) 1772
- [3644. Maximum K to Sort a Permutation](https://leetcode.com/problems/maximum-k-to-sort-a-permutation/) 1775
- [2712. Minimum Cost to Make All Characters Equal](https://leetcode.com/problems/minimum-cost-to-make-all-characters-equal/) 1791
- [3148. Maximum Difference Score in a Grid](https://leetcode.com/problems/maximum-difference-score-in-a-grid/) 1820
- [2311. Longest Binary Subsequence Less Than or Equal to K](https://leetcode.com/problems/longest-binary-subsequence-less-than-or-equal-to-k/) 1840
- [2332. The Latest Time to Catch a Bus](https://leetcode.com/problems/the-latest-time-to-catch-a-bus/) 1841
- [2680. Maximum OR](https://leetcode.com/problems/maximum-or/) 1912
- [2731. Movement of Robots](https://leetcode.com/problems/movement-of-robots/) 1923 (related to 1503)
- [2556. Disconnect Path in a Binary Matrix by at Most One Flip](https://leetcode.com/problems/disconnect-path-in-a-binary-matrix-by-at-most-one-flip/) 2369
- [3353. Minimum Total Operations](https://leetcode.com/problems/minimum-total-operations/) 🔒
- [1708. Largest Subarray Length K](https://leetcode.com/problems/largest-subarray-length-k/) 🔒
- [3596. Minimum Cost Path with Alternating Directions I](https://leetcode.com/problems/minimum-cost-path-with-alternating-directions-i/) 🔒
- [3496. Maximize Score After Pair Deletions](https://leetcode.com/problems/maximize-score-after-pair-deletions/) 🔒
- [3125. Maximum Number That Makes Result of Bitwise AND Zero](https://leetcode.com/problems/maximum-number-that-makes-result-of-bitwise-and-zero/) 🔒
- [1794. Count Pairs of Equal Substrings With Minimum Difference](https://leetcode.com/problems/count-pairs-of-equal-substrings-with-minimum-difference/) 🔒

### §5.3 Equivalent Transformation

- [453. Minimum Moves to Equal Array Elements](https://leetcode.com/problems/minimum-moves-to-equal-array-elements/)
- [3375. Minimum Operations to Make Array Values Equal to K](https://leetcode.com/problems/minimum-operations-to-make-array-values-equal-to-k/) 1383
- [2840. Check if Strings Can be Made Equal With Operations II](https://leetcode.com/problems/check-if-strings-can-be-made-equal-with-operations-ii/) 1486
- [2914. Minimum Number of Changes to Make Binary String Beautiful](https://leetcode.com/problems/minimum-number-of-changes-to-make-binary-string-beautiful/) 1480
- [3365. Rearrange K Substrings to Form Target String](https://leetcode.com/problems/rearrange-k-substrings-to-form-target-string/) 1514
- [1657. Determine if Two Strings Are Close](https://leetcode.com/problems/determine-if-two-strings-are-close/) 1530
- [3868. Minimum Cost to Equalize Arrays Using Swaps](https://leetcode.com/problems/minimum-cost-to-equalize-arrays-using-swaps/) 1579
- [3857. Minimum Cost to Split Into Ones](https://leetcode.com/problems/minimum-cost-to-split-into-ones/) (achieve O(1))
- [2551. Put Marbles in Bags](https://leetcode.com/problems/put-marbles-in-bags/) 2042
- [391. Perfect Rectangle](https://leetcode.com/problems/perfect-rectangle/)
- [1585. Check If String Is Transformable With Substring Sort Operations](https://leetcode.com/problems/check-if-string-is-transformable-with-substring-sort-operations/) 2333
- [1040. Moving Stones Until Consecutive II](https://leetcode.com/problems/moving-stones-until-consecutive-ii/) 2456
- [1622. Fancy Sequence](https://leetcode.com/problems/fancy-sequence/) 2476
- [249. Group Shifted Strings](https://leetcode.com/problems/group-shifted-strings/) 🔒
- [49. Group Anagrams](https://leetcode.com/problems/group-anagrams/)
- [1183. Maximum Number of Ones](https://leetcode.com/problems/maximum-number-of-ones/) 🔒

### §5.4 Reverse Thinking

- [2139. Minimum Moves to Reach Target Score](https://leetcode.com/problems/minimum-moves-to-reach-target-score/) 1417
- [3779. Minimum Number of Operations to Have Distinct Elements](https://leetcode.com/problems/minimum-number-of-operations-to-have-distinct-elements/) 1444
- [3396. Minimum Number of Operations to Make Elements in Array Distinct](https://leetcode.com/problems/minimum-number-of-operations-to-make-elements-in-array-distinct/) (same as 3779)
- [3147. Taking Maximum Energy From the Mystic Dungeon](https://leetcode.com/problems/taking-maximum-energy-from-the-mystic-dungeon/) 1460
- [869. Reordered Power of 2](https://leetcode.com/problems/reordered-power-of-2/) 1505
- [1558. Minimum Numbers of Function Calls to Make Target Array](https://leetcode.com/problems/minimum-numbers-of-function-calls-to-make-target-array/) 1637
- [554. Brick Wall](https://leetcode.com/problems/brick-wall/) ~1700
- [780. Reaching Points](https://leetcode.com/problems/reaching-points/) 1897
- [417. Pacific Atlantic Water Flow](https://leetcode.com/problems/pacific-atlantic-water-flow/) ~1900
- [991. Broken Calculator](https://leetcode.com/problems/broken-calculator/) 1909
- [2227. Encrypt and Decrypt Strings](https://leetcode.com/problems/encrypt-and-decrypt-strings/) 1945
- [1354. Construct Target Array With Multiple Sums](https://leetcode.com/problems/construct-target-array-with-multiple-sums/) 2015
- [2543. Check if Point Is Reachable](https://leetcode.com/problems/check-if-point-is-reachable/) 2221
- [3307. Find the K-th Character in String Game II](https://leetcode.com/problems/find-the-k-th-character-in-string-game-ii/) 2232
- [3614. Process String With Special Operations II](https://leetcode.com/problems/process-string-with-special-operations-ii/) (a strengthened version of the previous problem)
- [3419. Minimize the Maximum Edge Weight of Graph](https://leetcode.com/problems/minimize-the-maximum-edge-weight-of-graph/) 2243
- [1611. Minimum One Bit Operations to Make Integers Zero](https://leetcode.com/problems/minimum-one-bit-operations-to-make-integers-zero/) 2345
- [3609. Minimum Moves to Reach Target in Grid](https://leetcode.com/problems/minimum-moves-to-reach-target-in-grid/) 2419
- [936. Stamping the Sequence](https://leetcode.com/problems/stamping-the-sequence/) 2583
- [782. Transform to Chessboard](https://leetcode.com/problems/transform-to-chessboard/)
- [683. K Empty Slots](https://leetcode.com/problems/k-empty-slots/) 🔒 (achieve O(n))
- [3141. Maximum Hamming Distances](https://leetcode.com/problems/maximum-hamming-distances/) 🔒

**Turning Back Time**:

- [3607. Power Grid Maintenance](https://leetcode.com/problems/power-grid-maintenance/) 1700
- [2718. Sum of Matrix After Queries](https://leetcode.com/problems/sum-of-matrix-after-queries/) 1769
- [3639. Minimum Time to Activate String](https://leetcode.com/problems/minimum-time-to-activate-string/) 1853
- [1970. Last Day Where You Can Still Cross](https://leetcode.com/problems/last-day-where-you-can-still-cross/) 2124
- [2382. Maximum Segment Sum After Removals](https://leetcode.com/problems/maximum-segment-sum-after-removals/) 2136
- [803. Bricks Falling When Hit](https://leetcode.com/problems/bricks-falling-when-hit/) 2765

### §5.5 Contribution Technique

- [3871. Count Commas in Range II](https://leetcode.com/problems/count-commas-in-range-ii/) 1381
- [2063. Vowels of All Substrings](https://leetcode.com/problems/vowels-of-all-substrings/) 1663
- [979. Distribute Coins in Binary Tree](https://leetcode.com/problems/distribute-coins-in-binary-tree/) 1709
- [1588. Sum of All Odd Length Subarrays](https://leetcode.com/problems/sum-of-all-odd-length-subarrays/) (achieve O(n))
- [3771. Total Score of Dungeon Runs](https://leetcode.com/problems/total-score-of-dungeon-runs/) 1981
- [2477. Minimum Fuel Cost to Report to the Capital](https://leetcode.com/problems/minimum-fuel-cost-to-report-to-the-capital/) 2012
- [2681. Power of Heroes](https://leetcode.com/problems/power-of-heroes/) 2060
- [3855. Sum of K-Digit Numbers in a Range](https://leetcode.com/problems/sum-of-k-digit-numbers-in-a-range/) 2085
- [3786. Total Sum of Interaction Cost in Tree Groups](https://leetcode.com/problems/total-sum-of-interaction-cost-in-tree-groups/) 2139
- [891. Sum of Subsequence Widths](https://leetcode.com/problems/sum-of-subsequence-widths/) 2183
- [3428. Maximum and Minimum Sums of At Most Size K Subsequences](https://leetcode.com/problems/maximum-and-minimum-sums-of-at-most-size-k-subsequences/) (an advanced version of 891)
- [3426. Manhattan Distances of All Arrangements of Pieces](https://leetcode.com/problems/manhattan-distances-of-all-arrangements-of-pieces/) 2443
- [2763. Sum of Imbalance Numbers of All Subarrays](https://leetcode.com/problems/sum-of-imbalance-numbers-of-all-subarrays/) (an O(n) approach exists, ~2700)

See also "III. Contribution Technique" in the [Monotonic Stack list](https://leetcode.cn/circle/discuss/9oZFK9/).

### §5.6 Two-Pass Scan

Scan once from left to right, then once from right to left.

- [135. Candy](https://leetcode.com/problems/candy/)
- [3796. Find Maximum Value in a Constrained Sequence](https://leetcode.com/problems/find-maximum-value-in-a-constrained-sequence/) 1833
- [3494. Find the Minimum Amount of Time to Brew Potions](https://leetcode.com/problems/find-the-minimum-amount-of-time-to-brew-potions/) 2042
- [1840. Maximum Building Height](https://leetcode.com/problems/maximum-building-height/) 2374

### §5.7 Case Analysis

- [2525. Categorize Box According to Criteria](https://leetcode.com/problems/categorize-box-according-to-criteria/) 1301
- [860. Lemonade Change](https://leetcode.com/problems/lemonade-change/)
- [2165. Smallest Value of the Rearranged Number](https://leetcode.com/problems/smallest-value-of-the-rearranged-number/) 1362
- [2091. Removing Minimum and Maximum From Array](https://leetcode.com/problems/removing-minimum-and-maximum-from-array/) 1384
- [2078. Two Furthest Houses With Different Colors](https://leetcode.com/problems/two-furthest-houses-with-different-colors/) (non-brute-force)
- [1033. Moving Stones Until Consecutive](https://leetcode.com/problems/moving-stones-until-consecutive/) 1421
- [3876. Construct Uniform Parity Array II](https://leetcode.com/problems/construct-uniform-parity-array-ii/) 1444
- [2918. Minimum Equal Sum of Two Arrays After Replacing Zeros](https://leetcode.com/problems/minimum-equal-sum-of-two-arrays-after-replacing-zeros/) 1526
- [2591. Distribute Money to Maximum Children](https://leetcode.com/problems/distribute-money-to-maximum-children/) 1531
- [2131. Longest Palindrome by Concatenating Two Letter Words](https://leetcode.com/problems/longest-palindrome-by-concatenating-two-letter-words/) 1557
- [3789. Minimum Cost to Acquire Required Items](https://leetcode.com/problems/minimum-cost-to-acquire-required-items/) 1580
- [2844. Minimum Operations to Make a Special Number](https://leetcode.com/problems/minimum-operations-to-make-a-special-number/) 1588
- [1247. Minimum Swaps to Make Strings Equal](https://leetcode.com/problems/minimum-swaps-to-make-strings-equal/) 1597
- [838. Push Dominoes](https://leetcode.com/problems/push-dominoes/) 1638
- [2170. Minimum Operations to Make the Array Alternating](https://leetcode.com/problems/minimum-operations-to-make-the-array-alternating/) 1663
- [2202. Maximize the Topmost Element After K Moves](https://leetcode.com/problems/maximize-the-topmost-element-after-k-moves/) 1717
- [2982. Find Longest Special Substring That Occurs Thrice II](https://leetcode.com/problems/find-longest-special-substring-that-occurs-thrice-ii/) 1773
- [3724. Minimum Operations to Transform Array](https://leetcode.com/problems/minimum-operations-to-transform-array/) 1790 (see my solution for a variant of this problem)
- [3001. Minimum Moves to Capture The Queen](https://leetcode.com/problems/minimum-moves-to-capture-the-queen/) 1797
- [2423. Remove Letter To Equalize Frequency](https://leetcode.com/problems/remove-letter-to-equalize-frequency/) (non-brute-force)
- [2934. Minimum Operations to Maximize Last Elements in Arrays](https://leetcode.com/problems/minimum-operations-to-maximize-last-elements-in-arrays/) 1803
- [3800. Minimum Cost to Make Two Binary Strings Equal](https://leetcode.com/problems/minimum-cost-to-make-two-binary-strings-equal/) 1841
- [2162. Minimum Cost to Set Cooking Time](https://leetcode.com/problems/minimum-cost-to-set-cooking-time/) 1852
- [3863. Minimum Operations to Sort a String](https://leetcode.com/problems/minimum-operations-to-sort-a-string/) 1860
- [3440. Reschedule Meetings for Maximum Free Time II](https://leetcode.com/problems/reschedule-meetings-for-maximum-free-time-ii/) 1998
- [3886. Sum of Sortable Integers](https://leetcode.com/problems/sum-of-sortable-integers/) 1999
- [2508. Add Edges to Make Degrees of All Nodes Even](https://leetcode.com/problems/add-edges-to-make-degrees-of-all-nodes-even/) 2060
- [3240. Minimum Number of Flips to Make Binary Grid Palindromic II](https://leetcode.com/problems/minimum-number-of-flips-to-make-binary-grid-palindromic-ii/) 2080
- [3854. Minimum Operations to Make Array Parity Alternating](https://leetcode.com/problems/minimum-operations-to-make-array-parity-alternating/) 2095
- [3548. Equal Sum Grid Partition II](https://leetcode.com/problems/equal-sum-grid-partition-ii/) 2245
- [2468. Split Message Based on Limit](https://leetcode.com/problems/split-message-based-on-limit/) 2382
- [420. Strong Password Checker](https://leetcode.com/problems/strong-password-checker/)
- [3609. Minimum Moves to Reach Target in Grid](https://leetcode.com/problems/minimum-moves-to-reach-target-in-grid/) 2419
- [1040. Moving Stones Until Consecutive II](https://leetcode.com/problems/moving-stones-until-consecutive-ii/) 2456
- [335. Self Crossing](https://leetcode.com/problems/self-crossing/)
- [1330. Reverse Subarray To Maximize Array Value](https://leetcode.com/problems/reverse-subarray-to-maximize-array-value/) 2482
- [3197. Find the Minimum Area to Cover All Ones II](https://leetcode.com/problems/find-the-minimum-area-to-cover-all-ones-ii/) 2541
- [3366. Minimum Array Sum](https://leetcode.com/problems/minimum-array-sum/) (achieve O(n log n))
- [2499. Minimum Total Cost to Make Arrays Unequal](https://leetcode.com/problems/minimum-total-cost-to-make-arrays-unequal/) 2633
- [3311. Construct 2D Grid Matching Graph Layout](https://leetcode.com/problems/construct-2d-grid-matching-graph-layout/) 2664
- [3139. Minimum Cost to Equalize Array](https://leetcode.com/problems/minimum-cost-to-equalize-array/) 2666
- [3017. Count the Number of Houses at a Certain Distance II](https://leetcode.com/problems/count-the-number-of-houses-at-a-certain-distance-ii/) 2709
- [2983. Palindrome Rearrangement Queries](https://leetcode.com/problems/palindrome-rearrangement-queries/) 2780
- [3395. Subsequences with a Unique Middle Mode I](https://leetcode.com/problems/subsequences-with-a-unique-middle-mode-i/) 2800
- [3357. Minimize the Maximum Adjacent Element Difference](https://leetcode.com/problems/minimize-the-maximum-adjacent-element-difference/) 3077
- [1900. The Earliest and Latest Rounds Where Players Compete](https://leetcode.com/problems/the-earliest-and-latest-rounds-where-players-compete/) (achieve O(log n) or O(1))
- [LCP 48. Infinite Chessboard](https://leetcode.cn/problems/fsa7oZ/)
- [LCP 21. Chase Game](https://leetcode.cn/problems/Za25hA/)

## VI. Construction Problems

**Construction problems** give some constraints, and we need to construct an array/string/etc. that **satisfies these constraints**.

The way of thinking is the same as the "Thinking Checklist" in Chapter V — look for inspiration in special cases.

- [1304. Find N Unique Integers Sum up to Zero](https://leetcode.com/problems/find-n-unique-integers-sum-up-to-zero/) 1167
- [942. DI String Match](https://leetcode.com/problems/di-string-match/) 1444
- [1968. Array With Elements Not Equal to Average of Neighbors](https://leetcode.com/problems/array-with-elements-not-equal-to-average-of-neighbors/) 1499 (more than one approach exists — see [my comment](https://leetcode.com/problems/array-with-elements-not-equal-to-average-of-neighbors/solutions/936697/gou-zao-yuan-su-bu-deng-yu-liang-xiang-l-u6vz/comments/1081404) under the official solution)
- [1253. Reconstruct a 2-Row Binary Matrix](https://leetcode.com/problems/reconstruct-a-2-row-binary-matrix/) 1506
- [1317. Convert Integer to the Sum of Two No-Zero Integers](https://leetcode.com/problems/convert-integer-to-the-sum-of-two-no-zero-integers/) (achieve O(log n); follow-up: minimize a)
- [3513. Number of Unique XOR Triplets I](https://leetcode.com/problems/number-of-unique-xor-triplets-i/) 1663
- [2182. Construct String With Repeat Limit](https://leetcode.com/problems/construct-string-with-repeat-limit/) 1680
- [3592. Inverse Coin Change](https://leetcode.com/problems/inverse-coin-change/) 1701
- [969. Pancake Sorting](https://leetcode.com/problems/pancake-sorting/) ~1800
- [406. Queue Reconstruction by Height](https://leetcode.com/problems/queue-reconstruction-by-height/)
- [1605. Find Valid Matrix Given Row and Column Sums](https://leetcode.com/problems/find-valid-matrix-given-row-and-column-sums/) 1868 (northwest corner method)
- [2375. Construct Smallest Number From DI String](https://leetcode.com/problems/construct-smallest-number-from-di-string/) (achieve O(n))
- [324. Wiggle Sort II](https://leetcode.com/problems/wiggle-sort-ii/) ~2000
- [667. Beautiful Arrangement II](https://leetcode.com/problems/beautiful-arrangement-ii/) ~2100
- [2122. Recover the Original Array](https://leetcode.com/problems/recover-the-original-array/) 2159
- [1980. Find Unique Binary String](https://leetcode.com/problems/find-unique-binary-string/) (achieve O(n))
- [3680. Generate Schedule](https://leetcode.com/problems/generate-schedule/) 2378
- [932. Beautiful Array](https://leetcode.com/problems/beautiful-array/) ~2500
- [2790. Maximum Number of Groups With Increasing Length](https://leetcode.com/problems/maximum-number-of-groups-with-increasing-length/) 2620
- [3311. Construct 2D Grid Matching Graph Layout](https://leetcode.com/problems/construct-2d-grid-matching-graph-layout/) 2664
- [2573. Find the String with LCP](https://leetcode.com/problems/find-the-string-with-lcp/) 2682
- [1982. Find Array Given Subset Sums](https://leetcode.com/problems/find-array-given-subset-sums/) 2872
- [280. Wiggle Sort](https://leetcode.com/problems/wiggle-sort/) 🔒
- [484. Find Permutation](https://leetcode.com/problems/find-permutation/) 🔒

For more construction problems, search [constructive algorithms](https://codeforces.com/problemset?order=BY_SOLVED_DESC&tags=constructive+algorithms,900-) on Codeforces.

## VII. Interactive Problems

- [278. First Bad Version](https://leetcode.com/problems/first-bad-version/)
- [374. Guess Number Higher or Lower](https://leetcode.com/problems/guess-number-higher-or-lower/)
- [1237. Find Positive Integer Solution for a Given Equation](https://leetcode.com/problems/find-positive-integer-solution-for-a-given-equation/) (non-brute-force)
- [1095. Find in Mountain Array](https://leetcode.com/problems/find-in-mountain-array/) 1827
- [843. Guess the Word](https://leetcode.com/problems/guess-the-word/) 2078
- [2728. Count Houses in a Circular Street](https://leetcode.com/problems/count-houses-in-a-circular-street/) 🔒
- [277. Find the Celebrity](https://leetcode.com/problems/find-the-celebrity/) 🔒
- [2782. Number of Unique Categories](https://leetcode.com/problems/number-of-unique-categories/) 🔒
- [3064. Guess the Number Using Bitwise Questions I](https://leetcode.com/problems/guess-the-number-using-bitwise-questions-i/) 🔒
- [3094. Guess the Number Using Bitwise Questions II](https://leetcode.com/problems/guess-the-number-using-bitwise-questions-ii/) 🔒
- [1428. Leftmost Column with at Least a One](https://leetcode.com/problems/leftmost-column-with-at-least-a-one/) 🔒
- [702. Search in a Sorted Array of Unknown Size](https://leetcode.com/problems/search-in-a-sorted-array-of-unknown-size/) 🔒
- [1533. Find the Index of the Large Integer](https://leetcode.com/problems/find-the-index-of-the-large-integer/) 🔒
- [2936. Number of Equal Numbers Blocks](https://leetcode.com/problems/number-of-equal-numbers-blocks/) 🔒
- [1618. Maximum Font to Fit a Sentence in a Screen](https://leetcode.com/problems/maximum-font-to-fit-a-sentence-in-a-screen/) 🔒
- [1538. Guess the Majority in a Hidden Array](https://leetcode.com/problems/guess-the-majority-in-a-hidden-array/) 🔒
- [489. Robot Room Cleaner](https://leetcode.com/problems/robot-room-cleaner/) 🔒
- [1778. Shortest Path in a Hidden Grid](https://leetcode.com/problems/shortest-path-in-a-hidden-grid/) 🔒
- [1810. Minimum Path Cost in a Hidden Grid](https://leetcode.com/problems/minimum-path-cost-in-a-hidden-grid/) 🔒
- [1274. Number of Ships in a Rectangle](https://leetcode.com/problems/number-of-ships-in-a-rectangle/) 🔒

## VIII. Others

- [2740. Find the Value of the Partition](https://leetcode.com/problems/find-the-value-of-the-partition/) 1302
- [2946. Matrix Similarity After Cyclic Shifts](https://leetcode.com/problems/matrix-similarity-after-cyclic-shifts/) 1406 (conclusion-based)
- [3523. Make Array Non-decreasing](https://leetcode.com/problems/make-array-non-decreasing/) 1435 (the conclusion is easy to guess — how do you prove it?)
- [781. Rabbits in Forest](https://leetcode.com/problems/rabbits-in-forest/) 1453 (a logical reasoning problem)
- [1041. Robot Bounded in Circle](https://leetcode.com/problems/robot-bounded-in-circle/) 1521 (how do you prove the conclusion?)
- [3587. Minimum Adjacent Swaps to Alternate Parity](https://leetcode.com/problems/minimum-adjacent-swaps-to-alternate-parity/) 1548
- [1864. Minimum Number of Swaps to Make the Binary String Alternating](https://leetcode.com/problems/minimum-number-of-swaps-to-make-the-binary-string-alternating/) 1601
- [1899. Merge Triplets to Form Target Triplet](https://leetcode.com/problems/merge-triplets-to-form-target-triplet/) 1636
- [2498. Frog Jump II](https://leetcode.com/problems/frog-jump-ii/) 1759
- [134. Gas Station](https://leetcode.com/problems/gas-station/)
- [3443. Maximum Manhattan Distance After K Changes](https://leetcode.com/problems/maximum-manhattan-distance-after-k-changes/) 1856
- [3635. Earliest Finish Time for Land and Water Rides II](https://leetcode.com/problems/earliest-finish-time-for-land-and-water-rides-ii/) 1870
- [3002. Maximum Size of a Set After Removals](https://leetcode.com/problems/maximum-size-of-a-set-after-removals/) 1917
- [1733. Minimum Number of People to Teach](https://leetcode.com/problems/minimum-number-of-people-to-teach/) 1984
- [659. Split Array into Consecutive Subsequences](https://leetcode.com/problems/split-array-into-consecutive-subsequences/) ~2100
- [2732. Find a Good Subset of the Matrix](https://leetcode.com/problems/find-a-good-subset-of-the-matrix/) 2240 (note the data range)
- [3474. Lexicographically Smallest Generated String](https://leetcode.com/problems/lexicographically-smallest-generated-string/) 2605 (the conclusion is easy to guess — how do you prove it?)
- [LCP 03. Programmable Robot](https://leetcode.cn/problems/programmable-robot/)
- [LCP 26. Navigation Device](https://leetcode.cn/problems/hSRGyL/)
- [LCP 70. Sand Land Management](https://leetcode.cn/problems/XxZZjK/)
- [2340. Minimum Adjacent Swaps to Make a Valid Array](https://leetcode.com/problems/minimum-adjacent-swaps-to-make-a-valid-array/) 🔒
- [3460. Longest Common Prefix After at Most One Removal](https://leetcode.com/problems/longest-common-prefix-after-at-most-one-removal/) 🔒 (proof)
- [2753. Count Houses in a Circular Street II](https://leetcode.com/problems/count-houses-in-a-circular-street-ii/) 🔒

## Q&A

**Q**: What's the difference between greedy and DP?

**A**: DP can be viewed as memoized brute-force search — as long as no branch is missed, the answer is guaranteed correct. Greedy can be viewed as pruned search: if the greedy strategy is wrong, it's easy to over-prune and cut off the correct branch.

**Q**: Is there a universal method to determine whether a problem should be solved with greedy or DP?

**A**: It's hard. Many people mistake a DP problem for a greedy one if they don't recognize the problem type in advance. My suggestion is to **think about whether DP works first, then consider greedy**. If the DP's time complexity is efficient enough to pass, there's no need to think about a greedy strategy.

This also reveals a downside of practicing by topic list: knowing the problem type in advance skips some of the thinking process. How to make up for this? See [How to Practice LeetCode Scientifically](https://leetcode.cn/circle/discuss/RvFUtj/).

## Related Lists

- [Math list](https://leetcode.cn/circle/discuss/IYT3ss/) — the "Game Theory" section.
- [Data Structures list](https://leetcode.cn/circle/discuss/mOr1u6/) — the "Heap" section.
- [Graph list](https://leetcode.cn/circle/discuss/01LUak/) — Dijkstra's algorithm and Kruskal's/Prim's algorithm, both of which are based on the first basic greedy strategy: always pick the smallest number first.

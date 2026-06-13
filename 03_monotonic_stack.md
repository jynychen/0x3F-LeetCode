# Monotonic Stack

Problem list from [0x3F's LeetCode Study Plan](https://leetcode.cn/discuss/post/3579480/) — Monotonic Stack (Rectangle Area / Contribution Technique / Lexicographically Smallest).

## I. Monotonic Stack

### §1.1 Basics

- [739. Daily Temperatures](https://leetcode.com/problems/daily-temperatures/)
- [1475. Final Prices With A Special Discount In A Shop](https://leetcode.com/problems/final-prices-with-a-special-discount-in-a-shop/) (non-brute-force)
- [496. Next Greater Element I](https://leetcode.com/problems/next-greater-element-i/)
- [503. Next Greater Element II](https://leetcode.com/problems/next-greater-element-ii/)
- [901. Online Stock Span](https://leetcode.com/problems/online-stock-span/) 1709
- [853. Car Fleet](https://leetcode.com/problems/car-fleet/)

### §1.2 Advanced

- [1019. Next Greater Node In Linked List](https://leetcode.com/problems/next-greater-node-in-linked-list/) 1571
- [654. Maximum Binary Tree](https://leetcode.com/problems/maximum-binary-tree/) (O(n) required)
- [768. Max Chunks To Make Sorted II](https://leetcode.com/problems/max-chunks-to-make-sorted-ii/) 1788
- [3814. Maximum Capacity Within Budget](https://leetcode.com/problems/maximum-capacity-within-budget/) 1796
- [3676. Count Bowl Subarrays](https://leetcode.com/problems/count-bowl-subarrays/) 1848
- [2054. Two Best Non-Overlapping Events](https://leetcode.com/problems/two-best-non-overlapping-events/) 1883
- [456. 132 Pattern](https://leetcode.com/problems/132-pattern/) ~2000
- [3113. Find The Number Of Subarrays Where Boundary Elements Are Maximum](https://leetcode.com/problems/find-the-number-of-subarrays-where-boundary-elements-are-maximum/) 2046
- [2866. Beautiful Towers II](https://leetcode.com/problems/beautiful-towers-ii/) 2072
- [975. Odd Even Jump](https://leetcode.com/problems/odd-even-jump/) 2079
- [1944. Number Of Visible People In A Queue](https://leetcode.com/problems/number-of-visible-people-in-a-queue/) 2105
- [2454. Next Greater Element IV](https://leetcode.com/problems/next-greater-element-iv/) 2175
- [1130. Minimum Cost Tree From Leaf Values](https://leetcode.com/problems/minimum-cost-tree-from-leaf-values/) (O(n) required)
- [2289. Steps To Make Array Non-Decreasing](https://leetcode.com/problems/steps-to-make-array-non-decreasing/) 2482
- [1776. Car Fleet II](https://leetcode.com/problems/car-fleet-ii/) 2531
- [2736. Maximum Sum Queries](https://leetcode.com/problems/maximum-sum-queries/) 2533
- [3420. Count Non-Decreasing Subarrays After K Operations](https://leetcode.com/problems/count-non-decreasing-subarrays-after-k-operations/) 2855 (tree structure)
- [3221. Maximum Array Hopping Score II](https://leetcode.com/problems/maximum-array-hopping-score-ii/) 🔒
- [1966. Binary Searchable Numbers In An Unsorted Array](https://leetcode.com/problems/binary-searchable-numbers-in-an-unsorted-array/) 🔒
- [2832. Maximal Range That Each Element Is Maximum In It](https://leetcode.com/problems/maximal-range-that-each-element-is-maximum-in-it/) 🔒
- [1063. Number Of Valid Subarrays](https://leetcode.com/problems/number-of-valid-subarrays/) 🔒
- [1950. Maximum Of Minimum Values In All Subarrays](https://leetcode.com/problems/maximum-of-minimum-values-in-all-subarrays/) 🔒
- [2282. Number Of People That Can Be Seen In A Grid](https://leetcode.com/problems/number-of-people-that-can-be-seen-in-a-grid/) 🔒
- [3555. Smallest Subarray To Sort In Every Sliding Window](https://leetcode.com/problems/smallest-subarray-to-sort-in-every-sliding-window/) 🔒 (non-brute-force)
- [2355. Maximum Number Of Books You Can Take](https://leetcode.com/problems/maximum-number-of-books-you-can-take/) 🔒

**Mind Extensions**:

- [962. Maximum Width Ramp](https://leetcode.com/problems/maximum-width-ramp/) 1608
- [3542. Minimum Operations To Convert All Elements To Zero](https://leetcode.com/problems/minimum-operations-to-convert-all-elements-to-zero/) 1890
- [1124. Longest Well-Performing Interval](https://leetcode.com/problems/longest-well-performing-interval/) 1908
- [1340. Jump Game V](https://leetcode.com/problems/jump-game-v/) (O(n) required)
- [2863. Maximum Length Of Semi-Decreasing Subarrays](https://leetcode.com/problems/maximum-length-of-semi-decreasing-subarrays/) 🔒

## II. Rectangle

- [84. Largest Rectangle In Histogram](https://leetcode.com/problems/largest-rectangle-in-histogram/)
- [1793. Maximum Score Of A Good Subarray](https://leetcode.com/problems/maximum-score-of-a-good-subarray/) 1946
- [85. Maximal Rectangle](https://leetcode.com/problems/maximal-rectangle/)
- [221. Maximal Square](https://leetcode.com/problems/maximal-square/)
- [42. Trapping Rain Water](https://leetcode.com/problems/trapping-rain-water/) (multiple approaches)
- [1504. Count Submatrices With All Ones](https://leetcode.com/problems/count-submatrices-with-all-ones/)
- [1277. Count Square Submatrices With All Ones](https://leetcode.com/problems/count-square-submatrices-with-all-ones/)
- [755. Pour Water](https://leetcode.com/problems/pour-water/) 🔒

**Mind Extensions**:

- [1727. Largest Submatrix With Rearrangements](https://leetcode.com/problems/largest-submatrix-with-rearrangements/) 1927 (not monotonic stack, but shares similar ideas)

## III. Contribution Technique

- [907. Sum Of Subarray Minimums](https://leetcode.com/problems/sum-of-subarray-minimums/) 1976
- [2104. Sum Of Subarray Ranges](https://leetcode.com/problems/sum-of-subarray-ranges/) (max − min; O(n) approach ~2000)
- [1856. Maximum Subarray Min-Product](https://leetcode.com/problems/maximum-subarray-min-product/) 2051
- [3878. Count Good Subarrays](https://leetcode.com/problems/count-good-subarrays/) 2230
- [2818. Apply Operations To Maximize Score](https://leetcode.com/problems/apply-operations-to-maximize-score/) 2397
- [2281. Sum Of Total Strength Of Wizards](https://leetcode.com/problems/sum-of-total-strength-of-wizards/) (min × sum) 2621
- [3430. Maximum And Minimum Sums Of At Most Size K Subarrays](https://leetcode.com/problems/maximum-and-minimum-sums-of-at-most-size-k-subarrays/) 2645
- [3359. Find Sorted Submatrices With Maximum Element At Most K](https://leetcode.com/problems/find-sorted-submatrices-with-maximum-element-at-most-k/) 🔒 (rectangle)

**Mind Extensions**:

- [2334. Subarray With Elements Greater Than Varying Threshold](https://leetcode.com/problems/subarray-with-elements-greater-than-varying-threshold/) 2381
- [2962. Count Subarrays Where Max Element Appears At Least K Times](https://leetcode.com/problems/count-subarrays-where-max-element-appears-at-least-k-times/) (thinking exercise)

## IV. Lexicographically Smallest

- [402. Remove K Digits](https://leetcode.com/problems/remove-k-digits/) ~1800
- [1673. Find The Most Competitive Subsequence](https://leetcode.com/problems/find-the-most-competitive-subsequence/) 1802
- [316. Remove Duplicate Letters](https://leetcode.com/problems/remove-duplicate-letters/) 2185
- [1081. Smallest Subsequence Of Distinct Characters](https://leetcode.com/problems/smallest-subsequence-of-distinct-characters/) (same as 316)
- [3816. Lexicographically Smallest String After Deleting Duplicate Characters](https://leetcode.com/problems/lexicographically-smallest-string-after-deleting-duplicate-characters/) 2377
- [321. Create Maximum Number](https://leetcode.com/problems/create-maximum-number/)
- [2030. Smallest K-Length Subsequence With Occurrences Of A Letter](https://leetcode.com/problems/smallest-k-length-subsequence-with-occurrences-of-a-letter/) 2562

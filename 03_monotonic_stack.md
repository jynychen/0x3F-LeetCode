# Monotonic Stack

> Problem list from [0x3F's LeetCode Problem Lists](https://leetcode.cn/circle/discuss/9oZFK9/)

-----

### §1.1 Basics

Template:

Python3

Java

C++

Go

    def nearestGreater(nums: List[int]) -> Tuple[List[int], List[int]]:
        n = len(nums)
        left = [-1] * n
        st = []
        for i, x in enumerate(nums):
                st.pop()
            if st:
                left[i] = st[-1]
            st.append(i)

        right = [n] * n
        st = []
        for i in range(n - 1, -1, -1):
            x = nums[i]
            while st and nums[st[-1]] <= x:
                st.pop()
            if st:
                right[i] = st[-1]
            st.append(i)

        return left, right

*   [739. Daily Temperatures](https://leetcode.com/problems/daily-temperatures/)
*   [1475. Final Prices with a Special Discount in a Shop](https://leetcode.com/problems/final-prices-with-a-special-discount-in-a-shop/)
*   [496. Next Greater Element I](https://leetcode.com/problems/next-greater-element-i/)
*   [503. Next Greater Element Ii](https://leetcode.com/problems/next-greater-element-ii/)
*   [901. Online Stock Span](https://leetcode.com/problems/online-stock-span/) 1709
*   [853. Car Fleet](https://leetcode.com/problems/car-fleet/)

### §1.2 Advanced（Optional）

*   [1019. Next Greater Node in Linked List](https://leetcode.com/problems/next-greater-node-in-linked-list/) 1571
*   [768. Max Chunks to Make Sorted Ii](https://leetcode.com/problems/max-chunks-to-make-sorted-ii/) 1788
*   [654. Maximum Binary Tree](https://leetcode.com/problems/maximum-binary-tree/)
*   [456. 132 Pattern](https://leetcode.com/problems/132-pattern/) 2000
*   [3113. Find the Number of Subarrays Where Boundary Elements Are Maximum](https://leetcode.com/problems/find-the-number-of-subarrays-where-boundary-elements-are-maximum/) 2046
*   [2866. Beautiful Towers Ii](https://leetcode.com/problems/beautiful-towers-ii/) 2072
*   [1944. Number of Visible People in a Queue](https://leetcode.com/problems/number-of-visible-people-in-a-queue/) 2105
*   [2454. Next Greater Element Iv](https://leetcode.com/problems/next-greater-element-iv/) 2175
*   [1130. Minimum Cost Tree from Leaf Values](https://leetcode.com/problems/minimum-cost-tree-from-leaf-values/) O(n)
*   [2289. Steps to Make Array Non Decreasing](https://leetcode.com/problems/steps-to-make-array-non-decreasing/) 2482
*   [1776. Car Fleet Ii](https://leetcode.com/problems/car-fleet-ii/) 2531
*   [2736. Maximum Sum Queries](https://leetcode.com/problems/maximum-sum-queries/) 2533
*   [3420. Count Non Decreasing Subarrays after K Operations](https://leetcode.com/problems/count-non-decreasing-subarrays-after-k-operations/) 2855
*   [3221. Maximum Array Hopping Score Ii](https://leetcode.com/problems/maximum-array-hopping-score-ii/) (Premium)
*   [1966. Binary Searchable Numbers in an Unsorted Array](https://leetcode.com/problems/binary-searchable-numbers-in-an-unsorted-array/) (Premium)
*   [2832. Maximal Range that Each Element is Maximum in it](https://leetcode.com/problems/maximal-range-that-each-element-is-maximum-in-it/) (Premium)
*   [2282. Number of People that Can Be Seen in a Grid](https://leetcode.com/problems/number-of-people-that-can-be-seen-in-a-grid/) (Premium)
*   [3555. Smallest Subarray to Sort in Every Sliding Window](https://leetcode.com/problems/smallest-subarray-to-sort-in-every-sliding-window/) (Premium)

**Advanced Thinking**:

*   [962. Maximum Width Ramp](https://leetcode.com/problems/maximum-width-ramp/) 1608
*   [3542. Minimum Operations to Convert All Elements to Zero](https://leetcode.com/problems/minimum-operations-to-convert-all-elements-to-zero/) 1890
*   [1124. Longest Well Performing Interval](https://leetcode.com/problems/longest-well-performing-interval/) 1908

## Rectangle
----

*   [84. Largest Rectangle in Histogram](https://leetcode.com/problems/largest-rectangle-in-histogram/)
*   [1793. Maximum Score of a Good Subarray](https://leetcode.com/problems/maximum-score-of-a-good-subarray/) 1946
*   [85. Maximal Rectangle](https://leetcode.com/problems/maximal-rectangle/)
*   [221. Maximal Square](https://leetcode.com/problems/maximal-square/)
*   [42. Trapping Rain Water](https://leetcode.com/problems/trapping-rain-water/)
*   [1504. Count Submatrices with All Ones](https://leetcode.com/problems/count-submatrices-with-all-ones/)
*   [1277. Count Square Submatrices with All Ones](https://leetcode.com/problems/count-square-submatrices-with-all-ones/)
*   [755. Pour Water](https://leetcode.com/problems/pour-water/) (Premium)

## Contribution Method
-----

*   [907. Sum of Subarray Minimums](https://leetcode.com/problems/sum-of-subarray-minimums/) 1976
*   [2104. Sum of Subarray Ranges](https://leetcode.com/problems/sum-of-subarray-ranges/) O(n) 2000
*   [1856. Maximum Subarray Min Product](https://leetcode.com/problems/maximum-subarray-min-product/) 2051
*   [2818. Apply Operations to Maximize Score](https://leetcode.com/problems/apply-operations-to-maximize-score/) 2397
*   [2281. Sum of Total Strength of Wizards](https://leetcode.com/problems/sum-of-total-strength-of-wizards/) 2621
*   [3430. Maximum and Minimum Sums of at Most Size K Subarrays](https://leetcode.com/problems/maximum-and-minimum-sums-of-at-most-size-k-subarrays/) 2645
*   [3359. Find Sorted Submatrices with Maximum Element at Most K](https://leetcode.com/problems/find-sorted-submatrices-with-maximum-element-at-most-k/) (Premium)

**Advanced Thinking**:

*   [2334. Subarray with Elements Greater than Varying Threshold](https://leetcode.com/problems/subarray-with-elements-greater-than-varying-threshold/) 2381
*   [2962. Count Subarrays Where Max Element Appears at Least K Times/solutions/2560940/hua Dong Chuang Kou Fu Ti Dan Pythonjava Xvwg](https://leetcode.com/problems/count-subarrays-where-max-element-appears-at-least-k-times/solutions/2560940/hua-dong-chuang-kou-fu-ti-dan-pythonjava-xvwg/)

## Minimum Lexicographic Order
-------

*   [402. Remove K Digits](https://leetcode.com/problems/remove-k-digits/) 1800
*   [1673. Find the Most Competitive Subsequence](https://leetcode.com/problems/find-the-most-competitive-subsequence/) 1802
*   [316. Remove Duplicate Letters](https://leetcode.com/problems/remove-duplicate-letters/) 2185
*   [316 Extension: Repeat Count at Most limit](https://leetcode.com/contest/tianchi2022/problems/ev2bru/)
*   [1081. Smallest Subsequence of Distinct Characters](https://leetcode.com/problems/smallest-subsequence-of-distinct-characters/)
*   [321. Create Maximum Number](https://leetcode.com/problems/create-maximum-number/)
*   [2030. Smallest K Length Subsequence with Occurrences of a Letter](https://leetcode.com/problems/smallest-k-length-subsequence-with-occurrences-of-a-letter/) 2562


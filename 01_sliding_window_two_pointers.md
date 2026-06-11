# Sliding Window & Two Pointers

> Problem list from [0x3F's LeetCode Problem Lists](https://leetcode.cn/circle/discuss/0viNMK/)


## Fixed-Length Sliding Window

### §1.1 Basics

*   [1456. Maximum Number of Vowels in a Substring of Given Length](https://leetcode.com/problems/maximum-number-of-vowels-in-a-substring-of-given-length/) 1263
*   [643. Maximum Average Subarray I](https://leetcode.com/problems/maximum-average-subarray-i/)
*   [1343. Number of Sub Arrays of Size K and Average Greater than or Equal to Threshold](https://leetcode.com/problems/number-of-sub-arrays-of-size-k-and-average-greater-than-or-equal-to-threshold/) 1317
*   [2090. K Radius Subarray Averages](https://leetcode.com/problems/k-radius-subarray-averages/) 1358
*   [2379. Minimum Recolors to Get K Consecutive Black Blocks](https://leetcode.com/problems/minimum-recolors-to-get-k-consecutive-black-blocks/) 1360
*   [2841. Maximum Sum of Almost Unique Subarray](https://leetcode.com/problems/maximum-sum-of-almost-unique-subarray/) 1546
*   [2461. Maximum Sum of Distinct Subarrays with Length K](https://leetcode.com/problems/maximum-sum-of-distinct-subarrays-with-length-k/) 1553
*   [1423. Maximum Points You Can Obtain from Cards](https://leetcode.com/problems/maximum-points-you-can-obtain-from-cards/) 1574
*   [1176. Diet Plan Performance](https://leetcode.com/problems/diet-plan-performance/) (Premium)
*   [1100. Find K Length Substrings with No Repeated Characters](https://leetcode.com/problems/find-k-length-substrings-with-no-repeated-characters/) (Premium)
*   [1852. Distinct Numbers in Each Subarray](https://leetcode.com/problems/distinct-numbers-in-each-subarray/) (Premium)
*   [1151. Minimum Swaps to Group All 1s Together](https://leetcode.com/problems/minimum-swaps-to-group-all-1s-together/) (Premium)
*   [2107. Number of Unique Flavors after Sharing K Candies](https://leetcode.com/problems/number-of-unique-flavors-after-sharing-k-candies/) (Premium)

### §1.2 Advanced（Optional）

*   [3679. Minimum Discards to Balance Inventory](https://leetcode.com/problems/minimum-discards-to-balance-inventory/) 1639
*   [1052. Grumpy Bookstore Owner](https://leetcode.com/problems/grumpy-bookstore-owner/)
*   [3439. Reschedule Meetings for Maximum Free Time I](https://leetcode.com/problems/reschedule-meetings-for-maximum-free-time-i/) 1729
*   [3694. Distinct Points Reachable after Substring Removal](https://leetcode.com/problems/distinct-points-reachable-after-substring-removal/) 1739
*   [3652. Best Time to Buy and Sell Stock Using Strategy](https://leetcode.com/problems/best-time-to-buy-and-sell-stock-using-strategy/)
*   [2134. Minimum Swaps to Group All 1s Together Ii](https://leetcode.com/problems/minimum-swaps-to-group-all-1s-together-ii/) 1748
*   [1652. Defuse the Bomb](https://leetcode.com/problems/defuse-the-bomb/)
*   [1297. Maximum Number of Occurrences of a Substring](https://leetcode.com/problems/maximum-number-of-occurrences-of-a-substring/) 1748
*   [2653. Sliding Subarray Beauty](https://leetcode.com/problems/sliding-subarray-beauty/) 1786
*   [1888. Minimum Number of Flips to Make the Binary String Alternating](https://leetcode.com/problems/minimum-number-of-flips-to-make-the-binary-string-alternating/) 2006
*   [567. Permutation in String](https://leetcode.com/problems/permutation-in-string/)
*   [438. Find All Anagrams in a String](https://leetcode.com/problems/find-all-anagrams-in-a-string/)
*   [30. Substring with Concatenation of All Words](https://leetcode.com/problems/substring-with-concatenation-of-all-words/)
*   [2156. Find Substring with Given Hash Value](https://leetcode.com/problems/find-substring-with-given-hash-value/) 2063
*   [2953. Count Complete Substrings](https://leetcode.com/problems/count-complete-substrings/) 2449
*   [1016. Binary String with Substrings Representing 1 to N](https://leetcode.com/problems/binary-string-with-substrings-representing-1-to-n/)
*   [3672. Sum of Weighted Modes in Subarrays](https://leetcode.com/problems/sum-of-weighted-modes-in-subarrays/) (Premium)
*   [683. K Empty Slots](https://leetcode.com/problems/k-empty-slots/) (Premium)
*   [2067. Number of Equal Count Substrings](https://leetcode.com/problems/number-of-equal-count-substrings/) (Premium)
*   [2524. Maximum Frequency Score of a Subarray](https://leetcode.com/problems/maximum-frequency-score-of-a-subarray/) (Premium)

### §1.3 Others (Optional)

*   [2200. Find All K Distant Indices in an Array](https://leetcode.com/problems/find-all-k-distant-indices-in-an-array/) 1266
*   [2269. Find the K Beauty of a Number](https://leetcode.com/problems/find-the-k-beauty-of-a-number/) 1280
*   [1984. Minimum Difference Between Highest and Lowest of K Scores](https://leetcode.com/problems/minimum-difference-between-highest-and-lowest-of-k-scores/) 1306
*   [1461. Check If a String Contains All Binary Codes of Size K](https://leetcode.com/problems/check-if-a-string-contains-all-binary-codes-of-size-k/) 1504
*   [220. Contains Duplicate Iii](https://leetcode.com/problems/contains-duplicate-iii/)

## Variable-Length Sliding Window
---------

### §2.1 Shorter is Valid / Find Longest / Maximum

#### §2.1.1 Basics

*   [3. Longest Substring Without Repeating Characters](https://leetcode.com/problems/longest-substring-without-repeating-characters/)
*   [3090. Maximum Length Substring with Two Occurrences](https://leetcode.com/problems/maximum-length-substring-with-two-occurrences/) 1329
*   [1493. Longest Subarray of 1s after Deleting One Element](https://leetcode.com/problems/longest-subarray-of-1s-after-deleting-one-element/) 1423
*   [3634. Minimum Removals to Balance Array](https://leetcode.com/problems/minimum-removals-to-balance-array/) 1453
*   [1208. Get Equal Substrings Within Budget](https://leetcode.com/problems/get-equal-substrings-within-budget/) 1497
*   [904. Fruit Into Baskets](https://leetcode.com/problems/fruit-into-baskets/) 1516
*   [1695. Maximum Erasure Value](https://leetcode.com/problems/maximum-erasure-value/) 1529
*   [2958. Length of Longest Subarray with at Most K Frequency](https://leetcode.com/problems/length-of-longest-subarray-with-at-most-k-frequency/) 1535
*   [2024. Maximize the Confusion of an Exam](https://leetcode.com/problems/maximize-the-confusion-of-an-exam/) 1643
*   [1004. Max Consecutive Ones Iii](https://leetcode.com/problems/max-consecutive-ones-iii/) 1656
*   [1658. Minimum Operations to Reduce X to Zero](https://leetcode.com/problems/minimum-operations-to-reduce-x-to-zero/) 1817
*   [3641. Longest Semi Repeating Subarray](https://leetcode.com/problems/longest-semi-repeating-subarray/) (Premium)

#### §2.1.2 Advanced（Optional）

*   [2730. Find the Longest Semi Repetitive Substring](https://leetcode.com/problems/find-the-longest-semi-repetitive-substring/)
*   [2779. Maximum Beauty of an Array after Applying Operation](https://leetcode.com/problems/maximum-beauty-of-an-array-after-applying-operation/) 1638
*   [1838. Frequency of the Most Frequent Element](https://leetcode.com/problems/frequency-of-the-most-frequent-element/) 1876
*   [2516. Take K of Each Character from Left and Right](https://leetcode.com/problems/take-k-of-each-character-from-left-and-right/) 1948
*   [2831. Find the Longest Equal Subarray](https://leetcode.com/problems/find-the-longest-equal-subarray/) 1976
*   [2271. Maximum White Tiles Covered by a Carpet](https://leetcode.com/problems/maximum-white-tiles-covered-by-a-carpet/) 2022
*   [2106. Maximum Fruits Harvested after at Most K Steps](https://leetcode.com/problems/maximum-fruits-harvested-after-at-most-k-steps/) 2062
*   [2555. Maximize Win from Two Segments](https://leetcode.com/problems/maximize-win-from-two-segments/) 2081
*   [2009. Minimum Number of Operations to Make Array Continuous](https://leetcode.com/problems/minimum-number-of-operations-to-make-array-continuous/) 2084
*   [1610. Maximum Number of Visible Points](https://leetcode.com/problems/maximum-number-of-visible-points/) 2147
*   [2781. Length of the Longest Valid Substring](https://leetcode.com/problems/length-of-the-longest-valid-substring/) 2204
*   [3411. Maximum Subarray with Equal Products](https://leetcode.com/problems/maximum-subarray-with-equal-products/)
*   [3413. Maximum Coins from K Consecutive Bags](https://leetcode.com/problems/maximum-coins-from-k-consecutive-bags/) 2374
*   [395. Longest Substring with at Least K Repeating Characters](https://leetcode.com/problems/longest-substring-with-at-least-k-repeating-characters/)
*   [1763. Longest Nice Substring](https://leetcode.com/problems/longest-nice-substring/)
*   [2968. Apply Operations to Maximize Frequency Score](https://leetcode.com/problems/apply-operations-to-maximize-frequency-score/) 2444
*   [1040. Moving Stones Until Consecutive Ii](https://leetcode.com/problems/moving-stones-until-consecutive-ii/) 2456
*   [487. Max Consecutive Ones Ii](https://leetcode.com/problems/max-consecutive-ones-ii/) (Premium)
*   [159. Longest Substring with at Most Two Distinct Characters](https://leetcode.com/problems/longest-substring-with-at-most-two-distinct-characters/) (Premium)
*   [340. Longest Substring with at Most K Distinct Characters](https://leetcode.com/problems/longest-substring-with-at-most-k-distinct-characters/) (Premium)

### §2.2 Longer is Valid / Find Shortest / Minimum

*   [209. Minimum Size Subarray Sum](https://leetcode.com/problems/minimum-size-subarray-sum/)
*   [3726. Minimum Subarray Length with Distinct Sum at Least K](https://leetcode.com/problems/minimum-subarray-length-with-distinct-sum-at-least-k/)
*   [2904. Shortest and Lexicographically Smallest Beautiful String](https://leetcode.com/problems/shortest-and-lexicographically-smallest-beautiful-string/)
*   [1234. Replace the Substring for Balanced String](https://leetcode.com/problems/replace-the-substring-for-balanced-string/) 1878
*   [2875. Minimum Size Subarray in Infinite Array](https://leetcode.com/problems/minimum-size-subarray-in-infinite-array/) 1914
*   [76. Minimum Window Substring](https://leetcode.com/problems/minimum-window-substring/)
*   [632. Smallest Range Covering Elements from K Lists](https://leetcode.com/problems/smallest-range-covering-elements-from-k-lists/)

### §2.3 Count Subarrays

#### §2.3.1 Shorter is Valid

*   [713. Subarray Product Less than K](https://leetcode.com/problems/subarray-product-less-than-k/)
*   [3258. Count Substrings that Satisfy K Constraint I](https://leetcode.com/problems/count-substrings-that-satisfy-k-constraint-i/)
*   [2302. Count Subarrays with Score Less than K](https://leetcode.com/problems/count-subarrays-with-score-less-than-k/) 1808
*   [2762. Continuous Subarrays](https://leetcode.com/problems/continuous-subarrays/) 1940
*   [LCP 68. 1gxjyy](https://leetcode.com/problems/1GxJYY/)
*   [2743. Count Substrings Without Repeating Character](https://leetcode.com/problems/count-substrings-without-repeating-character/) (Premium)

**Advanced Thinking (Optional)**

*   [3134. Find the Median of the Uniqueness Array](https://leetcode.com/problems/find-the-median-of-the-uniqueness-array/) 2451
*   [3261. Count Substrings that Satisfy K Constraint Ii](https://leetcode.com/problems/count-substrings-that-satisfy-k-constraint-ii/) 2659

#### §2.3.2 Longer is Valid

*   [1358. Number of Substrings Containing All Three Characters](https://leetcode.com/problems/number-of-substrings-containing-all-three-characters/) 1646
*   [2962. Count Subarrays Where Max Element Appears at Least K Times](https://leetcode.com/problems/count-subarrays-where-max-element-appears-at-least-k-times/) 1701
*   [3325. Count Substrings with K Frequency Characters I](https://leetcode.com/problems/count-substrings-with-k-frequency-characters-i/)
*   [2062. Count Vowel Substrings of a String](https://leetcode.com/problems/count-vowel-substrings-of-a-string/)
*   [2799. Count Complete Subarrays in an Array](https://leetcode.com/problems/count-complete-subarrays-in-an-array/)
*   [2537. Count the Number of Good Subarrays](https://leetcode.com/problems/count-the-number-of-good-subarrays/) 1892
*   [3298. Count Substrings that Can Be Rearranged to Contain a String Ii](https://leetcode.com/problems/count-substrings-that-can-be-rearranged-to-contain-a-string-ii/) 1909
*   [2495. Number of Subarrays Having Even Product](https://leetcode.com/problems/number-of-subarrays-having-even-product/) (Premium)

#### §2.3.3 Exact Match Sliding Window

*   Count subarrays with sum ≥k.
*   Count subarrays with sum >k, i.e., ≥k+1.

**Summary**: "Exactly" can be decomposed into two "at least" problems, i.e., two "longer is valid" sliding window problems.

*   [930. Binary Subarrays with Sum](https://leetcode.com/problems/binary-subarrays-with-sum/) 1592
*   [1248. Count Number of Nice Subarrays](https://leetcode.com/problems/count-number-of-nice-subarrays/) 1624
*   [3306. Count of Substrings Containing Every Vowel and K Consonants Ii](https://leetcode.com/problems/count-of-substrings-containing-every-vowel-and-k-consonants-ii/) 2200
*   [992. Subarrays with K Different Integers](https://leetcode.com/problems/subarrays-with-k-different-integers/) 2210
*   [3519. Count Subarrays with K Distinct Integers](https://leetcode.com/problems/count-subarrays-with-k-distinct-integers/) (Premium)

### §2.4 Others (Optional)

*   [825. Friends of Appropriate Ages](https://leetcode.com/problems/friends-of-appropriate-ages/) 1697
*   [2401. Longest Nice Subarray](https://leetcode.com/problems/longest-nice-subarray/) 1750
*   [1156. Swap for Longest Repeated Character Substring](https://leetcode.com/problems/swap-for-longest-repeated-character-substring/) 1787
*   [424. Longest Repeating Character Replacement](https://leetcode.com/problems/longest-repeating-character-replacement/)
*   [438. Find All Anagrams in a String](https://leetcode.com/problems/find-all-anagrams-in-a-string/)
*   [1712. Ways to Split Array Into Three Subarrays](https://leetcode.com/problems/ways-to-split-array-into-three-subarrays/) 2079
*   [LCR 180. He Wei Sde Lian Xu Zheng Shu Xu Lie Lcof](https://leetcode.com/problems/he-wei-sde-lian-xu-zheng-shu-xu-lie-lcof/)
*   [1918. Kth Smallest Subarray Sum](https://leetcode.com/problems/kth-smallest-subarray-sum/) (Premium)

## Single Array Two Pointers

### §3.1 Opposite-Direction Two Pointers

*   [344. Reverse String](https://leetcode.com/problems/reverse-string/)
*   [2000. Reverse String Prefix](https://leetcode.com/problems/reverse-string-prefix/)
*   [2120. Reverse Prefix of Word](https://leetcode.com/problems/reverse-prefix-of-word/)
*   [3643. Flip Square Submatrix Vertically](https://leetcode.com/problems/flip-square-submatrix-vertically/) 1235
*   [832. Flipping an Image](https://leetcode.com/problems/flipping-an-image/)
*   [3734. Reverse Letters Then Special Characters in a String](https://leetcode.com/problems/reverse-letters-then-special-characters-in-a-string/)
*   [541. Reverse String Ii](https://leetcode.com/problems/reverse-string-ii/)
*   [557. Reverse Words in a String Iii](https://leetcode.com/problems/reverse-words-in-a-string-iii/)
*   [151. Reverse Words in a String](https://leetcode.com/problems/reverse-words-in-a-string/)
*   [3738. Reverse Words with Same Vowel Count](https://leetcode.com/problems/reverse-words-with-same-vowel-count/)
*   [345. Reverse Vowels of a String](https://leetcode.com/problems/reverse-vowels-of-a-string/)
*   [3735. Reverse K Subarrays](https://leetcode.com/problems/reverse-k-subarrays/) (Premium)
*   [186. Reverse Words in a String Ii](https://leetcode.com/problems/reverse-words-in-a-string-ii/) (Premium)
*   [2697. Lexicographically Smallest Palindrome](https://leetcode.com/problems/lexicographically-smallest-palindrome/)
*   [917. Reverse Only Letters](https://leetcode.com/problems/reverse-only-letters/)
*   [125. Valid Palindrome](https://leetcode.com/problems/valid-palindrome/)
*   [1750. Minimum Length of String after Deleting Similar Ends](https://leetcode.com/problems/minimum-length-of-string-after-deleting-similar-ends/) 1502
*   [2105. Watering Plants Ii](https://leetcode.com/problems/watering-plants-ii/) 1507
*   [977. Squares of a Sorted Array](https://leetcode.com/problems/squares-of-a-sorted-array/)
*   [658. Find K Closest Elements](https://leetcode.com/problems/find-k-closest-elements/)
*   [1471. The K Strongest Values in an Array](https://leetcode.com/problems/the-k-strongest-values-in-an-array/)
*   [167. Two Sum Ii Input Array is Sorted](https://leetcode.com/problems/two-sum-ii-input-array-is-sorted/)
*   [633. Sum of Square Numbers](https://leetcode.com/problems/sum-of-square-numbers/)
*   [2824. Count Pairs Whose Sum is Less than Target](https://leetcode.com/problems/count-pairs-whose-sum-is-less-than-target/)
*   [2563. Count the Number of Fair Pairs](https://leetcode.com/problems/count-the-number-of-fair-pairs/)
*   [LCP 28. 4xy4wx](https://leetcode.com/problems/4xy4Wx/)
*   [15. 3sum](https://leetcode.com/problems/3sum/)
*   [16. 3sum Closest](https://leetcode.com/problems/3sum-closest/)
*   [18. 4sum](https://leetcode.com/problems/4sum/)
*   [611. Valid Triangle Number](https://leetcode.com/problems/valid-triangle-number/)
*   [1577. Number of Ways Where Square of Number is Equal to Product of Two Numbers](https://leetcode.com/problems/number-of-ways-where-square-of-number-is-equal-to-product-of-two-numbers/)
*   [3728. Find the Smallest Balanced Index](https://leetcode.com/problems/find-the-smallest-balanced-index/)
*   [923. 3sum with Multiplicity](https://leetcode.com/problems/3sum-with-multiplicity/) 1711
*   [948. Bag of Tokens](https://leetcode.com/problems/bag-of-tokens/) 1762
*   [11. Container with Most Water](https://leetcode.com/problems/container-with-most-water/)
*   [42. Trapping Rain Water](https://leetcode.com/problems/trapping-rain-water/)
*   [1616. Split Two Strings to Make Palindrome](https://leetcode.com/problems/split-two-strings-to-make-palindrome/) 1868
*   [1498. Number of Subsequences that Satisfy the Given Sum Condition](https://leetcode.com/problems/number-of-subsequences-that-satisfy-the-given-sum-condition/) 2276
*   [1782. Count Pairs of Nodes](https://leetcode.com/problems/count-pairs-of-nodes/) 2457
*   [1099. Two Sum Less than K](https://leetcode.com/problems/two-sum-less-than-k/) (Premium)
*   [360. Sort Transformed Array](https://leetcode.com/problems/sort-transformed-array/) (Premium)
*   [2422. Merge Operations to Turn Array Into a Palindrome](https://leetcode.com/problems/merge-operations-to-turn-array-into-a-palindrome/) (Premium)
*   [259. 3sum Smaller](https://leetcode.com/problems/3sum-smaller/) (Premium)
*   [3729. Number of Ways to Paint Sheets](https://leetcode.com/problems/number-of-ways-to-paint-sheets/)
*   [1861. Rotating the Box](https://leetcode.com/problems/rotating-the-box/)
*   [3730. Maximum Capacity Within Budget](https://leetcode.com/problems/maximum-capacity-within-budget/)

### §3.2 Same-Direction Two Pointers

*   [611. Valid Triangle Number](https://leetcode.com/problems/valid-triangle-number/)
*   [3649. Number of Perfect Pairs](https://leetcode.com/problems/number-of-perfect-pairs/) 1716
*   [1871. Jump Game Vii](https://leetcode.com/problems/jump-game-vii/)
*   [1574. Shortest Subarray to Be Removed to Make Array Sorted](https://leetcode.com/problems/shortest-subarray-to-be-removed-to-make-array-sorted/) 1932
*   [2972. Count the Number of Incremovable Subarrays Ii](https://leetcode.com/problems/count-the-number-of-incremovable-subarrays-ii/) 2153
*   [2122. Recover the Original Array](https://leetcode.com/problems/recover-the-original-array/) 2159
*   [2234. Maximum Total Beauty of the Gardens](https://leetcode.com/problems/maximum-total-beauty-of-the-gardens/) 2562
*   [1989. Maximum Number of People that Can Be Caught in Tag](https://leetcode.com/problems/maximum-number-of-people-that-can-be-caught-in-tag/) (Premium)
*   [3323. Minimize Connected Groups by Inserting Interval](https://leetcode.com/problems/minimize-connected-groups-by-inserting-interval/) (Premium)

*   [581. Shortest Unsorted Continuous Subarray](https://leetcode.com/problems/shortest-unsorted-continuous-subarray/)
*   [3555. Smallest Subarray to Sort in Every Sliding Window](https://leetcode.com/problems/smallest-subarray-to-sort-in-every-sliding-window/) (Premium)

### §3.3 Expanding Two Pointers

*   [1793. Maximum Score of a Good Subarray](https://leetcode.com/problems/maximum-score-of-a-good-subarray/) 1946
*   [976. Largest Perimeter Triangle](https://leetcode.com/problems/largest-perimeter-triangle/)

### §3.4 In-Place Modification

*   [27. Remove Element](https://leetcode.com/problems/remove-element/)
*   [26. Remove Duplicates from Sorted Array](https://leetcode.com/problems/remove-duplicates-from-sorted-array/)
*   [80. Remove Duplicates from Sorted Array Ii](https://leetcode.com/problems/remove-duplicates-from-sorted-array-ii/)
*   [2273. Find Resultant Array after Removing Anagrams](https://leetcode.com/problems/find-resultant-array-after-removing-anagrams/)
*   [3684. Maximize Sum of at Most K Distinct Elements](https://leetcode.com/problems/maximize-sum-of-at-most-k-distinct-elements/)
*   [283. Move Zeroes](https://leetcode.com/problems/move-zeroes/)
*   [905. Sort Array by Parity](https://leetcode.com/problems/sort-array-by-parity/)
*   [922. Sort Array by Parity Ii](https://leetcode.com/problems/sort-array-by-parity-ii/)
*   [3467. Transform Array by Parity](https://leetcode.com/problems/transform-array-by-parity/)
*   [2460. Apply Operations to an Array](https://leetcode.com/problems/apply-operations-to-an-array/)
*   [1089. Duplicate Zeros](https://leetcode.com/problems/duplicate-zeros/)
*   [75. Sort Colors](https://leetcode.com/problems/sort-colors/)
*   [1752. Check If Array is Good](https://leetcode.com/problems/check-if-array-is-good/)

**Advanced Thinking (Optional)**：

*   [1920. Build Array from Permutation](https://leetcode.com/problems/build-array-from-permutation/)
*   [442. Find All Duplicates in an Array](https://leetcode.com/problems/find-all-duplicates-in-an-array/)
*   [448. Find All Numbers Disappeared in an Array](https://leetcode.com/problems/find-all-numbers-disappeared-in-an-array/)
*   [41. First Missing Positive](https://leetcode.com/problems/first-missing-positive/)
*   [240. Search a 2d Matrix Ii](https://leetcode.com/problems/search-a-2d-matrix-ii/)
*   [1351. Count Negative Numbers in a Sorted Matrix](https://leetcode.com/problems/count-negative-numbers-in-a-sorted-matrix/)

## Two Arrays Two Pointers

### §4.1 Two Pointers

*   [2109. Adding Spaces to a String](https://leetcode.com/problems/adding-spaces-to-a-string/) 1315
*   [2540. Minimum Common Value](https://leetcode.com/problems/minimum-common-value/)
*   [88. Merge Sorted Array](https://leetcode.com/problems/merge-sorted-array/)
*   [2570. Merge Two 2d Arrays by Summing Values](https://leetcode.com/problems/merge-two-2d-arrays-by-summing-values/)
*   [350. Intersection of Two Arrays Ii](https://leetcode.com/problems/intersection-of-two-arrays-ii/)
*   [LCP 18. 2vyngi](https://leetcode.com/problems/2vYnGI/)
*   [1855. Maximum Distance Between a Pair of Values](https://leetcode.com/problems/maximum-distance-between-a-pair-of-values/) 1515
*   [1385. Find the Distance Value Between Two Arrays](https://leetcode.com/problems/find-the-distance-value-between-two-arrays/)
*   [925. Long Pressed Name](https://leetcode.com/problems/long-pressed-name/)
*   [809. Expressive Words](https://leetcode.com/problems/expressive-words/) 1605
*   [2337. Move Pieces to Obtain a String](https://leetcode.com/problems/move-pieces-to-obtain-a-string/) 1693
*   [777. Swap Adjacent in Lr String](https://leetcode.com/problems/swap-adjacent-in-lr-string/)
*   [844. Backspace String Compare](https://leetcode.com/problems/backspace-string-compare/)
*   [986. Interval List Intersections](https://leetcode.com/problems/interval-list-intersections/)
*   [Interview 16.06. Smallest Difference Lcci](https://leetcode.com/problems/smallest-difference-lcci/)
*   [475. Heaters](https://leetcode.com/problems/heaters/)
*   [1537. Get the Maximum Score](https://leetcode.com/problems/get-the-maximum-score/) 1961
*   [244. Shortest Word Distance Ii](https://leetcode.com/problems/shortest-word-distance-ii/) (Premium)
*   [2838. Maximum Coins Heroes Can Collect](https://leetcode.com/problems/maximum-coins-heroes-can-collect/) (Premium)
*   [1229. Meeting Scheduler](https://leetcode.com/problems/meeting-scheduler/) (Premium)
*   [1570. Dot Product of Two Sparse Vectors](https://leetcode.com/problems/dot-product-of-two-sparse-vectors/) (Premium)
*   [1868. Product of Two Run Length Encoded Arrays](https://leetcode.com/problems/product-of-two-run-length-encoded-arrays/) (Premium)

### §4.2 Subsequence Check

*   [392. Is Subsequence](https://leetcode.com/problems/is-subsequence/)
*   [524. Longest Word in Dictionary Through Deleting](https://leetcode.com/problems/longest-word-in-dictionary-through-deleting/)
*   [2486. Append Characters to String to Make Subsequence](https://leetcode.com/problems/append-characters-to-string-to-make-subsequence/) 1363
*   [2825. Make String a Subsequence Using Cyclic Increments](https://leetcode.com/problems/make-string-a-subsequence-using-cyclic-increments/) 1415
*   [1023. Camelcase Matching](https://leetcode.com/problems/camelcase-matching/) 1537
*   [3132. Find the Integer Added to Array Ii](https://leetcode.com/problems/find-the-integer-added-to-array-ii/) 1620
*   [522. Longest Uncommon Subsequence Ii](https://leetcode.com/problems/longest-uncommon-subsequence-ii/) 1700
*   [1826. Faulty Sensor](https://leetcode.com/problems/faulty-sensor/) (Premium)

**Advanced**:

*   [1898. Maximum Number of Removable Characters](https://leetcode.com/problems/maximum-number-of-removable-characters/) 1913
*   [2565. Subsequence with the Minimum Score](https://leetcode.com/problems/subsequence-with-the-minimum-score/) 2432
*   [3302. Find the Lexicographically Smallest Valid Sequence](https://leetcode.com/problems/find-the-lexicographically-smallest-valid-sequence/) 2474

## Three Pointers
-----

*   [2367. Number of Arithmetic Triplets](https://leetcode.com/problems/number-of-arithmetic-triplets/)
*   [2563. Count the Number of Fair Pairs](https://leetcode.com/problems/count-the-number-of-fair-pairs/) 1721
*   [795. Number of Subarrays with Bounded Maximum](https://leetcode.com/problems/number-of-subarrays-with-bounded-maximum/) 1817
*   [2444. Count Subarrays with Fixed Bounds](https://leetcode.com/problems/count-subarrays-with-fixed-bounds/) 2093
*   [3347. Maximum Frequency of an Element after Performing Operations Ii](https://leetcode.com/problems/maximum-frequency-of-an-element-after-performing-operations-ii/) 2156
*   [1213. Intersection of Three Sorted Arrays](https://leetcode.com/problems/intersection-of-three-sorted-arrays/) (Premium)

**Advanced Thinking**:

*   [3464. Maximize the Distance Between Points on a Square](https://leetcode.com/problems/maximize-the-distance-between-points-on-a-square/) 2806

## Group Loop
------

**Use case**: The array is split into groups according to problem requirements, with the same logic applied to each group.

**Core idea**:

*   The outer loop handles preparation before traversing a group (recording start position) and statistics after (updating the answer).
*   The inner loop traverses the group and finds where it ends.

*   [485. Max Consecutive Ones](https://leetcode.com/problems/max-consecutive-ones/)
*   [1446. Consecutive Characters](https://leetcode.com/problems/consecutive-characters/) 1165
*   [1869. Longer Contiguous Segments of Ones than Zeros](https://leetcode.com/problems/longer-contiguous-segments-of-ones-than-zeros/) 1205
*   [2414. Length of the Longest Alphabetical Continuous Substring](https://leetcode.com/problems/length-of-the-longest-alphabetical-continuous-substring/) 1222
*   [3456. Find Special Substring of Length K](https://leetcode.com/problems/find-special-substring-of-length-k/) 1244
*   [830. Positions of Large Groups](https://leetcode.com/problems/positions-of-large-groups/)
*   [2273. Find Resultant Array after Removing Anagrams](https://leetcode.com/problems/find-resultant-array-after-removing-anagrams/) 1295
*   [2264. Largest 3 Same Digit Number in String](https://leetcode.com/problems/largest-3-same-digit-number-in-string/)
*   [2348. Number of Zero Filled Subarrays](https://leetcode.com/problems/number-of-zero-filled-subarrays/) 1316
*   [1513. Number of Substrings with Only 1s](https://leetcode.com/problems/number-of-substrings-with-only-1s/) 1351
*   [1957. Delete Characters to Make Fancy String](https://leetcode.com/problems/delete-characters-to-make-fancy-string/) 1358
*   [674. Longest Continuous Increasing Subsequence](https://leetcode.com/problems/longest-continuous-increasing-subsequence/)
*   [3708. Longest Fibonacci Subarray](https://leetcode.com/problems/longest-fibonacci-subarray/) 1381
*   [696. Count Binary Substrings](https://leetcode.com/problems/count-binary-substrings/)
*   [978. Longest Turbulent Subarray](https://leetcode.com/problems/longest-turbulent-subarray/) 1393
*   [2110. Number of Smooth Descent Periods of a Stock](https://leetcode.com/problems/number-of-smooth-descent-periods-of-a-stock/) 1408
*   [228. Summary Ranges](https://leetcode.com/problems/summary-ranges/)
*   [2760. Longest Even Odd Subarray with Threshold](https://leetcode.com/problems/longest-even-odd-subarray-with-threshold/) 1420
*   [1887. Reduction Operations to Make the Array Elements Equal](https://leetcode.com/problems/reduction-operations-to-make-the-array-elements-equal/) 1428
*   [845. Longest Mountain in Array](https://leetcode.com/problems/longest-mountain-in-array/) 1437
*   [2038. Remove Colored Pieces If Both Neighbors Are the Same Color](https://leetcode.com/problems/remove-colored-pieces-if-both-neighbors-are-the-same-color/) 1468
*   [2900. Longest Unequal Adjacent Groups Subsequence I](https://leetcode.com/problems/longest-unequal-adjacent-groups-subsequence-i/) 1469
*   [1759. Count Number of Homogenous Substrings](https://leetcode.com/problems/count-number-of-homogenous-substrings/) 1491
*   [3011. Find If Array Can Be Sorted](https://leetcode.com/problems/find-if-array-can-be-sorted/) 1497
*   [1861. Rotating the Box](https://leetcode.com/problems/rotating-the-box/)
*   [1578. Minimum Time to Make Rope Colorful](https://leetcode.com/problems/minimum-time-to-make-rope-colorful/) 1574
*   [1839. Longest Substring of All Vowels in Order](https://leetcode.com/problems/longest-substring-of-all-vowels-in-order/) 1580
*   [2765. Longest Alternating Subarray](https://leetcode.com/problems/longest-alternating-subarray/) 1581
*   [3255. Find the Power of K Size Subarrays Ii](https://leetcode.com/problems/find-the-power-of-k-size-subarrays-ii/) 1595
*   [3350. Adjacent Increasing Subarrays Detection Ii](https://leetcode.com/problems/adjacent-increasing-subarrays-detection-ii/) 1600
*   [3105. Longest Strictly Increasing or Strictly Decreasing Subarray](https://leetcode.com/problems/longest-strictly-increasing-or-strictly-decreasing-subarray/)
*   [3737. Count Valid Word Occurrences](https://leetcode.com/problems/count-valid-word-occurrences/)
*   [838. Push Dominoes](https://leetcode.com/problems/push-dominoes/) 1638
*   [467. Unique Substrings in Wraparound String](https://leetcode.com/problems/unique-substrings-in-wraparound-string/) 1700
*   [3499. Maximize Active Section with Trade I](https://leetcode.com/problems/maximize-active-section-with-trade-i/) 1729
*   [413. Arithmetic Slices](https://leetcode.com/problems/arithmetic-slices/)
*   [2771. Longest Non Decreasing Subarray after Replacing at Most One Element](https://leetcode.com/problems/longest-non-decreasing-subarray-after-replacing-at-most-one-element/)
*   [2147. Number of Ways to Divide a Long Corridor](https://leetcode.com/problems/number-of-ways-to-divide-a-long-corridor/)
*   [68. Text Justification](https://leetcode.com/problems/text-justification/)
*   [135. Candy](https://leetcode.com/problems/candy/)
*   [3731. Longest Arithmetic Sequence after Changing at Most One Element](https://leetcode.com/problems/longest-arithmetic-sequence-after-changing-at-most-one-element/)
*   [2948. Make Lexicographically Smallest Array by Swapping Elements](https://leetcode.com/problems/make-lexicographically-smallest-array-by-swapping-elements/) 2047
*   [3736. Longest Alternating Subarray after Removing at Most One Element](https://leetcode.com/problems/longest-alternating-subarray-after-removing-at-most-one-element/)
*   [2593. Find Score of an Array after Marking All Elements](https://leetcode.com/problems/find-score-of-an-array-after-marking-all-elements/)
*   [3640. Trionic Array Ii](https://leetcode.com/problems/trionic-array-ii/) 2278
*   [2393. Count Strictly Increasing Subarrays](https://leetcode.com/problems/count-strictly-increasing-subarrays/) (Premium)
*   [3732. Maximum Number of Equal Length Runs](https://leetcode.com/problems/maximum-number-of-equal-length-runs/) (Premium)
*   [2436. Minimum Split Into Subarrays with Gcd Greater than One](https://leetcode.com/problems/minimum-split-into-subarrays-with-gcd-greater-than-one/) (Premium)
*   [2495. Number of Subarrays Having Even Product](https://leetcode.com/problems/number-of-subarrays-having-even-product/) (Premium)
*   [3063. Linked List Frequency](https://leetcode.com/problems/linked-list-frequency/) (Premium)


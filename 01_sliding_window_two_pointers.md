# Sliding Window & Two Pointers

Problem list from [0x3F's LeetCode Study Plan](https://leetcode.com/discuss/post/3578981/) — problems sorted by difficulty rating.

## I. Fixed-Length Sliding Window

### §1.1 Basics

[Tutorial](https://leetcode.com/problems/maximum-number-of-vowels-in-a-substring-of-given-length/solutions/2809359/tao-lu-jiao-ni-jie-jue-ding-chang-hua-ch-fzfo/)

- [1456. Maximum Number Of Vowels In A Substring Of Given Length](https://leetcode.com/problems/maximum-number-of-vowels-in-a-substring-of-given-length/) 1263
- [643. Maximum Average Subarray I](https://leetcode.com/problems/maximum-average-subarray-i/)
- [1343. Number Of Sub Arrays Of Size K And Average Greater Than Or Equal To Threshold](https://leetcode.com/problems/number-of-sub-arrays-of-size-k-and-average-greater-than-or-equal-to-threshold/) 1317
- [2090. K Radius Subarray Averages](https://leetcode.com/problems/k-radius-subarray-averages/) 1358
- [2379. Minimum Recolors To Get K Consecutive Black Blocks](https://leetcode.com/problems/minimum-recolors-to-get-k-consecutive-black-blocks/) 1360
- [2841. Maximum Sum Of Almost Unique Subarray](https://leetcode.com/problems/maximum-sum-of-almost-unique-subarray/) 1546
- [2461. Maximum Sum Of Distinct Subarrays With Length K](https://leetcode.com/problems/maximum-sum-of-distinct-subarrays-with-length-k/) 1553
- [1423. Maximum Points You Can Obtain From Cards](https://leetcode.com/problems/maximum-points-you-can-obtain-from-cards/) 1574
- [1176. Diet Plan Performance](https://leetcode.com/problems/diet-plan-performance/) 🔒
- [1100. Find K Length Substrings With No Repeated Characters](https://leetcode.com/problems/find-k-length-substrings-with-no-repeated-characters/) 🔒
- [1852. Distinct Numbers In Each Subarray](https://leetcode.com/problems/distinct-numbers-in-each-subarray/) 🔒
- [1151. Minimum Swaps To Group All 1s Together](https://leetcode.com/problems/minimum-swaps-to-group-all-1s-together/) 🔒
- [2107. Number Of Unique Flavors After Sharing K Candies](https://leetcode.com/problems/number-of-unique-flavors-after-sharing-k-candies/) 🔒

### §1.2 Advanced (Optional)

- [1052. Grumpy Bookstore Owner](https://leetcode.com/problems/grumpy-bookstore-owner/) 1418
- [3679. Minimum Discards To Balance Inventory](https://leetcode.com/problems/minimum-discards-to-balance-inventory/) 1639
- [3439. Reschedule Meetings For Maximum Free Time I](https://leetcode.com/problems/reschedule-meetings-for-maximum-free-time-i/) 1729
- [3694. Distinct Points Reachable After Substring Removal](https://leetcode.com/problems/distinct-points-reachable-after-substring-removal/) 1739
- [2134. Minimum Swaps To Group All 1s Together II](https://leetcode.com/problems/minimum-swaps-to-group-all-1s-together-ii/) 1748
- [1652. Defuse The Bomb](https://leetcode.com/problems/defuse-the-bomb/) (O(n) required)
- [1297. Maximum Number Of Occurrences Of A Substring](https://leetcode.com/problems/maximum-number-of-occurrences-of-a-substring/) 1748
- [3652. Best Time To Buy And Sell Stock Using Strategy](https://leetcode.com/problems/best-time-to-buy-and-sell-stock-using-strategy/)
- [567. Permutation In String](https://leetcode.com/problems/permutation-in-string/)
- [438. Find All Anagrams In A String](https://leetcode.com/problems/find-all-anagrams-in-a-string/)
- [30. Substring With Concatenation Of All Words](https://leetcode.com/problems/substring-with-concatenation-of-all-words/)
- [1888. Minimum Number Of Flips To Make The Binary String Alternating](https://leetcode.com/problems/minimum-number-of-flips-to-make-the-binary-string-alternating/) 2006
- [2156. Find Substring With Given Hash Value](https://leetcode.com/problems/find-substring-with-given-hash-value/) 2063
- [2953. Count Complete Substrings](https://leetcode.com/problems/count-complete-substrings/) 2449
- [3672. Sum Of Weighted Modes In Subarrays](https://leetcode.com/problems/sum-of-weighted-modes-in-subarrays/) 🔒
- [2067. Number Of Equal Count Substrings](https://leetcode.com/problems/number-of-equal-count-substrings/) 🔒
- [2524. Maximum Frequency Score Of A Subarray](https://leetcode.com/problems/maximum-frequency-score-of-a-subarray/) 🔒

**Mind Extensions**:

- [2200. Find All K Distant Indices In An Array](https://leetcode.com/problems/find-all-k-distant-indices-in-an-array/) (O(n) required)
- [1461. Check If A String Contains All Binary Codes Of Size K](https://leetcode.com/problems/check-if-a-string-contains-all-binary-codes-of-size-k/) 1504
- [1016. Binary String With Substrings Representing 1 To N](https://leetcode.com/problems/binary-string-with-substrings-representing-1-to-n/) (O(|s|) required)
- [2653. Sliding Subarray Beauty](https://leetcode.com/problems/sliding-subarray-beauty/) 1786

## II. Variable-Length Sliding Window

Variable-length sliding window covers three categories: find longest subarray, find shortest subarray, count subarrays.

> **Note**: A sliding window maintains a **queue**. Moving the right pointer = enqueue; moving the left pointer = dequeue.

### §2.1 Shorter is Valid / Find Longest

#### §2.1.1 Basics

- [3. Longest Substring Without Repeating Characters](https://leetcode.com/problems/longest-substring-without-repeating-characters/)
- [3090. Maximum Length Substring With Two Occurrences](https://leetcode.com/problems/maximum-length-substring-with-two-occurrences/) 1329
- [1493. Longest Subarray Of 1s After Deleting One Element](https://leetcode.com/problems/longest-subarray-of-1s-after-deleting-one-element/) 1423
- [3634. Minimum Removals To Balance Array](https://leetcode.com/problems/minimum-removals-to-balance-array/) 1453
- [1208. Get Equal Substrings Within Budget](https://leetcode.com/problems/get-equal-substrings-within-budget/) 1497
- [904. Fruit Into Baskets](https://leetcode.com/problems/fruit-into-baskets/) 1516
- [1695. Maximum Erasure Value](https://leetcode.com/problems/maximum-erasure-value/) 1529
- [2958. Length Of Longest Subarray With At Most K Frequency](https://leetcode.com/problems/length-of-longest-subarray-with-at-most-k-frequency/) 1535
- [2024. Maximize The Confusion Of An Exam](https://leetcode.com/problems/maximize-the-confusion-of-an-exam/) 1643
- [1004. Max Consecutive Ones III](https://leetcode.com/problems/max-consecutive-ones-iii/) 1656
- [3641. Longest Semi Repeating Subarray](https://leetcode.com/problems/longest-semi-repeating-subarray/) 🔒

#### §2.1.2 Advanced (Optional)

- [2730. Find The Longest Semi Repetitive Substring](https://leetcode.com/problems/find-the-longest-semi-repetitive-substring/) (non-brute-force)
- [2779. Maximum Beauty Of An Array After Applying Operation](https://leetcode.com/problems/maximum-beauty-of-an-array-after-applying-operation/) 1638
- [1658. Minimum Operations To Reduce X To Zero](https://leetcode.com/problems/minimum-operations-to-reduce-x-to-zero/) 1817
- [1838. Frequency Of The Most Frequent Element](https://leetcode.com/problems/frequency-of-the-most-frequent-element/) 1876
- [2516. Take K Of Each Character From Left And Right](https://leetcode.com/problems/take-k-of-each-character-from-left-and-right/) 1948
- [2831. Find The Longest Equal Subarray](https://leetcode.com/problems/find-the-longest-equal-subarray/) 1976
- [2271. Maximum White Tiles Covered By A Carpet](https://leetcode.com/problems/maximum-white-tiles-covered-by-a-carpet/) 2022
- [2106. Maximum Fruits Harvested After At Most K Steps](https://leetcode.com/problems/maximum-fruits-harvested-after-at-most-k-steps/) 2062
- [2555. Maximize Win From Two Segments](https://leetcode.com/problems/maximize-win-from-two-segments/) 2081
- [2009. Minimum Number Of Operations To Make Array Continuous](https://leetcode.com/problems/minimum-number-of-operations-to-make-array-continuous/) 2084
- [1610. Maximum Number Of Visible Points](https://leetcode.com/problems/maximum-number-of-visible-points/) 2147
- [2781. Length Of The Longest Valid Substring](https://leetcode.com/problems/length-of-the-longest-valid-substring/) 2204
- [3411. Maximum Subarray With Equal Products](https://leetcode.com/problems/maximum-subarray-with-equal-products/) (non-brute-force ~2300)
- [3413. Maximum Coins From K Consecutive Bags](https://leetcode.com/problems/maximum-coins-from-k-consecutive-bags/) 2374
- [395. Longest Substring With At Least K Repeating Characters](https://leetcode.com/problems/longest-substring-with-at-least-k-repeating-characters/)
- [1763. Longest Nice Substring](https://leetcode.com/problems/longest-nice-substring/) (non-brute-force)
- [2968. Apply Operations To Maximize Frequency Score](https://leetcode.com/problems/apply-operations-to-maximize-frequency-score/) 2444
- [1040. Moving Stones Until Consecutive II](https://leetcode.com/problems/moving-stones-until-consecutive-ii/) 2456
- [487. Max Consecutive Ones II](https://leetcode.com/problems/max-consecutive-ones-ii/) 🔒
- [159. Longest Substring With At Most Two Distinct Characters](https://leetcode.com/problems/longest-substring-with-at-most-two-distinct-characters/) 🔒
- [340. Longest Substring With At Most K Distinct Characters](https://leetcode.com/problems/longest-substring-with-at-most-k-distinct-characters/) 🔒

### §2.2 Longer is Valid / Find Shortest

- [209. Minimum Size Subarray Sum](https://leetcode.com/problems/minimum-size-subarray-sum/)
- [3795. Minimum Subarray Length With Distinct Sum At Least K](https://leetcode.com/problems/minimum-subarray-length-with-distinct-sum-at-least-k/) 1505
- [2904. Shortest And Lexicographically Smallest Beautiful String](https://leetcode.com/problems/shortest-and-lexicographically-smallest-beautiful-string/)
- [1234. Replace The Substring For Balanced String](https://leetcode.com/problems/replace-the-substring-for-balanced-string/) 1878
- [2875. Minimum Size Subarray In Infinite Array](https://leetcode.com/problems/minimum-size-subarray-in-infinite-array/) 1914
- [76. Minimum Window Substring](https://leetcode.com/problems/minimum-window-substring/)
- [632. Smallest Range Covering Elements From K Lists](https://leetcode.com/problems/smallest-range-covering-elements-from-k-lists/) (multiple approaches)

### §2.3 Count Subarrays

#### §2.3.1 Basics

- [713. Subarray Product Less Than K](https://leetcode.com/problems/subarray-product-less-than-k/)
- [3258. Count Substrings That Satisfy K Constraint I](https://leetcode.com/problems/count-substrings-that-satisfy-k-constraint-i/) (O(n) required)
- [2302. Count Subarrays With Score Less Than K](https://leetcode.com/problems/count-subarrays-with-score-less-than-k/) 1808
- [2762. Continuous Subarrays](https://leetcode.com/problems/continuous-subarrays/) 1940
- [LCP 68. Bouquet of Flowers](https://leetcode.com/problems/1GxJYY/)
- [2743. Count Substrings Without Repeating Character](https://leetcode.com/problems/count-substrings-without-repeating-character/) 🔒

**Mind Extensions**:

- [3134. Find The Median Of The Uniqueness Array](https://leetcode.com/problems/find-the-median-of-the-uniqueness-array/) 2451
- [3261. Count Substrings That Satisfy K Constraint II](https://leetcode.com/problems/count-substrings-that-satisfy-k-constraint-ii/) 2659 (substring of substrings)

#### §2.3.2 Advanced (Optional)

- [1358. Number Of Substrings Containing All Three Characters](https://leetcode.com/problems/number-of-substrings-containing-all-three-characters/) 1646
- [2962. Count Subarrays Where Max Element Appears At Least K Times](https://leetcode.com/problems/count-subarrays-where-max-element-appears-at-least-k-times/) 1701
- [3325. Count Substrings With K Frequency Characters I](https://leetcode.com/problems/count-substrings-with-k-frequency-characters-i/) (O(n) required)
- [2062. Count Vowel Substrings Of A String](https://leetcode.com/problems/count-vowel-substrings-of-a-string/) (O(n) required)
- [2799. Count Complete Subarrays In An Array](https://leetcode.com/problems/count-complete-subarrays-in-an-array/) (O(n) required)
- [2537. Count The Number Of Good Subarrays](https://leetcode.com/problems/count-the-number-of-good-subarrays/) 1892
- [3298. Count Substrings That Can Be Rearranged To Contain A String II](https://leetcode.com/problems/count-substrings-that-can-be-rearranged-to-contain-a-string-ii/) 1909 (same as 76)
- [2495. Number Of Subarrays Having Even Product](https://leetcode.com/problems/number-of-subarrays-having-even-product/) 🔒

#### §2.3.3 Other Advanced

- [930. Binary Subarrays With Sum](https://leetcode.com/problems/binary-subarrays-with-sum/) 1592
- [1248. Count Number Of Nice Subarrays](https://leetcode.com/problems/count-number-of-nice-subarrays/) 1624
- [3306. Count Of Substrings Containing Every Vowel And K Consonants II](https://leetcode.com/problems/count-of-substrings-containing-every-vowel-and-k-consonants-ii/) 2200
- [992. Subarrays With K Different Integers](https://leetcode.com/problems/subarrays-with-k-different-integers/) 2210
- [3859. Count Subarrays With K Distinct Integers](https://leetcode.com/problems/count-subarrays-with-k-distinct-integers/) 2302

### §2.4 Other

- [825. Friends Of Appropriate Ages](https://leetcode.com/problems/friends-of-appropriate-ages/) 1697
- [2401. Longest Nice Subarray](https://leetcode.com/problems/longest-nice-subarray/) 1750
- [1156. Swap For Longest Repeated Character Substring](https://leetcode.com/problems/swap-for-longest-repeated-character-substring/) 1787 (simple approach exists)
- [424. Longest Repeating Character Replacement](https://leetcode.com/problems/longest-repeating-character-replacement/)
- [438. Find All Anagrams In A String](https://leetcode.com/problems/find-all-anagrams-in-a-string/) (fixed-length and variable-length approaches)
- [1712. Ways To Split Array Into Three Subarrays](https://leetcode.com/problems/ways-to-split-array-into-three-subarrays/) 2079
- [LCR 180. File Combination](https://leetcode.com/problems/he-wei-sde-lian-xu-zheng-shu-xu-lie-lcof/)
- [1918. Kth Smallest Subarray Sum](https://leetcode.com/problems/kth-smallest-subarray-sum/) 🔒

---
> **Note**: Sliding window problems end here. Continue to the next study plan.

Study roadmap: [How to Study Systematically](https://leetcode.com/circle/discuss/RvFUtj/)

---

## III. Single-Sequence Two Pointers

### §3.1 Reverse String

- [344. Reverse String](https://leetcode.com/problems/reverse-string/)
- [3794. Reverse String Prefix](https://leetcode.com/problems/reverse-string-prefix/)
- [2000. Reverse Prefix Of Word](https://leetcode.com/problems/reverse-prefix-of-word/) 1199
- [3643. Flip Square Submatrix Vertically](https://leetcode.com/problems/flip-square-submatrix-vertically/) 1235
- [832. Flipping An Image](https://leetcode.com/problems/flipping-an-image/) 1243
- [3823. Reverse Letters Then Special Characters In A String](https://leetcode.com/problems/reverse-letters-then-special-characters-in-a-string/) 1250
- [541. Reverse String II](https://leetcode.com/problems/reverse-string-ii/)
- [557. Reverse Words In A String III](https://leetcode.com/problems/reverse-words-in-a-string-iii/)
- [151. Reverse Words In A String](https://leetcode.com/problems/reverse-words-in-a-string/)
- [3775. Reverse Words With Same Vowel Count](https://leetcode.com/problems/reverse-words-with-same-vowel-count/) 1392
- [917. Reverse Only Letters](https://leetcode.com/problems/reverse-only-letters/)
- [345. Reverse Vowels Of A String](https://leetcode.com/problems/reverse-vowels-of-a-string/)
- [3865. Reverse K Subarrays](https://leetcode.com/problems/reverse-k-subarrays/) 🔒
- [186. Reverse Words In A String II](https://leetcode.com/problems/reverse-words-in-a-string-ii/) 🔒

### §3.2 Two Pointers on Sorted Array/String

- [2697. Lexicographically Smallest Palindrome](https://leetcode.com/problems/lexicographically-smallest-palindrome/) 1304
- [125. Valid Palindrome](https://leetcode.com/problems/valid-palindrome/)
- [1750. Minimum Length Of String After Deleting Similar Ends](https://leetcode.com/problems/minimum-length-of-string-after-deleting-similar-ends/) 1502
- [2105. Watering Plants II](https://leetcode.com/problems/watering-plants-ii/) 1507
- [977. Squares Of A Sorted Array](https://leetcode.com/problems/squares-of-a-sorted-array/) (O(n) required)
- [658. Find K Closest Elements](https://leetcode.com/problems/find-k-closest-elements/)
- [1471. The K Strongest Values In An Array](https://leetcode.com/problems/the-k-strongest-values-in-an-array/)
- [167. Two Sum II Input Array Is Sorted](https://leetcode.com/problems/two-sum-ii-input-array-is-sorted/)
- [633. Sum Of Square Numbers](https://leetcode.com/problems/sum-of-square-numbers/)
- [2824. Count Pairs Whose Sum Is Less Than Target](https://leetcode.com/problems/count-pairs-whose-sum-is-less-than-target/) (non-brute-force)
- [LCP 28. Purchasing Plan](https://leetcode.com/problems/4xy4Wx/) (same as 2824)
- [16. 3sum Closest](https://leetcode.com/problems/3sum-closest/)
- [15. 3sum](https://leetcode.com/problems/3sum/)
- [18. 4sum](https://leetcode.com/problems/4sum/)
- [1577. Number Of Ways Where Square Of Number Is Equal To Product Of Two Numbers](https://leetcode.com/problems/number-of-ways-where-square-of-number-is-equal-to-product-of-two-numbers/) 1594
- [3862. Find The Smallest Balanced Index](https://leetcode.com/problems/find-the-smallest-balanced-index/) 1697
- [611. Valid Triangle Number](https://leetcode.com/problems/valid-triangle-number/)
- [923. 3sum With Multiplicity](https://leetcode.com/problems/3sum-with-multiplicity/) 1711
- [2563. Count The Number Of Fair Pairs](https://leetcode.com/problems/count-the-number-of-fair-pairs/) 1721
- [948. Bag Of Tokens](https://leetcode.com/problems/bag-of-tokens/) 1762
- [11. Container With Most Water](https://leetcode.com/problems/container-with-most-water/)
- [42. Trapping Rain Water](https://leetcode.com/problems/trapping-rain-water/)
- [1616. Split Two Strings To Make Palindrome](https://leetcode.com/problems/split-two-strings-to-make-palindrome/) 1868
- [1498. Number Of Subsequences That Satisfy The Given Sum Condition](https://leetcode.com/problems/number-of-subsequences-that-satisfy-the-given-sum-condition/) 2276
- [1782. Count Pairs Of Nodes](https://leetcode.com/problems/count-pairs-of-nodes/) 2457
- [1099. Two Sum Less Than K](https://leetcode.com/problems/two-sum-less-than-k/) 🔒
- [360. Sort Transformed Array](https://leetcode.com/problems/sort-transformed-array/) 🔒
- [2422. Merge Operations To Turn Array Into A Palindrome](https://leetcode.com/problems/merge-operations-to-turn-array-into-a-palindrome/) 🔒
- [259. 3sum Smaller](https://leetcode.com/problems/3sum-smaller/) 🔒
- [3802. Number Of Ways To Paint Sheets](https://leetcode.com/problems/number-of-ways-to-paint-sheets/) 🔒

**Mind Extensions**:

- [1861. Rotating The Box](https://leetcode.com/problems/rotating-the-box/) 1537
- [3814. Maximum Capacity Within Budget](https://leetcode.com/problems/maximum-capacity-within-budget/) 1796

### §3.3 Partition

- [2200. Find All K Distant Indices In An Array](https://leetcode.com/problems/find-all-k-distant-indices-in-an-array/) (O(n) required)
- [611. Valid Triangle Number](https://leetcode.com/problems/valid-triangle-number/)
- [3649. Number Of Perfect Pairs](https://leetcode.com/problems/number-of-perfect-pairs/) 1716
- [1871. Jump Game VII](https://leetcode.com/problems/jump-game-vii/) 1896 (multiple approaches)
- [1574. Shortest Subarray To Be Removed To Make Array Sorted](https://leetcode.com/problems/shortest-subarray-to-be-removed-to-make-array-sorted/) 1932
- [2972. Count The Number Of Incremovable Subarrays II](https://leetcode.com/problems/count-the-number-of-incremovable-subarrays-ii/) 2153
- [2122. Recover The Original Array](https://leetcode.com/problems/recover-the-original-array/) 2159
- [2234. Maximum Total Beauty Of The Gardens](https://leetcode.com/problems/maximum-total-beauty-of-the-gardens/) 2562
- [1989. Maximum Number Of People That Can Be Caught In Tag](https://leetcode.com/problems/maximum-number-of-people-that-can-be-caught-in-tag/) 🔒
- [3323. Minimize Connected Groups By Inserting Interval](https://leetcode.com/problems/minimize-connected-groups-by-inserting-interval/) 🔒

- [581. Shortest Unsorted Continuous Subarray](https://leetcode.com/problems/shortest-unsorted-continuous-subarray/)
- [3555. Smallest Subarray To Sort In Every Sliding Window](https://leetcode.com/problems/smallest-subarray-to-sort-in-every-sliding-window/) 🔒

### §3.4 Other Single-Sequence

- [1793. Maximum Score Of A Good Subarray](https://leetcode.com/problems/maximum-score-of-a-good-subarray/) 1946
- [976. Largest Perimeter Triangle](https://leetcode.com/problems/largest-perimeter-triangle/)

### §3.5 In-Place Modification

- [27. Remove Element](https://leetcode.com/problems/remove-element/)
- [26. Remove Duplicates From Sorted Array](https://leetcode.com/problems/remove-duplicates-from-sorted-array/)
- [80. Remove Duplicates From Sorted Array II](https://leetcode.com/problems/remove-duplicates-from-sorted-array-ii/)
- [2273. Find Resultant Array After Removing Anagrams](https://leetcode.com/problems/find-resultant-array-after-removing-anagrams/)
- [3684. Maximize Sum Of At Most K Distinct Elements](https://leetcode.com/problems/maximize-sum-of-at-most-k-distinct-elements/)
- [283. Move Zeroes](https://leetcode.com/problems/move-zeroes/)
- [905. Sort Array By Parity](https://leetcode.com/problems/sort-array-by-parity/)
- [922. Sort Array By Parity II](https://leetcode.com/problems/sort-array-by-parity-ii/)
- [3467. Transform Array By Parity](https://leetcode.com/problems/transform-array-by-parity/)
- [2460. Apply Operations To An Array](https://leetcode.com/problems/apply-operations-to-an-array/)
- [1089. Duplicate Zeros](https://leetcode.com/problems/duplicate-zeros/)
- [75. Sort Colors](https://leetcode.com/problems/sort-colors/)

**Mind Extensions**:

- [2784. Check If Array Is Good](https://leetcode.com/problems/check-if-array-is-good/)
- [442. Find All Duplicates In An Array](https://leetcode.com/problems/find-all-duplicates-in-an-array/)
- [448. Find All Numbers Disappeared In An Array](https://leetcode.com/problems/find-all-numbers-disappeared-in-an-array/)
- [1920. Build Array From Permutation](https://leetcode.com/problems/build-array-from-permutation/)
- [41. First Missing Positive](https://leetcode.com/problems/first-missing-positive/)

### §3.6 Two Pointers on Matrix

- [240. Search A 2d Matrix II](https://leetcode.com/problems/search-a-2d-matrix-ii/)
- [1351. Count Negative Numbers In A Sorted Matrix](https://leetcode.com/problems/count-negative-numbers-in-a-sorted-matrix/)

## IV. Two-Sequence Two Pointers

### §4.1 Two Pointers

- [2109. Adding Spaces To A String](https://leetcode.com/problems/adding-spaces-to-a-string/) 1315
- [2540. Minimum Common Value](https://leetcode.com/problems/minimum-common-value/) (O(n+m) required)
- [350. Intersection Of Two Arrays II](https://leetcode.com/problems/intersection-of-two-arrays-ii/) (solve follow-up)
- [88. Merge Sorted Array](https://leetcode.com/problems/merge-sorted-array/) (O(n+m) required)
- [2570. Merge Two 2d Arrays By Summing Values](https://leetcode.com/problems/merge-two-2d-arrays-by-summing-values/) (O(n+m) required)
- [LCP 18. Breakfast Combo](https://leetcode.com/problems/2vYnGI/)
- [1855. Maximum Distance Between A Pair Of Values](https://leetcode.com/problems/maximum-distance-between-a-pair-of-values/) 1515
- [1385. Find The Distance Value Between Two Arrays](https://leetcode.com/problems/find-the-distance-value-between-two-arrays/)
- [925. Long Pressed Name](https://leetcode.com/problems/long-pressed-name/) (O(n+m) required)
- [809. Expressive Words](https://leetcode.com/problems/expressive-words/) 1605
- [2337. Move Pieces To Obtain A String](https://leetcode.com/problems/move-pieces-to-obtain-a-string/) 1693
- [777. Swap Adjacent In LR String](https://leetcode.com/problems/swap-adjacent-in-lr-string/) (same as 2337)
- [844. Backspace String Compare](https://leetcode.com/problems/backspace-string-compare/) (O(1) extra space)
- [986. Interval List Intersections](https://leetcode.com/problems/interval-list-intersections/) (O(n+m) required)
- [Interview 16.06. Smallest Difference](https://leetcode.com/problems/smallest-difference-lcci/)
- [475. Heaters](https://leetcode.com/problems/heaters/)
- [1537. Get The Maximum Score](https://leetcode.com/problems/get-the-maximum-score/) 1961
- [244. Shortest Word Distance II](https://leetcode.com/problems/shortest-word-distance-ii/) 🔒
- [2838. Maximum Coins Heroes Can Collect](https://leetcode.com/problems/maximum-coins-heroes-can-collect/) 🔒
- [1229. Meeting Scheduler](https://leetcode.com/problems/meeting-scheduler/) 🔒
- [1570. Dot Product Of Two Sparse Vectors](https://leetcode.com/problems/dot-product-of-two-sparse-vectors/) 🔒
- [1868. Product Of Two Run Length Encoded Arrays](https://leetcode.com/problems/product-of-two-run-length-encoded-arrays/) 🔒

### §4.2 Merge Two Arrays/Strings

- [392. Is Subsequence](https://leetcode.com/problems/is-subsequence/)
- [524. Longest Word In Dictionary Through Deleting](https://leetcode.com/problems/longest-word-in-dictionary-through-deleting/)
- [2486. Append Characters To String To Make Subsequence](https://leetcode.com/problems/append-characters-to-string-to-make-subsequence/) 1363
- [2825. Make String A Subsequence Using Cyclic Increments](https://leetcode.com/problems/make-string-a-subsequence-using-cyclic-increments/) 1415
- [1023. Camelcase Matching](https://leetcode.com/problems/camelcase-matching/) 1537
- [3132. Find The Integer Added To Array II](https://leetcode.com/problems/find-the-integer-added-to-array-ii/) 1620
- [522. Longest Uncommon Subsequence II](https://leetcode.com/problems/longest-uncommon-subsequence-ii/) ~1700
- [1826. Faulty Sensor](https://leetcode.com/problems/faulty-sensor/) 🔒

- [1898. Maximum Number Of Removable Characters](https://leetcode.com/problems/maximum-number-of-removable-characters/) 1913
- [2565. Subsequence With The Minimum Score](https://leetcode.com/problems/subsequence-with-the-minimum-score/) 2432
- [3302. Find The Lexicographically Smallest Valid Sequence](https://leetcode.com/problems/find-the-lexicographically-smallest-valid-sequence/) 2474

## V. Three Pointers

- [2367. Number Of Arithmetic Triplets](https://leetcode.com/problems/number-of-arithmetic-triplets/) (O(n) required)
- [2563. Count The Number Of Fair Pairs](https://leetcode.com/problems/count-the-number-of-fair-pairs/) 1721
- [795. Number Of Subarrays With Bounded Maximum](https://leetcode.com/problems/number-of-subarrays-with-bounded-maximum/) 1817
- [2444. Count Subarrays With Fixed Bounds](https://leetcode.com/problems/count-subarrays-with-fixed-bounds/) 2093
- [3347. Maximum Frequency Of An Element After Performing Operations II](https://leetcode.com/problems/maximum-frequency-of-an-element-after-performing-operations-ii/) 2156
- [1213. Intersection Of Three Sorted Arrays](https://leetcode.com/problems/intersection-of-three-sorted-arrays/) 🔒

**Mind Extensions**:

- [3464. Maximize The Distance Between Points On A Square](https://leetcode.com/problems/maximize-the-distance-between-points-on-a-square/) 2806 (k pointers)

## VI. Group Loop

**Use case**: The array is divided into groups per the problem rules, and each group uses the same logic.

**Core idea**:

- The outer loop handles setup before each group (record start position) and aggregation after (update max answer).
- The inner loop traverses the group to find where it ends.

This pattern keeps logic blocks clear and avoids special-casing the last group (a common bug). It's the least error-prone approach.

[Longest Even Odd Subarray With Threshold](https://leetcode.com/problems/longest-even-odd-subarray-with-threshold/solutions/2528771/jiao-ni-yi-ci-xing-ba-dai-ma-xie-dui-on-zuspx/)

- [485. Max Consecutive Ones](https://leetcode.com/problems/max-consecutive-ones/)
- [1446. Consecutive Characters](https://leetcode.com/problems/consecutive-characters/) 1165
- [1869. Longer Contiguous Segments Of Ones Than Zeros](https://leetcode.com/problems/longer-contiguous-segments-of-ones-than-zeros/) 1205
- [2414. Length Of The Longest Alphabetical Continuous Substring](https://leetcode.com/problems/length-of-the-longest-alphabetical-continuous-substring/) 1222
- [3456. Find Special Substring Of Length K](https://leetcode.com/problems/find-special-substring-of-length-k/) 1244
- [830. Positions Of Large Groups](https://leetcode.com/problems/positions-of-large-groups/) 1252
- [2273. Find Resultant Array After Removing Anagrams](https://leetcode.com/problems/find-resultant-array-after-removing-anagrams/) 1295
- [2264. Largest 3 Same Digit Number In String](https://leetcode.com/problems/largest-3-same-digit-number-in-string/) 1309
- [2348. Number Of Zero Filled Subarrays](https://leetcode.com/problems/number-of-zero-filled-subarrays/) 1316
- [1513. Number Of Substrings With Only 1s](https://leetcode.com/problems/number-of-substrings-with-only-1s/) 1351
- [1957. Delete Characters To Make Fancy String](https://leetcode.com/problems/delete-characters-to-make-fancy-string/) 1358
- [674. Longest Continuous Increasing Subsequence](https://leetcode.com/problems/longest-continuous-increasing-subsequence/)
- [3708. Longest Fibonacci Subarray](https://leetcode.com/problems/longest-fibonacci-subarray/) 1381 (O(n) required)
- [696. Count Binary Substrings](https://leetcode.com/problems/count-binary-substrings/)
- [978. Longest Turbulent Subarray](https://leetcode.com/problems/longest-turbulent-subarray/) 1393
- [2110. Number Of Smooth Descent Periods Of A Stock](https://leetcode.com/problems/number-of-smooth-descent-periods-of-a-stock/) 1408
- [228. Summary Ranges](https://leetcode.com/problems/summary-ranges/)
- [2760. Longest Even Odd Subarray With Threshold](https://leetcode.com/problems/longest-even-odd-subarray-with-threshold/) 1420
- [1887. Reduction Operations To Make The Array Elements Equal](https://leetcode.com/problems/reduction-operations-to-make-the-array-elements-equal/) 1428
- [845. Longest Mountain In Array](https://leetcode.com/problems/longest-mountain-in-array/) 1437
- [2038. Remove Colored Pieces If Both Neighbors Are The Same Color](https://leetcode.com/problems/remove-colored-pieces-if-both-neighbors-are-the-same-color/) 1468
- [2900. Longest Unequal Adjacent Groups Subsequence I](https://leetcode.com/problems/longest-unequal-adjacent-groups-subsequence-i/) 1469
- [1759. Count Number Of Homogenous Substrings](https://leetcode.com/problems/count-number-of-homogenous-substrings/) 1491
- [3011. Find If Array Can Be Sorted](https://leetcode.com/problems/find-if-array-can-be-sorted/) 1497
- [1861. Rotating The Box](https://leetcode.com/problems/rotating-the-box/) 1537
- [1578. Minimum Time To Make Rope Colorful](https://leetcode.com/problems/minimum-time-to-make-rope-colorful/) 1574
- [1839. Longest Substring Of All Vowels In Order](https://leetcode.com/problems/longest-substring-of-all-vowels-in-order/) 1580
- [2765. Longest Alternating Subarray](https://leetcode.com/problems/longest-alternating-subarray/) 1581
- [3255. Find The Power Of K Size Subarrays II](https://leetcode.com/problems/find-the-power-of-k-size-subarrays-ii/) 1595
- [3350. Adjacent Increasing Subarrays Detection II](https://leetcode.com/problems/adjacent-increasing-subarrays-detection-ii/) 1600
- [3105. Longest Strictly Increasing Or Strictly Decreasing Subarray](https://leetcode.com/problems/longest-strictly-increasing-or-strictly-decreasing-subarray/)
- [3926. Count Valid Word Occurrences](https://leetcode.com/problems/count-valid-word-occurrences/) 1608
- [838. Push Dominoes](https://leetcode.com/problems/push-dominoes/) 1638
- [467. Unique Substrings In Wraparound String](https://leetcode.com/problems/unique-substrings-in-wraparound-string/) ~1700
- [3499. Maximize Active Section With Trade I](https://leetcode.com/problems/maximize-active-section-with-trade-i/) 1729
- [413. Arithmetic Slices](https://leetcode.com/problems/arithmetic-slices/)
- [3738. Longest Non Decreasing Subarray After Replacing At Most One Element](https://leetcode.com/problems/longest-non-decreasing-subarray-after-replacing-at-most-one-element/) 1811
- [2147. Number Of Ways To Divide A Long Corridor](https://leetcode.com/problems/number-of-ways-to-divide-a-long-corridor/) 1915
- [2593. Find Score Of An Array After Marking All Elements](https://leetcode.com/problems/find-score-of-an-array-after-marking-all-elements/) (O(n) required)
- [68. Text Justification](https://leetcode.com/problems/text-justification/)
- [135. Candy](https://leetcode.com/problems/candy/)
- [3872. Longest Arithmetic Sequence After Changing At Most One Element](https://leetcode.com/problems/longest-arithmetic-sequence-after-changing-at-most-one-element/) 2042
- [2948. Make Lexicographically Smallest Array By Swapping Elements](https://leetcode.com/problems/make-lexicographically-smallest-array-by-swapping-elements/) 2047
- [3830. Longest Alternating Subarray After Removing At Most One Element](https://leetcode.com/problems/longest-alternating-subarray-after-removing-at-most-one-element/) 2162
- [3640. Trionic Array II](https://leetcode.com/problems/trionic-array-ii/) 2278
- [2393. Count Strictly Increasing Subarrays](https://leetcode.com/problems/count-strictly-increasing-subarrays/) 🔒
- [3773. Maximum Number Of Equal Length Runs](https://leetcode.com/problems/maximum-number-of-equal-length-runs/) 🔒
- [2436. Minimum Split Into Subarrays With Gcd Greater Than One](https://leetcode.com/problems/minimum-split-into-subarrays-with-gcd-greater-than-one/) 🔒
- [2495. Number Of Subarrays Having Even Product](https://leetcode.com/problems/number-of-subarrays-having-even-product/) 🔒
- [3063. Linked List Frequency](https://leetcode.com/problems/linked-list-frequency/) 🔒

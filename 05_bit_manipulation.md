# Bit Manipulation

> Problem list from [0x3F's LeetCode Problem Lists](https://leetcode.cn/circle/discuss/dHn9Vk/)

-----

*   [3370. Smallest Number with All Set Bits](https://leetcode.com/problems/smallest-number-with-all-set-bits/) 1199
*   [3226. Number of Bit Changes to Make Two Integers Equal](https://leetcode.com/problems/number-of-bit-changes-to-make-two-integers-equal/) 1247
*   [1356. Sort Integers by the Number of 1 Bits](https://leetcode.com/problems/sort-integers-by-the-number-of-1-bits/) 1258
*   [461. Hamming Distance](https://leetcode.com/problems/hamming-distance/) 1282
*   [2220. Minimum Bit Flips to Convert Number](https://leetcode.com/problems/minimum-bit-flips-to-convert-number/) 1282
*   [1342. Number of Steps to Reduce a Number to Zero](https://leetcode.com/problems/number-of-steps-to-reduce-a-number-to-zero/)
*   [476. Number Complement](https://leetcode.com/problems/number-complement/)
*   [1009. Complement of Base 10 Integer](https://leetcode.com/problems/complement-of-base-10-integer/)
*   [868. Binary Gap](https://leetcode.com/problems/binary-gap/) 1307
*   [2917. Find the K or of an Array](https://leetcode.com/problems/find-the-k-or-of-an-array/) 1389
*   [693. Binary Number with Alternating Bits](https://leetcode.com/problems/binary-number-with-alternating-bits/)
*   [2657. Find the Prefix Common Array of Two Arrays](https://leetcode.com/problems/find-the-prefix-common-array-of-two-arrays/)
*   [面试题 05.01. Insert Into Bits Lcci](https://leetcode.com/problems/insert-into-bits-lcci/)
*   [231. Power of Two](https://leetcode.com/problems/power-of-two/)
*   [342. Power of Four](https://leetcode.com/problems/power-of-four/)
*   [191. Number of 1 Bits](https://leetcode.com/problems/number-of-1-bits/)
*   [338. Counting Bits](https://leetcode.com/problems/counting-bits/) DP
*   [2595. Number of Even and Odd Bits](https://leetcode.com/problems/number-of-even-and-odd-bits/)
*   [2154. Keep Multiplying Found Values by Two](https://leetcode.com/problems/keep-multiplying-found-values-by-two/) ：O(n) ，O(1)
*   [3211. Generate Binary Strings Without Adjacent Zeros](https://leetcode.com/problems/generate-binary-strings-without-adjacent-zeros/)

**用位运算代替数组操作**：

*   [3690. Split and Merge Array Transformation](https://leetcode.com/problems/split-and-merge-array-transformation/)

------------

*   [1486. Xor Operation in an Array](https://leetcode.com/problems/xor-operation-in-an-array/) 1181
*   [1720. Decode Xored Array](https://leetcode.com/problems/decode-xored-array/) 1284
*   [2433. Find the Original Array of Prefix Xor](https://leetcode.com/problems/find-the-original-array-of-prefix-xor/) 1367
*   [1310. Xor Queries of a Subarray](https://leetcode.com/problems/xor-queries-of-a-subarray/) 1460
*   [2683. Neighboring Bitwise Xor](https://leetcode.com/problems/neighboring-bitwise-xor/) 1518
*   [1829. Maximum Xor for Each Query](https://leetcode.com/problems/maximum-xor-for-each-query/) 1523
*   [2997. Minimum Number of Operations to Make Array Xor Equal to K](https://leetcode.com/problems/minimum-number-of-operations-to-make-array-xor-equal-to-k/) 1525
*   [1442. Count Triplets that Can Form Two Arrays of Equal Xor](https://leetcode.com/problems/count-triplets-that-can-form-two-arrays-of-equal-xor/) 1525
*   [2429. Minimize Xor](https://leetcode.com/problems/minimize-xor/) 1532
*   [2527. Find Xor Beauty of Array](https://leetcode.com/problems/find-xor-beauty-of-array/) 1550
*   [2317. Maximum Xor after Operations](https://leetcode.com/problems/maximum-xor-after-operations/) 1679
*   [2588. Count the Number of Beautiful Subarrays](https://leetcode.com/problems/count-the-number-of-beautiful-subarrays/) 1697
*   [2564. Substring Xor Queries](https://leetcode.com/problems/substring-xor-queries/) 1959
*   [1734. Decode Xored Permutation](https://leetcode.com/problems/decode-xored-permutation/) 2024
*   [2857. Count Pairs of Points with Distance K](https://leetcode.com/problems/count-pairs-of-points-with-distance-k/) 2082
*   [1803. Count Pairs with Xor in a Range](https://leetcode.com/problems/count-pairs-with-xor-in-a-range/) 2479
*   [3215. Count Triplets with Even Xor Set Bits Ii](https://leetcode.com/problems/count-triplets-with-even-xor-set-bits-ii/) (Premium)

---------------

*   [2980. Check If Bitwise or Has Trailing Zeros](https://leetcode.com/problems/check-if-bitwise-or-has-trailing-zeros/) 1234
*   [1318. Minimum Flips to Make a or B Equal to C](https://leetcode.com/problems/minimum-flips-to-make-a-or-b-equal-to-c/) 1383
*   [2419. Longest Subarray with Maximum Bitwise and](https://leetcode.com/problems/longest-subarray-with-maximum-bitwise-and/) 1496
*   [2871. Split Array Into Maximum Number of Subarrays](https://leetcode.com/problems/split-array-into-maximum-number-of-subarrays/) 1750
*   [2401. Longest Nice Subarray](https://leetcode.com/problems/longest-nice-subarray/) 1750
*   [2680. Maximum or](https://leetcode.com/problems/maximum-or/) 1912
*   [3133. Minimum Array End](https://leetcode.com/problems/minimum-array-end/) 1935
*   [3108. Minimum Cost Walk in Weighted Graph](https://leetcode.com/problems/minimum-cost-walk-in-weighted-graph/) 2109
*   [3117. Minimum Sum of Values by Dividing Array](https://leetcode.com/problems/minimum-sum-of-values-by-dividing-array/) 2735
*   [3125. Maximum Number that Makes Result of Bitwise and Zero](https://leetcode.com/problems/maximum-number-that-makes-result-of-bitwise-and-zero/) (Premium)

### AND/OR LogTrick

模板：

Python3

Java

C++

Go

    def logTrick(nums: List[int]) -> None:
        for i, x in enumerate(nums):
            for p in or_left:
            or_left.append([x, i])

            idx = 1
            for j in range(1, len(or_left)):
                if or_left[j][0] != or_left[j - 1][0]:
                    or_left[idx] = or_left[j]
                    idx += 1
            del or_left[idx:]

            print(i, x)
            for k, (or_val, left) in enumerate(or_left):
                right = or_left[k + 1][1] - 1 if k < len(or_left) - 1 else i
                print(left, right, or_val)

    logTrick([4, 2, 1, 5])

*   [3171. Find Subarray with Bitwise or Closest to K](https://leetcode.com/problems/find-subarray-with-bitwise-or-closest-to-k/)
*   [1521. Find a Value of a Mysterious Function Closest to Target](https://leetcode.com/problems/find-a-value-of-a-mysterious-function-closest-to-target/) ，OR  AND
*   [3097. Shortest Subarray with or at Least K Ii](https://leetcode.com/problems/shortest-subarray-with-or-at-least-k-ii/) 1891
*   [2411. Smallest Subarrays with Maximum Bitwise or](https://leetcode.com/problems/smallest-subarrays-with-maximum-bitwise-or/) 1938
*   [3209. Number of Subarrays with and Value of K](https://leetcode.com/problems/number-of-subarrays-with-and-value-of-k/) 2050
*   [898. Bitwise Ors of Subarrays](https://leetcode.com/problems/bitwise-ors-of-subarrays/)

### GCD LogTrick

*   [2447. Number of Subarrays with Gcd Equal to K](https://leetcode.com/problems/number-of-subarrays-with-gcd-equal-to-k/)
*   [2654. Minimum Number of Operations to Make All Array Elements Equal to 1](https://leetcode.com/problems/minimum-number-of-operations-to-make-all-array-elements-equal-to-1/)
*   [3605. Minimum Stability Factor of Array](https://leetcode.com/problems/minimum-stability-factor-of-array/) 2410
*   [3574. Maximize Subarray Gcd Score](https://leetcode.com/problems/maximize-subarray-gcd-score/)
*   [2941. Maximum Gcd Sum of a Subarray](https://leetcode.com/problems/maximum-gcd-sum-of-a-subarray/) (Premium)

----------

*   [477. Total Hamming Distance](https://leetcode.com/problems/total-hamming-distance/)
*   [1863. Sum of All Subset Xor Totals](https://leetcode.com/problems/sum-of-all-subset-xor-totals/)
*   [2425. Bitwise Xor of All Pairings](https://leetcode.com/problems/bitwise-xor-of-all-pairings/) 1622
*   [2275. Largest Combination with Bitwise and Greater than Zero](https://leetcode.com/problems/largest-combination-with-bitwise-and-greater-than-zero/) 1642
*   [1835. Find Xor Sum of All Pairs Bitwise and](https://leetcode.com/problems/find-xor-sum-of-all-pairs-bitwise-and/) 1825
*   [3688. Bitwise or of Even Numbers in an Array](https://leetcode.com/problems/bitwise-or-of-even-numbers-in-an-array/)
*   [2505. Bitwise or of All Subsequence Sums](https://leetcode.com/problems/bitwise-or-of-all-subsequence-sums/) (Premium)

**十进制拆位**

*   [3153. Sum of Digit Differences of All Pairs](https://leetcode.com/problems/sum-of-digit-differences-of-all-pairs/) 1645

-----

*   [421. Maximum Xor of Two Numbers in an Array](https://leetcode.com/problems/maximum-xor-of-two-numbers-in-an-array/)
*   [2935. Maximum Strong Pair Xor Ii](https://leetcode.com/problems/maximum-strong-pair-xor-ii/) 2349
*   [3007. Maximum Number that Sum of the Prices is Less than or Equal to K](https://leetcode.com/problems/maximum-number-that-sum-of-the-prices-is-less-than-or-equal-to-k/)
*   [3145. Find Products of Elements of Big Array](https://leetcode.com/problems/find-products-of-elements-of-big-array/) 2859
*   [3022. Minimize or of Remaining Elements Using Operations](https://leetcode.com/problems/minimize-or-of-remaining-elements-using-operations/) 2918
*   [3287. Find the Maximum Sequence Value of Array](https://leetcode.com/problems/find-the-maximum-sequence-value-of-array/) ， U\=27
*   [3344. Maximum Sized Array](https://leetcode.com/problems/maximum-sized-array/) (Premium)

-----

*   [1835. Find Xor Sum of All Pairs Bitwise and](https://leetcode.com/problems/find-xor-sum-of-all-pairs-bitwise-and/) 1825
*   [2354. Number of Excellent Pairs](https://leetcode.com/problems/number-of-excellent-pairs/) 2076

-----

[讲解](/link/?target=https%3A%2F%2Fwww.bilibili.com%2Fvideo%2FBV1pm8vzAEXx%2F)

Python3

Java

C++

Go

    class XorBasis:
        def __init__(self, n: int):
            self.b = [0] * n

        def insert(self, x: int) -> None:
            b = self.b
            for i in range(len(b) - 1, -1, -1):
                        return

        def max_xor(self) -> int:
            b = self.b
            res = 0
            for i in range(len(b) - 1, -1, -1):
                    res ^= b[i]
            return res

*   [3681. Maximum Xor of Subsequences](https://leetcode.com/problems/maximum-xor-of-subsequences/)
*   [3630. Partition Array for Maximum Xor and and](https://leetcode.com/problems/partition-array-for-maximum-xor-and-and/) 2744

-----

*   [2546. Apply Bitwise Operations to Make Strings Equal](https://leetcode.com/problems/apply-bitwise-operations-to-make-strings-equal/) 1605
*   [1558. Minimum Numbers of Function Calls to Make Target Array](https://leetcode.com/problems/minimum-numbers-of-function-calls-to-make-target-array/) 1637
*   [2571. Minimum Operations to Reduce an Integer to 0](https://leetcode.com/problems/minimum-operations-to-reduce-an-integer-to-0/) 1649
*   [3315. Construct the Minimum Bitwise Array Ii](https://leetcode.com/problems/construct-the-minimum-bitwise-array-ii/) 1715
*   [2568. Minimum Impossible or](https://leetcode.com/problems/minimum-impossible-or/) 1754
*   [3644. Maximum K to Sort a Permutation](https://leetcode.com/problems/maximum-k-to-sort-a-permutation/) 1775
*   [2509. Cycle Length Queries in a Tree](https://leetcode.com/problems/cycle-length-queries-in-a-tree/) 1948
*   [2939. Maximum Xor Product](https://leetcode.com/problems/maximum-xor-product/) 2128
*   [2749. Minimum Operations to Make the Integer Zero](https://leetcode.com/problems/minimum-operations-to-make-the-integer-zero/) 2132
*   [2835. Minimum Operations to Form Subsequence with Target Sum](https://leetcode.com/problems/minimum-operations-to-form-subsequence-with-target-sum/) 2207
*   [2897. Apply Operations on Array to Maximize Sum of Squares](https://leetcode.com/problems/apply-operations-on-array-to-maximize-sum-of-squares/) 2301
*   [810. Chalkboard Xor Game](https://leetcode.com/problems/chalkboard-xor-game/) 2341
*   [3064. Guess the Number Using Bitwise Questions I](https://leetcode.com/problems/guess-the-number-using-bitwise-questions-i/) (Premium)
*   [3094. Guess the Number Using Bitwise Questions Ii](https://leetcode.com/problems/guess-the-number-using-bitwise-questions-ii/) (Premium)

## Others
----

*   [136. Single Number](https://leetcode.com/problems/single-number/)
*   [260. Single Number Iii](https://leetcode.com/problems/single-number-iii/)
*   [2965. Find Missing and Repeated Values](https://leetcode.com/problems/find-missing-and-repeated-values/)
*   [137. Single Number Ii](https://leetcode.com/problems/single-number-ii/)
*   [645. Set Mismatch](https://leetcode.com/problems/set-mismatch/)
*   [190. Reverse Bits](https://leetcode.com/problems/reverse-bits/)
*   [371. Sum of Two Integers](https://leetcode.com/problems/sum-of-two-integers/)
*   [201. Bitwise and of Numbers Range](https://leetcode.com/problems/bitwise-and-of-numbers-range/)
*   [2438. Range Product Queries of Powers](https://leetcode.com/problems/range-product-queries-of-powers/) 1610
*   [1680. Concatenation of Consecutive Binary Numbers](https://leetcode.com/problems/concatenation-of-consecutive-binary-numbers/) 1630
*   [1261. Find Elements in a Contaminated Binary Tree](https://leetcode.com/problems/find-elements-in-a-contaminated-binary-tree/)
*   [89. Gray Code](https://leetcode.com/problems/gray-code/)
*   [1238. Circular Permutation in Binary Representation](https://leetcode.com/problems/circular-permutation-in-binary-representation/) 1775
*   [982. Triples with Bitwise and Equal to Zero](https://leetcode.com/problems/triples-with-bitwise-and-equal-to-zero/) 2085
*   [3307. Find the K Th Character in String Game Ii](https://leetcode.com/problems/find-the-k-th-character-in-string-game-ii/) 2232
*   [1611. Minimum One Bit Operations to Make Integers Zero](https://leetcode.com/problems/minimum-one-bit-operations-to-make-integers-zero/) 2345
*   [3514. Number of Unique Xor Triplets Ii](https://leetcode.com/problems/number-of-unique-xor-triplets-ii/) FWT
*   [LCP 81. Ryfuiz](https://leetcode.com/problems/ryfUiz/)
*   [751. Ip to Cidr](https://leetcode.com/problems/ip-to-cidr/) (Premium)
*   [3595. Once Twice](https://leetcode.com/problems/once-twice/) (Premium) 137  260
*   [3141. Maximum Hamming Distances](https://leetcode.com/problems/maximum-hamming-distances/) (Premium)


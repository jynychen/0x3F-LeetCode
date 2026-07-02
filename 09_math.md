# Math Algorithms

Problem list from [0x3F's LeetCode Study Plan](https://leetcode.cn/circle/discuss/IYT3ss/) — Math Algorithms (Number Theory / Combinatorics / Probability & Expectation / Game Theory / Computational Geometry / Randomized Algorithms).

> Many combinatorics problems involve taking a result modulo a prime. For a detailed tutorial on modular arithmetic (fast power, precomputing binomial coefficients, etc.), see [The World of Modular Arithmetic](https://leetcode.cn/circle/discuss/mDfnkW/).

## I. Number Theory

### §1.1 Checking Primality

Check whether `n` is divisible by any integer greater than `1` up to `√n`; if not, `n` is prime. Note that `1` is not a prime.

- [3115. Maximum Prime Difference](https://leetcode.com/problems/maximum-prime-difference/) 1294
- [2614. Prime In Diagonal](https://leetcode.com/problems/prime-in-diagonal/) 1375
- [3765. Complete Prime Number](https://leetcode.com/problems/complete-prime-number/) 1378
- [3556. Sum of Largest Prime Substrings](https://leetcode.com/problems/sum-of-largest-prime-substrings/) 1440
- [3044. Most Frequent Prime](https://leetcode.com/problems/most-frequent-prime/) 1737
- [866. Prime Palindrome](https://leetcode.com/problems/prime-palindrome/) 1938

### §1.2 Prime Preprocessing (Sieve of Eratosthenes)

- [204. Count Primes](https://leetcode.com/problems/count-primes/)
- [3618. Split Array by Prime Indices](https://leetcode.com/problems/split-array-by-prime-indices/) 1227
- [3591. Check if Any Element Has Prime Frequency](https://leetcode.com/problems/check-if-any-element-has-prime-frequency/) 1235
- [762. Prime Number of Set Bits in Binary Representation](https://leetcode.com/problems/prime-number-of-set-bits-in-binary-representation/) 1383
- [2761. Prime Pairs With Target Sum](https://leetcode.com/problems/prime-pairs-with-target-sum/) 1505
- [3233. Find the Count of Numbers Which Are Not Special](https://leetcode.com/problems/find-the-count-of-numbers-which-are-not-special/) 1509
- [3770. Largest Prime From Consecutive Prime Sum](https://leetcode.com/problems/largest-prime-from-consecutive-prime-sum/) 1547
- [2523. Closest Prime Numbers in Range](https://leetcode.com/problems/closest-prime-numbers-in-range/) 1650
- [2601. Prime Subtraction Operation](https://leetcode.com/problems/prime-subtraction-operation/) 1779

### §1.3 Prime Factorization

- [2521. Distinct Prime Factors of Product of Array](https://leetcode.com/problems/distinct-prime-factors-of-product-of-array/) 1413
- [2507. Smallest Value After Replacing With Sum of Prime Factors](https://leetcode.com/problems/smallest-value-after-replacing-with-sum-of-prime-factors/) 1500
- [3326. Minimum Division Operations to Make Array Non-decreasing](https://leetcode.com/problems/minimum-division-operations-to-make-array-non-decreasing/) 1864
- [3629. Minimum Jumps to Reach End via Prime Teleportation](https://leetcode.com/problems/minimum-jumps-to-reach-end-via-prime-teleportation/) 2139
- [2584. Split the Array to Make Coprime Products](https://leetcode.com/problems/split-the-array-to-make-coprime-products/) 2159
- [2709. Greatest Common Divisor Traversal](https://leetcode.com/problems/greatest-common-divisor-traversal/) 2172
- [3715. Sum of Perfect Square Ancestors](https://leetcode.com/problems/sum-of-perfect-square-ancestors/) 2235 (squarefree core)
- [2862. Maximum Element-Sum of a Complete Subset of Indices](https://leetcode.com/problems/maximum-element-sum-of-a-complete-subset-of-indices/) 2292 (squarefree core)
- [2818. Apply Operations to Maximize Score](https://leetcode.com/problems/apply-operations-to-maximize-score/) 2397
- [1998. GCD Sort of an Array](https://leetcode.com/problems/gcd-sort-of-an-array/) 2429
- [1735. Count Ways to Make Array With Product](https://leetcode.com/problems/count-ways-to-make-array-with-product/) 2500
- [2338. Count the Number of Ideal Arrays](https://leetcode.com/problems/count-the-number-of-ideal-arrays/) 2615 (can be optimized with the Min_25 sieve)
- [LCP 14. Partition Array](https://leetcode.cn/problems/qie-fen-shu-zu/)

### §1.4 Factorial Factorization

- [172. Factorial Trailing Zeroes](https://leetcode.com/problems/factorial-trailing-zeroes/)
- [793. Preimage Size of Factorial Zeroes Function](https://leetcode.com/problems/preimage-size-of-factorial-zeroes-function/) 2100

### §1.5 Divisors

- [2427. Number of Common Factors](https://leetcode.com/problems/number-of-common-factors/) 1172
- [1952. Three Divisors](https://leetcode.com/problems/three-divisors/) 1204
- [1492. The kth Factor of n](https://leetcode.com/problems/the-kth-factor-of-n/) 1232
- [507. Perfect Number](https://leetcode.com/problems/perfect-number/)
- [1390. Four Divisors](https://leetcode.com/problems/four-divisors/) 1478
- [1362. Closest Divisors](https://leetcode.com/problems/closest-divisors/) 1534
- [829. Consecutive Numbers Sum](https://leetcode.com/problems/consecutive-numbers-sum/) 1694
- [3447. Assign Elements to Groups With Constraints](https://leetcode.com/problems/assign-elements-to-groups-with-constraints/) 1731 (harmonic series enumeration)
- [3164. Find the Number of Good Pairs II](https://leetcode.com/problems/find-the-number-of-good-pairs-ii/) 1777 (harmonic series enumeration)
- [2176. Count Equal and Divisible Pairs in an Array](https://leetcode.com/problems/count-equal-and-divisible-pairs-in-an-array/) (non-brute-force ~2200)
- [2183. Count Array Pairs Divisible by K](https://leetcode.com/problems/count-array-pairs-divisible-by-k/) 2246
- [952. Largest Component Size by Common Factor](https://leetcode.com/problems/largest-component-size-by-common-factor/) 2272
- [1627. Graph Connectivity With Threshold](https://leetcode.com/problems/graph-connectivity-with-threshold/) 2221
- [2198. Number of Single Divisor Triplets](https://leetcode.com/problems/number-of-single-divisor-triplets/) 🔒
- [625. Minimum Factorization](https://leetcode.com/problems/minimum-factorization/) 🔒
- [2847. Smallest Number With Given Digit Product](https://leetcode.com/problems/smallest-number-with-given-digit-product/) 🔒

### §1.6 Greatest Common Divisor (GCD)

Some languages' standard libraries lack GCD/LCM functions and require a manual implementation. An iterative version is recommended, as it's a bit faster than the recursive one.

- [1979. Find Greatest Common Divisor of Array](https://leetcode.com/problems/find-greatest-common-divisor-of-array/) 1184
- [3658. GCD of Odd and Even Sums](https://leetcode.com/problems/gcd-of-odd-and-even-sums/) 1220
- [2169. Count Operations to Obtain Zero](https://leetcode.com/problems/count-operations-to-obtain-zero/) (non-brute-force)
- [914. X of a Kind in a Deck of Cards](https://leetcode.com/problems/x-of-a-kind-in-a-deck-of-cards/) 1371
- [1071. Greatest Common Divisor of Strings](https://leetcode.com/problems/greatest-common-divisor-of-strings/) 1398
- [2344. Minimum Deletions to Make Array Divisible](https://leetcode.com/problems/minimum-deletions-to-make-array-divisible/) 1641
- [365. Water and Jug Problem](https://leetcode.com/problems/water-and-jug-problem/)
- [2654. Minimum Number of Operations to Make All Array Elements Equal to 1](https://leetcode.com/problems/minimum-number-of-operations-to-make-all-array-elements-equal-to-1/) 1929 (logTrick applicable)
- [1250. Check If It Is a Good Array](https://leetcode.com/problems/check-if-it-is-a-good-array/) 1983 (Bézout's identity)
- [1625. Lexicographically Smallest String After Applying Operations](https://leetcode.com/problems/lexicographically-smallest-string-after-applying-operations/) 1992 (Bézout's identity)
- [2607. Make K-Subarray Sums Equal](https://leetcode.com/problems/make-k-subarray-sums-equal/) 2071 (Bézout's identity)
- [2447. Number of Subarrays With GCD Equal to K](https://leetcode.com/problems/number-of-subarrays-with-gcd-equal-to-k/) (logTrick applicable)
- [2543. Check if Point Is Reachable](https://leetcode.com/problems/check-if-point-is-reachable/) 2221
- [3574. Maximize Subarray GCD Score](https://leetcode.com/problems/maximize-subarray-gcd-score/) 2300 (logTrick applicable)
- [3312. Sorted GCD Pair Queries](https://leetcode.com/problems/sorted-gcd-pair-queries/) 2533 (multiple inclusion-exclusion; variants: 1) subsequence GCD 2) GCD on tree paths)
- [3725. Count Ways to Choose Coprime Integers From Rows](https://leetcode.com/problems/count-ways-to-choose-coprime-integers-from-rows/) (multiple inclusion-exclusion)
- [1819. Number of Different Subsequences GCDs](https://leetcode.com/problems/number-of-different-subsequences-gcds/) 2540 (harmonic series enumeration)
- [3671. Sum of Beautiful Subsequences](https://leetcode.com/problems/sum-of-beautiful-subsequences/) 2647 (multiple inclusion-exclusion)
- [2436. Minimum Split Into Subarrays With GCD Greater Than One](https://leetcode.com/problems/minimum-split-into-subarrays-with-gcd-greater-than-one/) 🔒
- [2464. Minimum Subarrays in a Valid Split](https://leetcode.com/problems/minimum-subarrays-in-a-valid-split/) 🔒
- [2941. Maximum GCD-Sum of a Subarray](https://leetcode.com/problems/maximum-gcd-sum-of-a-subarray/) 🔒 (logTrick applicable)

**Extension**:

- [2807. Insert Greatest Common Divisors in Linked List](https://leetcode.com/problems/insert-greatest-common-divisors-in-linked-list/) 1279

### §1.7 Least Common Multiple (LCM)

- [2413. Smallest Even Multiple](https://leetcode.com/problems/smallest-even-multiple/) 1145
- [3334. Find the Maximum Factor Score of Array](https://leetcode.com/problems/find-the-maximum-factor-score-of-array/) 1519
- [858. Mirror Reflection](https://leetcode.com/problems/mirror-reflection/) 1881
- [2197. Replace Non-Coprime Numbers in Array](https://leetcode.com/problems/replace-non-coprime-numbers-in-array/) 2057
- [2470. Number of Subarrays With LCM Equal to K](https://leetcode.com/problems/number-of-subarrays-with-lcm-equal-to-k/) (logTrick achieves O(n log k))

### §1.8 Coprime

- [2748. Number of Beautiful Pairs](https://leetcode.com/problems/number-of-beautiful-pairs/) 1301
- [1447. Simplified Fractions](https://leetcode.com/problems/simplified-fractions/) ~1400
- [1766. Tree of Coprimes](https://leetcode.com/problems/tree-of-coprimes/) 2232
- [3411. Maximum Subarray With Equal Products](https://leetcode.com/problems/maximum-subarray-with-equal-products/) (non-brute-force, ~2300)

### §1.9 Congruence

- [2453. Destroy Sequential Targets](https://leetcode.com/problems/destroy-sequential-targets/) 1762
- [2598. Smallest Missing Non-negative Integer After Operations](https://leetcode.com/problems/smallest-missing-non-negative-integer-after-operations/) 1846
- [1590. Make Sum Divisible by P](https://leetcode.com/problems/make-sum-divisible-by-p/) 2039

### §1.10 Number-Theoretic Block Decomposition

- [1925. Count Square Sum Triples](https://leetcode.com/problems/count-square-sum-triples/) (primitive Pythagorean triples)

### §1.11 Others

- [1018. Binary Prefix Divisible By 5](https://leetcode.com/problems/binary-prefix-divisible-by-5/) 1376
- [326. Power of Three](https://leetcode.com/problems/power-of-three/) (achieve O(1))
- [1387. Sort Integers by The Power Value](https://leetcode.com/problems/sort-integers-by-the-power-value/) 1507 (Collatz conjecture)
- [372. Super Pow](https://leetcode.com/problems/super-pow/) (Euler's theorem)
- [1015. Smallest Integer Divisible by K](https://leetcode.com/problems/smallest-integer-divisible-by-k/) (Euler's theorem; Euler's totient function)
- [3790. Smallest All-Ones Multiple](https://leetcode.com/problems/smallest-all-ones-multiple/) (same as 1015)
- [633. Sum of Square Numbers](https://leetcode.com/problems/sum-of-square-numbers/) (Fermat's theorem on sums of two squares)
- [279. Perfect Squares](https://leetcode.com/problems/perfect-squares/) (Lagrange's four-square theorem)
- [2240. Number of Ways to Buy Pens and Pencils](https://leetcode.com/problems/number-of-ways-to-buy-pens-and-pencils/) (quasi-Euclidean algorithm)

## II. Combinatorics

### §2.1 Multiplication Principle

- [3128. Right Triangles](https://leetcode.com/problems/right-triangles/) 1541
- [1573. Number of Ways to Split a String](https://leetcode.com/problems/number-of-ways-to-split-a-string/) 1591
- [2750. Ways to Split Array Into Good Subarrays](https://leetcode.com/problems/ways-to-split-array-into-good-subarrays/) 1598
- [2316. Count Unreachable Pairs of Nodes in an Undirected Graph](https://leetcode.com/problems/count-unreachable-pairs-of-nodes-in-an-undirected-graph/) 1604
- [2550. Count Collisions of Monkeys on a Polygon](https://leetcode.com/problems/count-collisions-of-monkeys-on-a-polygon/) 1663
- [1922. Count Good Numbers](https://leetcode.com/problems/count-good-numbers/) 1675
- [3067. Count Pairs of Connectable Servers in a Weighted Tree Network](https://leetcode.com/problems/count-pairs-of-connectable-servers-in-a-weighted-tree-network/) 1909
- [2147. Number of Ways to Divide a Long Corridor](https://leetcode.com/problems/number-of-ways-to-divide-a-long-corridor/) 1915
- [2963. Count the Number of Good Partitions](https://leetcode.com/problems/count-the-number-of-good-partitions/) 1985
- [2306. Naming a Company](https://leetcode.com/problems/naming-a-company/) 2305
- [2867. Count Valid Paths in a Tree](https://leetcode.com/problems/count-valid-paths-in-a-tree/) 2428
- [1617. Count Subtrees With Max Distance Between Cities](https://leetcode.com/problems/count-subtrees-with-max-distance-between-cities/) (achieve O(n³))
- [2450. Number of Distinct Binary Strings After Applying Operations](https://leetcode.com/problems/number-of-distinct-binary-strings-after-applying-operations/) 🔒

### §2.2 Combinatorial Counting

- [62. Unique Paths](https://leetcode.com/problems/unique-paths/)
- [357. Count Numbers with Unique Digits](https://leetcode.com/problems/count-numbers-with-unique-digits/)
- [1175. Prime Arrangements](https://leetcode.com/problems/prime-arrangements/) 1489
- [3179. Find the N-th Value After K Seconds](https://leetcode.com/problems/find-the-n-th-value-after-k-seconds/) (combinatorial formula)
- [1359. Count All Valid Pickup and Delivery Options](https://leetcode.com/problems/count-all-valid-pickup-and-delivery-options/) 1723
- [2400. Number of Ways to Reach a Position After Exactly k Steps](https://leetcode.com/problems/number-of-ways-to-reach-a-position-after-exactly-k-steps/) 1751
- [3558. Number of Ways to Assign Edge Weights I](https://leetcode.com/problems/number-of-ways-to-assign-edge-weights-i/) 1845
- [3821. Find Nth Smallest Integer With K One Bits](https://leetcode.com/problems/find-nth-smallest-integer-with-k-one-bits/) 2069
- [762. Prime Number of Set Bits in Binary Representation](https://leetcode.com/problems/prime-number-of-set-bits-in-binary-representation/) (non-brute-force)
- [2514. Count Anagrams](https://leetcode.com/problems/count-anagrams/) 2070
- [3154. Find Number of Ways to Reach the K-th Stair](https://leetcode.com/problems/find-number-of-ways-to-reach-the-k-th-stair/) 2071
- [1643. Kth Smallest Instructions](https://leetcode.com/problems/kth-smallest-instructions/) 2080
- [2842. Count K-Subsequences of a String With Maximum Beauty](https://leetcode.com/problems/count-k-subsequences-of-a-string-with-maximum-beauty/) 2092
- [2221. Find Triangular Sum of an Array](https://leetcode.com/problems/find-triangular-sum-of-an-array/) (extended Lucas theorem; binomial coefficients mod 10)
- [3463. Check if Digits Are Equal in String After Operations II](https://leetcode.com/problems/check-if-digits-are-equal-in-string-after-operations-ii/) 2286 (extended Lucas theorem; binomial coefficients mod 10)
- [3519. Count Numbers with Non-Decreasing Digits](https://leetcode.com/problems/count-numbers-with-non-decreasing-digits/) 2246
- [1569. Number of Ways to Reorder Array to Get Same BST](https://leetcode.com/problems/number-of-ways-to-reorder-array-to-get-same-bst/) 2288
- [3405. Count the Number of Arrays With K Matching Adjacent Elements](https://leetcode.com/problems/count-the-number-of-arrays-with-k-matching-adjacent-elements/) 2310
- [1866. Number of Ways to Rearrange Sticks With K Sticks Visible](https://leetcode.com/problems/number-of-ways-to-rearrange-sticks-with-k-sticks-visible/) 2333 (Stirling numbers of the first kind)
- [1467. Probability of a Two Boxes Having The Same Number of Distinct Balls](https://leetcode.com/problems/probability-of-a-two-boxes-having-the-same-number-of-distinct-balls/) 2357
- [3518. Smallest Palindromic Rearrangement II](https://leetcode.com/problems/smallest-palindromic-rearrangement-ii/) 2375 (trial-and-fill; permutations of a multiset)
- [3272. Find the Count of Good Integers](https://leetcode.com/problems/find-the-count-of-good-integers/) 2382
- [3317. Find the Number of Possible Ways for an Event](https://leetcode.com/problems/find-the-number-of-possible-ways-for-an-event/) 2414 (Stirling numbers of the second kind)
- [3470. Permutations IV](https://leetcode.com/problems/permutations-iv/) 2474 (construction; k-th in lexicographical order)
- [1916. Count Ways to Build Rooms in an Ant Colony](https://leetcode.com/problems/count-ways-to-build-rooms-in-an-ant-colony/) 2486
- [3343. Count Number of Balanced Permutations](https://leetcode.com/problems/count-number-of-balanced-permutations/) 2615 (permutations of a multiset)
- [1830. Minimum Number of Operations to Make String Sorted](https://leetcode.com/problems/minimum-number-of-operations-to-make-string-sorted/) 2620
- [2954. Count the Number of Infection Sequences](https://leetcode.com/problems/count-the-number-of-infection-sequences/) 2645
- [3539. Find Sum of Array Product of Magical Sequences](https://leetcode.com/problems/find-sum-of-array-product-of-magical-sequences/) 2694 (permutations of a multiset)
- [3395. Subsequences with a Unique Middle Mode I](https://leetcode.com/problems/subsequences-with-a-unique-middle-mode-i/) 2800 (achieve O(n) time)
- [1575. Count All Possible Routes](https://leetcode.com/problems/count-all-possible-routes/)
- [3251. Find the Count of Monotonic Pairs II](https://leetcode.com/problems/find-the-count-of-monotonic-pairs-ii/) (achieve O(n) time)
- [LCP 25. Antique Keyboard](https://leetcode.cn/problems/Uh984O/)
- [2539. Count the Number of Good Subsequences](https://leetcode.com/problems/count-the-number-of-good-subsequences/) 🔒
- [634. Find the Derangement of An Array](https://leetcode.com/problems/find-the-derangement-of-an-array/) 🔒
- [1692. Count Ways to Distribute Candies](https://leetcode.com/problems/count-ways-to-distribute-candies/) 🔒 (Stirling numbers of the second kind)

For generating function problems, see "§2.5 Generating Functions" in this list.

For counting DP problems, see "§7.7 Counting DP" in the [Dynamic Programming list](https://leetcode.cn/circle/discuss/tXLS3i/).

### §2.3 Balls-into-Bins (Stars and Bars)

See also: [Illustrated: Multiset Combinations](https://leetcode.cn/problems/count-ways-to-make-array-with-product/solutions/2713481/tu-jie-zhi-yin-zi-fen-jie-fang-qiu-wen-t-fboo/).

- [1641. Count Sorted Vowel Strings](https://leetcode.com/problems/count-sorted-vowel-strings/) 1519
- [1621. Number of Sets of K Non-Overlapping Line Segments](https://leetcode.com/problems/number-of-sets-of-k-non-overlapping-line-segments/) 2198
- [1735. Count Ways to Make Array With Product](https://leetcode.com/problems/count-ways-to-make-array-with-product/) 2500
- [2338. Count the Number of Ideal Arrays](https://leetcode.com/problems/count-the-number-of-ideal-arrays/) 2615

**Mind Extensions**:

- [3669. Balanced K-Factor Decomposition](https://leetcode.com/problems/balanced-k-factor-decomposition/) (not strictly a combinatorics problem, but analyzing the algorithm's running time requires combinatorics)

### §2.4 Inclusion-Exclusion Principle

Some problems below have other solutions; the difficulty ratings are for reference only.

- [2652. Sum Multiples](https://leetcode.com/problems/sum-multiples/)
- [878. Nth Magical Number](https://leetcode.com/problems/nth-magical-number/) 1897
- [1201. Ugly Number III](https://leetcode.com/problems/ugly-number-iii/) 2039
- [2929. Distribute Candies Among Children II](https://leetcode.com/problems/distribute-candies-among-children-ii/)
- [2930. Number of Strings Which Can Be Rearranged to Contain Substring](https://leetcode.com/problems/number-of-strings-which-can-be-rearranged-to-contain-substring/)
- [2513. Minimize the Maximum of Two Arrays](https://leetcode.com/problems/minimize-the-maximum-of-two-arrays/) 2302
- [3733. Minimum Time to Complete All Deliveries](https://leetcode.com/problems/minimum-time-to-complete-all-deliveries/) (same as 2513)
- [3116. Kth Smallest Amount With Single Denomination Combination](https://leetcode.com/problems/kth-smallest-amount-with-single-denomination-combination/) 2387
- [3757. Number of Effective Subsequences](https://leetcode.com/problems/number-of-effective-subsequences/) 2519
- [3130. Find All Possible Stable Binary Arrays II](https://leetcode.com/problems/find-all-possible-stable-binary-arrays-ii/) 2825
- [920. Number of Music Playlists](https://leetcode.com/problems/number-of-music-playlists/) (faster approach exists)
- [3336. Find the Number of Subsequences With Equal GCD](https://leetcode.com/problems/find-the-number-of-subsequences-with-equal-gcd/) (multiple inclusion-exclusion; Möbius function)
- [2927. Distribute Candies Among Children III](https://leetcode.com/problems/distribute-candies-among-children-iii/) 🔒

### §2.5 Generating Functions

- [1155. Number of Dice Rolls With Target Sum](https://leetcode.com/problems/number-of-dice-rolls-with-target-sum/)
- [629. K Inverse Pairs Array](https://leetcode.com/problems/k-inverse-pairs-array/)
- [3193. Count the Number of Inversions](https://leetcode.com/problems/count-the-number-of-inversions/)
- [3082. Find the Sum of the Power of All Subsequences](https://leetcode.com/problems/find-the-sum-of-the-power-of-all-subsequences/)
- [2518. Number of Great Partitions](https://leetcode.com/problems/number-of-great-partitions/)
- [3333. Find the Original Typed String II](https://leetcode.com/problems/find-the-original-typed-string-ii/)

> Note: contribution-technique problems have been moved to the Greedy & Thinking list.

## III. Probability & Expectation

- [1227. Airplane Seat Assignment Probability](https://leetcode.com/problems/airplane-seat-assignment-probability/)
- [688. Knight Probability in Chessboard](https://leetcode.com/problems/knight-probability-in-chessboard/)
- [837. New 21 Game](https://leetcode.com/problems/new-21-game/) 2350
- [1467. Probability of a Two Boxes Having The Same Number of Distinct Balls](https://leetcode.com/problems/probability-of-a-two-boxes-having-the-same-number-of-distinct-balls/) 2357
- [808. Soup Servings](https://leetcode.com/problems/soup-servings/) 2397
- [LCR 185. Probability of Dice Roll Sums](https://leetcode.cn/problems/nge-tou-zi-de-dian-shu-lcof/)
- [LCP 11. Expected Number Statistics](https://leetcode.cn/problems/qi-wang-ge-shu-tong-ji/)
- [Ubiquant-04. Chip Game](https://leetcode.cn/contest/ubiquant2022/problems/I3Gm2h/)
- [1230. Toss Strange Coins](https://leetcode.com/problems/toss-strange-coins/) 🔒

**Significantly faster algorithm on random data**:

- [3494. Find the Minimum Amount of Time to Brew Potions](https://leetcode.com/problems/find-the-minimum-amount-of-time-to-brew-potions/)

## IV. Game Theory

- [292. Nim Game](https://leetcode.com/problems/nim-game/) (Bash Game)
- [1025. Divisor Game](https://leetcode.com/problems/divisor-game/) 1435
- [3227. Vowels Game in a String](https://leetcode.com/problems/vowels-game-in-a-string/) 1452
- [2038. Remove Colored Pieces if Both Neighbors are the Same Color](https://leetcode.com/problems/remove-colored-pieces-if-both-neighbors-are-the-same-color/) 1468
- [877. Stone Game](https://leetcode.com/problems/stone-game/) 1590
- [3828. Final Element After Subarray Deletions](https://leetcode.com/problems/final-element-after-subarray-deletions/) 1591
- [1510. Stone Game IV](https://leetcode.com/problems/stone-game-iv/) 1787
- [486. Predict the Winner](https://leetcode.com/problems/predict-the-winner/)
- [1690. Stone Game VII](https://leetcode.com/problems/stone-game-vii/) 1951
- [1686. Stone Game VI](https://leetcode.com/problems/stone-game-vi/) 2001
- [1927. Sum Game](https://leetcode.com/problems/sum-game/) 2005
- [1406. Stone Game III](https://leetcode.com/problems/stone-game-iii/) 2027
- [1140. Stone Game II](https://leetcode.com/problems/stone-game-ii/) 2035
- [1563. Stone Game V](https://leetcode.com/problems/stone-game-v/) 2087
- [464. Can I Win](https://leetcode.com/problems/can-i-win/)
- [2029. Stone Game IX](https://leetcode.com/problems/stone-game-ix/) 2277
- [810. Chalkboard XOR Game](https://leetcode.com/problems/chalkboard-xor-game/) 2341
- [1872. Stone Game VIII](https://leetcode.com/problems/stone-game-viii/) 2440
- [913. Cat and Mouse](https://leetcode.com/problems/cat-and-mouse/) (actual difficulty ~2800)
- [1728. Cat and Mouse II](https://leetcode.com/problems/cat-and-mouse-ii/) 2849
- [LCP 48. Infinite Chessboard](https://leetcode.cn/problems/fsa7oZ/)
- [294. Flip Game II](https://leetcode.com/problems/flip-game-ii/) 🔒
- [1908. Game of Nim](https://leetcode.com/problems/game-of-nim/) 🔒
- [2005. Subtree Removal Game with Fibonacci Tree](https://leetcode.com/problems/subtree-removal-game-with-fibonacci-tree/) 🔒
- [2868. The Wording Game](https://leetcode.com/problems/the-wording-game/) 🔒

## V. Computational Geometry

### §5.1 Points and Lines

- [1232. Check If It Is a Straight Line](https://leetcode.com/problems/check-if-it-is-a-straight-line/) 1247
- [2280. Minimum Lines to Represent a Line Chart](https://leetcode.com/problems/minimum-lines-to-represent-a-line-chart/) 1681
- [1610. Maximum Number of Visible Points](https://leetcode.com/problems/maximum-number-of-visible-points/) 2147
- [Interview 16.03. Intersection](https://leetcode.com/problems/intersection-lcci/)
- [Interview 16.13. Bisect Squares](https://leetcode.com/problems/bisect-squares-lcci/)
- [Interview 16.14. Best Line](https://leetcode.com/problems/best-line-lcci/)
- [LCP 37. Minimum Rectangle Area](https://leetcode.cn/problems/zui-xiao-ju-xing-mian-ji/)
- [2152. Minimum Number of Lines to Cover Points](https://leetcode.com/problems/minimum-number-of-lines-to-cover-points/) 🔒

### §5.2 Circles

- [1401. Circle and Rectangle Overlapping](https://leetcode.com/problems/circle-and-rectangle-overlapping/) 1709
- [1453. Maximum Number of Darts Inside of a Circular Dartboard](https://leetcode.com/problems/maximum-number-of-darts-inside-of-a-circular-dartboard/) 2202
- [LCP 42. Toy Ring Toss](https://leetcode.cn/problems/vFjcfV/)
- [3235. Check if the Rectangle Corner Is Reachable](https://leetcode.com/problems/check-if-the-rectangle-corner-is-reachable/)
- [1924. Erect the Fence II](https://leetcode.com/problems/erect-the-fence-ii/) 🔒 (smallest enclosing circle; Welzl's algorithm)

### §5.3 Rectangles and Polygons

- [836. Rectangle Overlap](https://leetcode.com/problems/rectangle-overlap/) 1443
- [223. Rectangle Area](https://leetcode.com/problems/rectangle-area/)
- [593. Valid Square](https://leetcode.com/problems/valid-square/)
- [939. Minimum Area Rectangle](https://leetcode.com/problems/minimum-area-rectangle/) 1752
- [963. Minimum Area Rectangle II](https://leetcode.com/problems/minimum-area-rectangle-ii/) 1991
- [3625. Count Number of Trapezoids II](https://leetcode.com/problems/count-number-of-trapezoids-ii/) 2643
- [469. Convex Polygon](https://leetcode.com/problems/convex-polygon/) 🔒

### §5.4 Convex Hull

- [587. Erect the Fence](https://leetcode.com/problems/erect-the-fence/)
- [812. Largest Triangle Area](https://leetcode.com/problems/largest-triangle-area/) (rotating calipers)
- [LCP 15. Amusement Park Maze](https://leetcode.cn/problems/you-le-yuan-de-mi-gong/)

See also "§11.7 Slope Trick DP" in the [Dynamic Programming list](https://leetcode.cn/circle/discuss/tXLS3i/).

## VI. Randomized Algorithms

### §6.1 Random Numbers

- [398. Random Pick Index](https://leetcode.com/problems/random-pick-index/)
- [382. Linked List Random Node](https://leetcode.com/problems/linked-list-random-node/)
- [384. Shuffle an Array](https://leetcode.com/problems/shuffle-an-array/)
- [380. Insert Delete GetRandom O(1)](https://leetcode.com/problems/insert-delete-getrandom-o1/)
- [381. Insert Delete GetRandom O(1) - Duplicates Allowed](https://leetcode.com/problems/insert-delete-getrandom-o1-duplicates-allowed/)
- [528. Random Pick with Weight](https://leetcode.com/problems/random-pick-with-weight/)
- [470. Implement Rand10() Using Rand7()](https://leetcode.com/problems/implement-rand10-using-rand7/)
- [710. Random Pick with Blacklist](https://leetcode.com/problems/random-pick-with-blacklist/)
- [478. Generate Random Point in a Circle](https://leetcode.com/problems/generate-random-point-in-a-circle/)
- [497. Random Point in Non-overlapping Rectangles](https://leetcode.com/problems/random-point-in-non-overlapping-rectangles/)
- [519. Random Flip Matrix](https://leetcode.com/problems/random-flip-matrix/)

### §6.2 Randomization Techniques

- [961. N-Repeated Element in Size 2N Array](https://leetcode.com/problems/n-repeated-element-in-size-2n-array/) 1162
- [1317. Convert Integer to the Sum of Two No-Zero Integers](https://leetcode.com/problems/convert-integer-to-the-sum-of-two-no-zero-integers/) 1278
- [1968. Array With Elements Not Equal to Average of Neighbors](https://leetcode.com/problems/array-with-elements-not-equal-to-average-of-neighbors/) 1499
- [1157. Online Majority Element In Subarray](https://leetcode.com/problems/online-majority-element-in-subarray/) 2205
- [3680. Generate Schedule](https://leetcode.com/problems/generate-schedule/) 2378

## VII. Miscellaneous

### §7.1 Palindromic Numbers

- [9. Palindrome Number](https://leetcode.com/problems/palindrome-number/)
- [2396. Strictly Palindromic Number](https://leetcode.com/problems/strictly-palindromic-number/) 1329
- [2217. Find Palindrome With Fixed Length](https://leetcode.com/problems/find-palindrome-with-fixed-length/) 1822
- [866. Prime Palindrome](https://leetcode.com/problems/prime-palindrome/) 1938
- [3766. Minimum Operations to Make Binary Palindrome](https://leetcode.com/problems/minimum-operations-to-make-binary-palindrome/) (non-brute-force)
- [564. Find the Closest Palindrome](https://leetcode.com/problems/find-the-closest-palindrome/)
- [2967. Minimum Cost to Make Array Equalindromic](https://leetcode.com/problems/minimum-cost-to-make-array-equalindromic/) 2116
- [906. Super Palindromes](https://leetcode.com/problems/super-palindromes/) 2140
- [2081. Sum of k-Mirror Numbers](https://leetcode.com/problems/sum-of-k-mirror-numbers/) 2210
- [3677. Count Binary Palindromic Numbers](https://leetcode.com/problems/count-binary-palindromic-numbers/) 2223
- [3260. Find the Largest Palindrome Divisible by K](https://leetcode.com/problems/find-the-largest-palindrome-divisible-by-k/) 2370
- [3272. Find the Count of Good Integers](https://leetcode.com/problems/find-the-count-of-good-integers/) 2382
- [3646. Next Special Palindrome Number](https://leetcode.com/problems/next-special-palindrome-number/) 2445
- [479. Largest Palindrome Product](https://leetcode.com/problems/largest-palindrome-product/)

### §7.2 Integer Breaking

- [343. Integer Break](https://leetcode.com/problems/integer-break/)
- [1808. Maximize Number of Nice Divisors](https://leetcode.com/problems/maximize-number-of-nice-divisors/) 2070

### §7.3 Manhattan Distance and Chebyshev Distance

- [1266. Minimum Time Visiting All Points](https://leetcode.com/problems/minimum-time-visiting-all-points/) 1303
- [3443. Maximum Manhattan Distance After K Changes](https://leetcode.com/problems/maximum-manhattan-distance-after-k-changes/) 1856
- [1131. Maximum of Absolute Value Expression](https://leetcode.com/problems/maximum-of-absolute-value-expression/) 2059
- [3102. Minimize Manhattan Distances](https://leetcode.com/problems/minimize-manhattan-distances/) 2216 (Manhattan distance → Chebyshev distance)
- [1330. Reverse Subarray To Maximize Array Value](https://leetcode.com/problems/reverse-subarray-to-maximize-array-value/) 2482
- [3464. Maximize the Distance Between Points on a Square](https://leetcode.com/problems/maximize-the-distance-between-points-on-a-square/) 2806
- [1956. Minimum Time For K Virus Variants to Spread](https://leetcode.com/problems/minimum-time-for-k-virus-variants-to-spread/) 🔒
- [2613. Beautiful Pairs](https://leetcode.com/problems/beautiful-pairs/) 🔒

### §7.4 Polynomials

- [611. Valid Triangle Number](https://leetcode.com/problems/valid-triangle-number/) (achieve O(n + U log U))
- [923. 3Sum With Multiplicity](https://leetcode.com/problems/3sum-with-multiplicity/) (achieve O(n + U log U))
- [835. Image Overlap](https://leetcode.com/problems/image-overlap/)
- [3549. Multiply Two Polynomials](https://leetcode.com/problems/multiply-two-polynomials/) 🔒 (FFT template)
- [259. 3Sum Smaller](https://leetcode.com/problems/3sum-smaller/) 🔒 (achieve O(n + U log U))
- [3078. Match Alphanumerical Pattern in Matrix I](https://leetcode.com/problems/match-alphanumerical-pattern-in-matrix-i/) 🔒
- [3400. Maximum Number of Matching Indices After Right Shifts](https://leetcode.com/problems/maximum-number-of-matching-indices-after-right-shifts/) 🔒 (square root decomposition)

See also "§2.5 Generating Functions" in this list.

### §7.5 Fast Walsh–Hadamard Transform (FWT)

- [3514. Number of Unique XOR Triplets II](https://leetcode.com/problems/number-of-unique-xor-triplets-ii/)
- [1723. Find Minimum Time to Finish All Jobs](https://leetcode.com/problems/find-minimum-time-to-finish-all-jobs/)

### §7.6 Linear Basis

See the [Bit Manipulation list](https://leetcode.cn/circle/discuss/dHn9Vk/).

### §7.7 Boyer–Moore Voting Algorithm

- [169. Majority Element](https://leetcode.com/problems/majority-element/)
- [961. N-Repeated Element in Size 2N Array](https://leetcode.com/problems/n-repeated-element-in-size-2n-array/)
- [2780. Minimum Index of a Valid Split](https://leetcode.com/problems/minimum-index-of-a-valid-split/) 1550
- [229. Majority Element II](https://leetcode.com/problems/majority-element-ii/)
- [1157. Online Majority Element In Subarray](https://leetcode.com/problems/online-majority-element-in-subarray/) 2205

### §7.8 Others

- [1523. Count Odd Numbers in an Interval Range](https://leetcode.com/problems/count-odd-numbers-in-an-interval-range/) 1209
- [1716. Calculate Money in Leetcode Bank](https://leetcode.com/problems/calculate-money-in-leetcode-bank/) 1295
- [2829. Determine the Minimum Sum of a k-avoiding Array](https://leetcode.com/problems/determine-the-minimum-sum-of-a-k-avoiding-array/) 1347
- [2579. Count Total Number of Colored Cells](https://leetcode.com/problems/count-total-number-of-colored-cells/) 1356
- [3648. Minimum Sensors to Cover Grid](https://leetcode.com/problems/minimum-sensors-to-cover-grid/) 1396
- [2834. Find the Minimum Possible Sum of a Beautiful Array](https://leetcode.com/problems/find-the-minimum-possible-sum-of-a-beautiful-array/) 1409
- [1414. Find the Minimum Number of Fibonacci Numbers Whose Sum Is K](https://leetcode.com/problems/find-the-minimum-number-of-fibonacci-numbers-whose-sum-is-k/) 1466
- [319. Bulb Switcher](https://leetcode.com/problems/bulb-switcher/) (~1500)
- [1780. Check if Number is a Sum of Powers of Three](https://leetcode.com/problems/check-if-number-is-a-sum-of-powers-of-three/) 1506
- [3091. Apply Operations to Make Sum of Array Greater Than or Equal to K](https://leetcode.com/problems/apply-operations-to-make-sum-of-array-greater-than-or-equal-to-k/) 1522
- [3468. Find the Number of Copy Arrays](https://leetcode.com/problems/find-the-number-of-copy-arrays/) 1545 (mathematical derivation)
- [2310. Sum of Numbers With Units Digit K](https://leetcode.com/problems/sum-of-numbers-with-units-digit-k/) 1559
- [2145. Count the Hidden Sequences](https://leetcode.com/problems/count-the-hidden-sequences/) 1614 (mathematical derivation)
- [2541. Minimum Operations to Make Array Equal II](https://leetcode.com/problems/minimum-operations-to-make-array-equal-ii/) 1620
- [1502. Can Make Arithmetic Progression From Sequence](https://leetcode.com/problems/can-make-arithmetic-progression-from-sequence/) (achieve O(n))
- [2195. Append K Integers With Minimal Sum](https://leetcode.com/problems/append-k-integers-with-minimal-sum/) 1659
- [2457. Minimum Addition to Make Integer Beautiful](https://leetcode.com/problems/minimum-addition-to-make-integer-beautiful/) 1680
- [1017. Convert to Base -2](https://leetcode.com/problems/convert-to-base-2/) 1698
- [3649. Number of Perfect Pairs](https://leetcode.com/problems/number-of-perfect-pairs/) 1716 (geometric meaning of absolute value)
- [1954. Minimum Garden Perimeter to Collect Enough Apples](https://leetcode.com/problems/minimum-garden-perimeter-to-collect-enough-apples/) 1759
- [1073. Adding Two Negabinary Numbers](https://leetcode.com/problems/adding-two-negabinary-numbers/) 1807
- [1823. Find the Winner of the Circular Game](https://leetcode.com/problems/find-the-winner-of-the-circular-game/) (Josephus problem)
- [166. Fraction to Recurring Decimal](https://leetcode.com/problems/fraction-to-recurring-decimal/) (has a math-based approach that avoids a hash table)
- [3012. Minimize Length of Array Using Operations](https://leetcode.com/problems/minimize-length-of-array-using-operations/) 1833
- [483. Smallest Good Base](https://leetcode.com/problems/smallest-good-base/)
- [3782. Last Remaining Integer After Alternating Deletion Operations](https://leetcode.com/problems/last-remaining-integer-after-alternating-deletion-operations/) 2074
- [390. Elimination Game](https://leetcode.com/problems/elimination-game/) (similar to 3782)
- [972. Equal Rational Numbers](https://leetcode.com/problems/equal-rational-numbers/) 2121
- [1515. Best Position for a Service Centre](https://leetcode.com/problems/best-position-for-a-service-centre/) 2157 (convex optimization; gradient descent)
- [1862. Sum of Floored Pairs](https://leetcode.com/problems/sum-of-floored-pairs/) 2170 (harmonic series enumeration)
- [1739. Building Boxes](https://leetcode.com/problems/building-boxes/) 2198
- [2443. Sum of Number and Its Reverse](https://leetcode.com/problems/sum-of-number-and-its-reverse/) (non-brute-force)
- [1806. Minimum Number of Operations to Reinitialize a Permutation](https://leetcode.com/problems/minimum-number-of-operations-to-reinitialize-a-permutation/) (non-brute-force)
- [458. Poor Pigs](https://leetcode.com/problems/poor-pigs/)
- [60. Permutation Sequence](https://leetcode.com/problems/permutation-sequence/)
- [2117. Abbreviating the Product of a Range](https://leetcode.com/problems/abbreviating-the-product-of-a-range/) 2477
- [3666. Minimum Operations to Equalize Binary String](https://leetcode.com/problems/minimum-operations-to-equalize-binary-string/) 2477 (Gale–Ryser theorem)
- [LCP 02. Fraction Simplification](https://leetcode.cn/problems/deep-dark-fraction/) (continued fractions)
- [LCP 29. Orchestra Layout](https://leetcode.cn/problems/SNJvJP/)
- [LCP 46. Volunteer Deployment](https://leetcode.cn/problems/05ZEDJ/) (solve equations)
- [800. Similar RGB Color](https://leetcode.com/problems/similar-rgb-color/) 🔒
- [660. Remove 9](https://leetcode.com/problems/remove-9/) 🔒
- [2979. Most Expensive Item That Can Not Be Bought](https://leetcode.com/problems/most-expensive-item-that-can-not-be-bought/) 🔒
- [2647. Color the Triangle Red](https://leetcode.com/problems/color-the-triangle-red/) 🔒

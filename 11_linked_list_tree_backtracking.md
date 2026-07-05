# Linked List, Binary Tree & Backtracking

Problem list from [0x3F's LeetCode Study Plan](https://leetcode.cn/circle/discuss/K0n2gO/) — Linked List, Binary Tree & Backtracking (Front/Back Pointers/Fast-Slow Pointers/DFS/BFS/Diameter/LCA/General Trees).

## I. Linked List

> Note: since contest linked-list problems can usually be converted to array problems, which are easier to work with than the actual linked list, no difficulty ratings are given below.

Work through the problems below while thinking about:

1. When do you need a sentinel/dummy node?
2. When should the loop condition be `while (node != null)`? When should it be `while (node.next != null)`?

### §1.1 Traversing a Linked List

- [1290. Convert Binary Number in a Linked List to Integer](https://leetcode.com/problems/convert-binary-number-in-a-linked-list-to-integer/)
- [2058. Find the Minimum and Maximum Number of Nodes Between Critical Points](https://leetcode.com/problems/find-the-minimum-and-maximum-number-of-nodes-between-critical-points/)
- [2181. Merge Nodes in Between Zeros](https://leetcode.com/problems/merge-nodes-in-between-zeros/)
- [725. Split Linked List in Parts](https://leetcode.com/problems/split-linked-list-in-parts/)
- [817. Linked List Components](https://leetcode.com/problems/linked-list-components/)
- [3263. Convert Doubly Linked List to Array I](https://leetcode.com/problems/convert-doubly-linked-list-to-array-i/) 🔒
- [3294. Convert Doubly Linked List to Array II](https://leetcode.com/problems/convert-doubly-linked-list-to-array-ii/) 🔒
- [3062. Winner of the Linked List Game](https://leetcode.com/problems/winner-of-the-linked-list-game/) 🔒
- [3063. Linked List Frequency](https://leetcode.com/problems/linked-list-frequency/) 🔒

### §1.2 Deleting Nodes

[Video Explanation: Basic Algorithms Lecture 08](https://leetcode.cn/link/?target=https%3A%2F%2Fwww.bilibili.com%2Fvideo%2FBV1VP4y1Q71e%2F)

- [203. Remove Linked List Elements](https://leetcode.com/problems/remove-linked-list-elements/)
- [3217. Delete Nodes from Linked List Present in Array](https://leetcode.com/problems/delete-nodes-from-linked-list-present-in-array/)
- [83. Remove Duplicates from Sorted List](https://leetcode.com/problems/remove-duplicates-from-sorted-list/)
- [82. Remove Duplicates from Sorted List II](https://leetcode.com/problems/remove-duplicates-from-sorted-list-ii/)
- [237. Delete Node in a Linked List](https://leetcode.com/problems/delete-node-in-a-linked-list/)
- [1669. Merge in Between Linked Lists](https://leetcode.com/problems/merge-in-between-linked-lists/)
- [2487. Remove Nodes from Linked List](https://leetcode.com/problems/remove-nodes-from-linked-list/)
- [1836. Remove Duplicates from an Unsorted Linked List](https://leetcode.com/problems/remove-duplicates-from-an-unsorted-linked-list/) 🔒

### §1.3 Inserting Nodes

- [2807. Insert Greatest Common Divisors in Linked List](https://leetcode.com/problems/insert-greatest-common-divisors-in-linked-list/)
- [147. Insertion Sort List](https://leetcode.com/problems/insertion-sort-list/)
- [LCR 029. Insertion into a Circular Sorted List](https://leetcode.com/problems/4ueAj6/)
- [708. Insert Into a Sorted Circular Linked List](https://leetcode.com/problems/insert-into-a-sorted-circular-linked-list/) 🔒
- [2046. Sort Linked List Already Sorted Using Absolute Values](https://leetcode.com/problems/sort-linked-list-already-sorted-using-absolute-values/) 🔒

### §1.4 Reversing a Linked List

[Video Explanation: Basic Algorithms Lecture 06](https://leetcode.cn/link/?target=https%3A%2F%2Fwww.bilibili.com%2Fvideo%2FBV1sd4y1x7KN%2F)

- [206. Reverse Linked List](https://leetcode.com/problems/reverse-linked-list/)
- [92. Reverse Linked List II](https://leetcode.com/problems/reverse-linked-list-ii/)
- [24. Swap Nodes in Pairs](https://leetcode.com/problems/swap-nodes-in-pairs/)
- [25. Reverse Nodes in K Group](https://leetcode.com/problems/reverse-nodes-in-k-group/)
- [2074. Reverse Nodes in Even Length Groups](https://leetcode.com/problems/reverse-nodes-in-even-length-groups/)

### §1.5 Front/Back Pointers

[Video Explanation: Basic Algorithms Lecture 08](https://leetcode.cn/link/?target=https%3A%2F%2Fwww.bilibili.com%2Fvideo%2FBV1VP4y1Q71e%2F)

- [19. Remove Nth Node from End of List](https://leetcode.com/problems/remove-nth-node-from-end-of-list/)
- [61. Rotate List](https://leetcode.com/problems/rotate-list/)
- [1721. Swapping Nodes in a Linked List](https://leetcode.com/problems/swapping-nodes-in-a-linked-list/)
- [1474. Delete N Nodes After M Nodes of a Linked List](https://leetcode.com/problems/delete-n-nodes-after-m-nodes-of-a-linked-list/) 🔒

### §1.6 Fast/Slow Pointers

[Video Explanation: Basic Algorithms Lecture 07](https://leetcode.cn/link/?target=https%3A%2F%2Fwww.bilibili.com%2Fvideo%2FBV1KG4y1G7cu%2F)

- [876. Middle of the Linked List](https://leetcode.com/problems/middle-of-the-linked-list/)
- [2095. Delete the Middle Node of a Linked List](https://leetcode.com/problems/delete-the-middle-node-of-a-linked-list/)
- [234. Palindrome Linked List](https://leetcode.com/problems/palindrome-linked-list/)
- [2130. Maximum Twin Sum of a Linked List](https://leetcode.com/problems/maximum-twin-sum-of-a-linked-list/)
- [143. Reorder List](https://leetcode.com/problems/reorder-list/)
- [141. Linked List Cycle](https://leetcode.com/problems/linked-list-cycle/)
- [142. Linked List Cycle II](https://leetcode.com/problems/linked-list-cycle-ii/)
- [457. Circular Array Loop](https://leetcode.com/problems/circular-array-loop/)
- [2674. Split a Circular Linked List](https://leetcode.com/problems/split-a-circular-linked-list/) 🔒

**Mind Extensions**:

- [287. Find the Duplicate Number](https://leetcode.com/problems/find-the-duplicate-number/)
- [1015. Smallest Integer Divisible by K](https://leetcode.com/problems/smallest-integer-divisible-by-k/)
- [3790. Smallest All-Ones Multiple](https://leetcode.com/problems/smallest-all-ones-multiple/) (same as 1015)

### §1.7 Two Pointers

- [328. Odd Even Linked List](https://leetcode.com/problems/odd-even-linked-list/)
- [86. Partition List](https://leetcode.com/problems/partition-list/)
- [160. Intersection of Two Linked Lists](https://leetcode.com/problems/intersection-of-two-linked-lists/)

### §1.8 Merging Linked Lists

- [2. Add Two Numbers](https://leetcode.com/problems/add-two-numbers/)
- [445. Add Two Numbers II](https://leetcode.com/problems/add-two-numbers-ii/)
- [2816. Double a Number Represented as a Linked List](https://leetcode.com/problems/double-a-number-represented-as-a-linked-list/)
- [21. Merge Two Sorted Lists](https://leetcode.com/problems/merge-two-sorted-lists/)
- [369. Plus One Linked List](https://leetcode.com/problems/plus-one-linked-list/) 🔒
- [1634. Add Two Polynomials Represented as Linked Lists](https://leetcode.com/problems/add-two-polynomials-represented-as-linked-lists/) 🔒

### §1.9 Divide and Conquer

- [23. Merge K Sorted Lists](https://leetcode.com/problems/merge-k-sorted-lists/) (can also use a heap)
- [148. Sort List](https://leetcode.com/problems/sort-list/)

### §1.10 Comprehensive Applications

- [1019. Next Greater Node In Linked List](https://leetcode.com/problems/next-greater-node-in-linked-list/)
- [1171. Remove Zero Sum Consecutive Nodes from Linked List](https://leetcode.com/problems/remove-zero-sum-consecutive-nodes-from-linked-list/)
- [707. Design Linked List](https://leetcode.com/problems/design-linked-list/)
- [146. LRU Cache](https://leetcode.com/problems/lru-cache/)
- [460. LFU Cache](https://leetcode.com/problems/lfu-cache/)
- [432. All O(1) Data Structure](https://leetcode.com/problems/all-oone-data-structure/)
- [1206. Design Skiplist](https://leetcode.com/problems/design-skiplist/)

### §1.11 Others

- [138. Copy List With Random Pointer](https://leetcode.com/problems/copy-list-with-random-pointer/)
- [382. Linked List Random Node](https://leetcode.com/problems/linked-list-random-node/)
- [430. Flatten a Multilevel Doubly Linked List](https://leetcode.com/problems/flatten-a-multilevel-doubly-linked-list/)
- [1265. Print Immutable Linked List in Reverse](https://leetcode.com/problems/print-immutable-linked-list-in-reverse/) 🔒

## II. Binary Tree

**Learn recursion by starting with binary trees.**

If recursion makes your head spin, watch [Basic Algorithms Lecture 09](https://leetcode.cn/link/?target=https%3A%2F%2Fwww.bilibili.com%2Fvideo%2FBV1UD4y1Y769%2F) first — likes are welcome~

There are generally three traversal orders:

- **Preorder traversal**: see §2.2 Top-Down DFS.
- **Inorder traversal**: see §2.9 Binary Search Tree (BST).
- **Postorder traversal**: see §2.3 Bottom-Up DFS.

Work through the problems below while thinking about:

1. Generally, the recursion base case for DFS is a null node. When do you additionally need to treat a **leaf node** as a base case?
2. When does the DFS need a return value? When doesn't it?
3. When is a problem better solved **top-down**? When is it better solved **bottom-up**?

### §2.1 Traversing a Binary Tree

- [144. Binary Tree Preorder Traversal](https://leetcode.com/problems/binary-tree-preorder-traversal/)
- [94. Binary Tree Inorder Traversal](https://leetcode.com/problems/binary-tree-inorder-traversal/)
- [145. Binary Tree Postorder Traversal](https://leetcode.com/problems/binary-tree-postorder-traversal/)
- [872. Leaf Similar Trees](https://leetcode.com/problems/leaf-similar-trees/) 1288
- [LCP 44. Opening Ceremony Fireworks](https://leetcode.cn/problems/sZ59z6/)
- [404. Sum of Left Leaves](https://leetcode.com/problems/sum-of-left-leaves/)
- [671. Second Minimum Node in a Binary Tree](https://leetcode.com/problems/second-minimum-node-in-a-binary-tree/)
- [1469. Find All the Lonely Nodes](https://leetcode.com/problems/find-all-the-lonely-nodes/) 🔒
- [1214. Two Sum BSTs](https://leetcode.com/problems/two-sum-bsts/) 🔒
- [2764. Is Array a Preorder of Some Binary Tree](https://leetcode.com/problems/is-array-a-preorder-of-some-binary-tree/) 🔒

### §2.2 Top-Down DFS (Preorder Traversal)

Update the state on the way down (the "descent").

> Some problems can be solved either top-down or bottom-up. Some can also be solved with BFS.

- [104. Maximum Depth of Binary Tree](https://leetcode.com/problems/maximum-depth-of-binary-tree/)
- [111. Minimum Depth of Binary Tree](https://leetcode.com/problems/minimum-depth-of-binary-tree/)
- [112. Path Sum](https://leetcode.com/problems/path-sum/)
- [129. Sum Root to Leaf Numbers](https://leetcode.com/problems/sum-root-to-leaf-numbers/)
- [199. Binary Tree Right Side View](https://leetcode.com/problems/binary-tree-right-side-view/)
- [1448. Count Good Nodes in Binary Tree](https://leetcode.com/problems/count-good-nodes-in-binary-tree/) 1360
- [1315. Sum of Nodes With Even Valued Grandparent](https://leetcode.com/problems/sum-of-nodes-with-even-valued-grandparent/) 1427
- [988. Smallest String Starting from Leaf](https://leetcode.com/problems/smallest-string-starting-from-leaf/) 1429
- [1026. Maximum Difference Between Node and Ancestor](https://leetcode.com/problems/maximum-difference-between-node-and-ancestor/) 1446
- [1022. Sum of Root to Leaf Binary Numbers](https://leetcode.com/problems/sum-of-root-to-leaf-binary-numbers/) 1462
- [623. Add One Row to Tree](https://leetcode.com/problems/add-one-row-to-tree/)
- [1372. Longest Zigzag Path in a Binary Tree](https://leetcode.com/problems/longest-zigzag-path-in-a-binary-tree/) 1713
- [971. Flip Binary Tree to Match Preorder Traversal](https://leetcode.com/problems/flip-binary-tree-to-match-preorder-traversal/) 1787 (there is a simpler approach)
- [2689. Extract Kth Character from the Rope Tree](https://leetcode.com/problems/extract-kth-character-from-the-rope-tree/) 🔒
- [298. Binary Tree Longest Consecutive Sequence](https://leetcode.com/problems/binary-tree-longest-consecutive-sequence/) 🔒
- [1430. Check If a String is a Valid Sequence from Root to Leaves Path in a Binary Tree](https://leetcode.com/problems/check-if-a-string-is-a-valid-sequence-from-root-to-leaves-path-in-a-binary-tree/) 🔒
- [545. Boundary of Binary Tree](https://leetcode.com/problems/boundary-of-binary-tree/) 🔒

### §2.3 Bottom-Up DFS (Postorder Traversal)

Compute the answer on the way back up (the "ascent").

[Video Explanation: Basic Algorithms Lecture 10 — how to flexibly apply recursion](https://leetcode.cn/link/?target=https%3A%2F%2Fwww.bilibili.com%2Fvideo%2FBV18M411z7bb%2F)

- [104. Maximum Depth of Binary Tree](https://leetcode.com/problems/maximum-depth-of-binary-tree/)
- [111. Minimum Depth of Binary Tree](https://leetcode.com/problems/minimum-depth-of-binary-tree/)
- [965. Univalued Binary Tree](https://leetcode.com/problems/univalued-binary-tree/) 1178
- [100. Same Tree](https://leetcode.com/problems/same-tree/)
- [101. Symmetric Tree](https://leetcode.com/problems/symmetric-tree/)
- [951. Flip Equivalent Binary Trees](https://leetcode.com/problems/flip-equivalent-binary-trees/)
- [1379. Find a Corresponding Node of a Binary Tree in a Clone of That Tree](https://leetcode.com/problems/find-a-corresponding-node-of-a-binary-tree-in-a-clone-of-that-tree/)
- [110. Balanced Binary Tree](https://leetcode.com/problems/balanced-binary-tree/)
- [226. Invert Binary Tree](https://leetcode.com/problems/invert-binary-tree/)
- [617. Merge Two Binary Trees](https://leetcode.com/problems/merge-two-binary-trees/)
- [2331. Evaluate Boolean Binary Tree](https://leetcode.com/problems/evaluate-boolean-binary-tree/) 1304
- [508. Most Frequent Subtree Sum](https://leetcode.com/problems/most-frequent-subtree-sum/) (without using external variables)
- [563. Binary Tree Tilt](https://leetcode.com/problems/binary-tree-tilt/)
- [606. Construct String from Binary Tree](https://leetcode.com/problems/construct-string-from-binary-tree/)
- [2265. Count Nodes Equal to Average of Subtree](https://leetcode.com/problems/count-nodes-equal-to-average-of-subtree/) 1473
- [1026. Maximum Difference Between Node and Ancestor](https://leetcode.com/problems/maximum-difference-between-node-and-ancestor/) (multiple approaches)
- [3319. Kth Largest Perfect Subtree Size in Binary Tree](https://leetcode.com/problems/k-th-largest-perfect-subtree-size-in-binary-tree/) 1603
- [1339. Maximum Product of Splitted Binary Tree](https://leetcode.com/problems/maximum-product-of-splitted-binary-tree/) 1675
- [1372. Longest Zigzag Path in a Binary Tree](https://leetcode.com/problems/longest-zigzag-path-in-a-binary-tree/) 1713
- [1145. Binary Tree Coloring Game](https://leetcode.com/problems/binary-tree-coloring-game/) 1741
- [572. Subtree of Another Tree](https://leetcode.com/problems/subtree-of-another-tree/) (achieve O(n) time)
- [1530. Number of Good Leaf Nodes Pairs](https://leetcode.com/problems/number-of-good-leaf-nodes-pairs/) (achieve better than O(n²) time)
- [LCP 67. Decorate the Tree](https://leetcode.cn/problems/KnLfVT/)
- [298. Binary Tree Longest Consecutive Sequence](https://leetcode.com/problems/binary-tree-longest-consecutive-sequence/) 🔒
- [250. Count Univalue Subtrees](https://leetcode.com/problems/count-univalue-subtrees/) 🔒
- [1973. Count Nodes Equal to Sum of Descendants](https://leetcode.com/problems/count-nodes-equal-to-sum-of-descendants/) 🔒
- [663. Equal Tree Partition](https://leetcode.com/problems/equal-tree-partition/) 🔒
- [1120. Maximum Average Subtree](https://leetcode.com/problems/maximum-average-subtree/) 🔒
- [2792. Count Nodes That Are Great Enough](https://leetcode.com/problems/count-nodes-that-are-great-enough/) 🔒
- [333. Largest BST Subtree](https://leetcode.com/problems/largest-bst-subtree/) 🔒
- [366. Find Leaves of Binary Tree](https://leetcode.com/problems/find-leaves-of-binary-tree/) 🔒
- [156. Binary Tree Upside Down](https://leetcode.com/problems/binary-tree-upside-down/) 🔒
- [1612. Check If Two Expression Trees Are Equivalent](https://leetcode.com/problems/check-if-two-expression-trees-are-equivalent/) 🔒

### §2.4 Bottom-Up DFS: Deleting Nodes

- [814. Binary Tree Pruning](https://leetcode.com/problems/binary-tree-pruning/) 1380
- [1325. Delete Leaves With a Given Value](https://leetcode.com/problems/delete-leaves-with-a-given-value/) 1407
- [1110. Delete Nodes and Return Forest](https://leetcode.com/problems/delete-nodes-and-return-forest/) 1511

### §2.5 Combined Top-Down and Bottom-Up DFS

- [538. Convert BST to Greater Tree](https://leetcode.com/problems/convert-bst-to-greater-tree/) 1375 (can also use an external variable to track the sum)
- [1038. Binary Search Tree to Greater Sum Tree](https://leetcode.com/problems/binary-search-tree-to-greater-sum-tree/) (same as 538)
- [865. Smallest Subtree With All the Deepest Nodes](https://leetcode.com/problems/smallest-subtree-with-all-the-deepest-nodes/) 1534 (can also be done bottom-up)
- [1080. Insufficient Nodes in Root to Leaf Paths](https://leetcode.com/problems/insufficient-nodes-in-root-to-leaf-paths/) 1805

### §2.6 Diameter of a Binary Tree

[Video Explanation: Basic Algorithms Lecture 23](https://leetcode.cn/link/?target=https%3A%2F%2Fwww.bilibili.com%2Fvideo%2FBV17o4y187h1%2F)

- [543. Diameter of Binary Tree](https://leetcode.com/problems/diameter-of-binary-tree/)
- [687. Longest Univalue Path](https://leetcode.com/problems/longest-univalue-path/)
- [124. Binary Tree Maximum Path Sum](https://leetcode.com/problems/binary-tree-maximum-path-sum/)
- [2385. Amount of Time for Binary Tree to Be Infected](https://leetcode.com/problems/amount-of-time-for-binary-tree-to-be-infected/) 1711
- [549. Binary Tree Longest Consecutive Sequence II](https://leetcode.com/problems/binary-tree-longest-consecutive-sequence-ii/) 🔒

See also "§3.5 Diameter of a Tree" in this list.

### §2.7 Backtracking

- [257. Binary Tree Paths](https://leetcode.com/problems/binary-tree-paths/)
- [113. Path Sum II](https://leetcode.com/problems/path-sum-ii/)
- [1457. Pseudo Palindromic Paths in a Binary Tree](https://leetcode.com/problems/pseudo-palindromic-paths-in-a-binary-tree/) 1405
- [437. Path Sum III](https://leetcode.com/problems/path-sum-iii/)

### §2.8 Lowest Common Ancestor (LCA)

[Video Explanation: Basic Algorithms Lecture 12](https://leetcode.cn/link/?target=https%3A%2F%2Fwww.bilibili.com%2Fvideo%2FBV1W44y1Z7AR%2F)

- [235. Lowest Common Ancestor of a Binary Search Tree](https://leetcode.com/problems/lowest-common-ancestor-of-a-binary-search-tree/)
- [236. Lowest Common Ancestor of a Binary Tree](https://leetcode.com/problems/lowest-common-ancestor-of-a-binary-tree/)
- [1123. Lowest Common Ancestor of Deepest Leaves](https://leetcode.com/problems/lowest-common-ancestor-of-deepest-leaves/) 1607
- [2096. Step by Step Directions from a Binary Tree Node to Another](https://leetcode.com/problems/step-by-step-directions-from-a-binary-tree-node-to-another/) 1805
- [1740. Find Distance in a Binary Tree](https://leetcode.com/problems/find-distance-in-a-binary-tree/) 🔒
- [1644. Lowest Common Ancestor of a Binary Tree II](https://leetcode.com/problems/lowest-common-ancestor-of-a-binary-tree-ii/) 🔒
- [1650. Lowest Common Ancestor of a Binary Tree III](https://leetcode.com/problems/lowest-common-ancestor-of-a-binary-tree-iii/) 🔒
- [1676. Lowest Common Ancestor of a Binary Tree IV](https://leetcode.com/problems/lowest-common-ancestor-of-a-binary-tree-iv/) 🔒

### §2.9 Binary Search Tree (BST)

Usually solved with an inorder traversal.

[Video Explanation: Basic Algorithms Lecture 11](https://leetcode.cn/link/?target=https%3A%2F%2Fwww.bilibili.com%2Fvideo%2FBV14G411P7C1%2F)

- [700. Search in a Binary Search Tree](https://leetcode.com/problems/search-in-a-binary-search-tree/)
- [530. Minimum Absolute Difference in BST](https://leetcode.com/problems/minimum-absolute-difference-in-bst/) 1303
- [783. Minimum Distance Between BST Nodes](https://leetcode.com/problems/minimum-distance-between-bst-nodes/) (same as 530)
- [938. Range Sum of BST](https://leetcode.com/problems/range-sum-of-bst/) 1335
- [501. Find Mode in Binary Search Tree](https://leetcode.com/problems/find-mode-in-binary-search-tree/)
- [230. Kth Smallest Element in a BST](https://leetcode.com/problems/kth-smallest-element-in-a-bst/)
- [98. Validate Binary Search Tree](https://leetcode.com/problems/validate-binary-search-tree/) (has preorder, inorder, and postorder approaches)
- [1305. All Elements in Two Binary Search Trees](https://leetcode.com/problems/all-elements-in-two-binary-search-trees/)
- [99. Recover Binary Search Tree](https://leetcode.com/problems/recover-binary-search-tree/)
- [897. Increasing Order Search Tree](https://leetcode.com/problems/increasing-order-search-tree/) 1473
- [2476. Closest Nodes Queries in a Binary Search Tree](https://leetcode.com/problems/closest-nodes-queries-in-a-binary-search-tree/) 1597
- [653. Two Sum IV - Input is a BST](https://leetcode.com/problems/two-sum-iv-input-is-a-bst/)
- [1373. Maximum Sum BST in Binary Tree](https://leetcode.com/problems/maximum-sum-bst-in-binary-tree/) 1914
- [1932. Merge BSTs to Create Single BST](https://leetcode.com/problems/merge-bsts-to-create-single-bst/) 2484
- [285. Inorder Successor in BST](https://leetcode.com/problems/inorder-successor-in-bst/) 🔒
- [510. Inorder Successor in BST II](https://leetcode.com/problems/inorder-successor-in-bst-ii/) 🔒
- [270. Closest Binary Search Tree Value](https://leetcode.com/problems/closest-binary-search-tree-value/) 🔒
- [272. Closest Binary Search Tree Value II](https://leetcode.com/problems/closest-binary-search-tree-value-ii/) 🔒
- [255. Verify Preorder Sequence in Binary Search Tree](https://leetcode.com/problems/verify-preorder-sequence-in-binary-search-tree/) 🔒
- [1902. Depth of BST Given Insertion Order](https://leetcode.com/problems/depth-of-bst-given-insertion-order/) 🔒

### §2.10 Constructing a Binary Tree

- [108. Convert Sorted Array to Binary Search Tree](https://leetcode.com/problems/convert-sorted-array-to-binary-search-tree/)
- [654. Maximum Binary Tree](https://leetcode.com/problems/maximum-binary-tree/)
- [998. Maximum Binary Tree II](https://leetcode.com/problems/maximum-binary-tree-ii/) 1498
- [1008. Construct Binary Search Tree from Preorder Traversal](https://leetcode.com/problems/construct-binary-search-tree-from-preorder-traversal/) 1563
- [1382. Balance a Binary Search Tree](https://leetcode.com/problems/balance-a-binary-search-tree/)
- [2196. Create Binary Tree from Descriptions](https://leetcode.com/problems/create-binary-tree-from-descriptions/) 1644
- [105. Construct Binary Tree from Preorder and Inorder Traversal](https://leetcode.com/problems/construct-binary-tree-from-preorder-and-inorder-traversal/)
- [106. Construct Binary Tree from Inorder and Postorder Traversal](https://leetcode.com/problems/construct-binary-tree-from-inorder-and-postorder-traversal/)
- [889. Construct Binary Tree from Preorder and Postorder Traversal](https://leetcode.com/problems/construct-binary-tree-from-preorder-and-postorder-traversal/) 1732
- [1028. Recover a Tree from Preorder Traversal](https://leetcode.com/problems/recover-a-tree-from-preorder-traversal/) 1797
- [536. Construct Binary Tree from String](https://leetcode.com/problems/construct-binary-tree-from-string/) 🔒
- [1628. Design An Expression Tree With Evaluate Function](https://leetcode.com/problems/design-an-expression-tree-with-evaluate-function/) 🔒
- [1597. Build Binary Expression Tree From Infix Expression](https://leetcode.com/problems/build-binary-expression-tree-from-infix-expression/) 🔒

### §2.11 Inserting/Deleting Nodes

- [701. Insert Into a Binary Search Tree](https://leetcode.com/problems/insert-into-a-binary-search-tree/)
- [450. Delete Node in a BST](https://leetcode.com/problems/delete-node-in-a-bst/)
- [669. Trim a Binary Search Tree](https://leetcode.com/problems/trim-a-binary-search-tree/)
- [776. Split BST](https://leetcode.com/problems/split-bst/) 🔒
- [1666. Change the Root of a Binary Tree](https://leetcode.com/problems/change-the-root-of-a-binary-tree/) 🔒

### §2.12 Tree DP

- [337. House Robber III](https://leetcode.com/problems/house-robber-iii/)
- [968. Binary Tree Cameras](https://leetcode.com/problems/binary-tree-cameras/)
- [LCP 10. Binary Tree Task Scheduling](https://leetcode.cn/problems/er-cha-shu-ren-wu-diao-du/)
- [LCP 34. Binary Tree Coloring](https://leetcode.cn/problems/er-cha-shu-ran-se-UGC/)
- [LCP 64. Binary Tree Lights](https://leetcode.cn/problems/U7WvvU/)
- [2313. Minimum Flips in Binary Tree to Get Result](https://leetcode.com/problems/minimum-flips-in-binary-tree-to-get-result/) 🔒

For more tree DP problems, see "Tree DP" in the [Dynamic Programming list](07_dynamic_programming.md).

### §2.13 Binary Tree BFS

[Video Explanation: Basic Algorithms Lecture 13](https://leetcode.cn/link/?target=https%3A%2F%2Fwww.bilibili.com%2Fvideo%2FBV1hG4y1277i%2F)

- [102. Binary Tree Level Order Traversal](https://leetcode.com/problems/binary-tree-level-order-traversal/)
- [103. Binary Tree Zigzag Level Order Traversal](https://leetcode.com/problems/binary-tree-zigzag-level-order-traversal/)
- [107. Binary Tree Level Order Traversal II](https://leetcode.com/problems/binary-tree-level-order-traversal-ii/)
- [199. Binary Tree Right Side View](https://leetcode.com/problems/binary-tree-right-side-view/) (can also use DFS)
- [513. Find Bottom Left Tree Value](https://leetcode.com/problems/find-bottom-left-tree-value/)
- [515. Find Largest Value in Each Tree Row](https://leetcode.com/problems/find-largest-value-in-each-tree-row/)
- [637. Average of Levels in Binary Tree](https://leetcode.com/problems/average-of-levels-in-binary-tree/)
- [1161. Maximum Level Sum of a Binary Tree](https://leetcode.com/problems/maximum-level-sum-of-a-binary-tree/) 1250
- [993. Cousins in Binary Tree](https://leetcode.com/problems/cousins-in-binary-tree/) 1288
- [2583. Kth Largest Sum in a Binary Tree](https://leetcode.com/problems/kth-largest-sum-in-a-binary-tree/) 1374
- [1302. Deepest Leaves Sum](https://leetcode.com/problems/deepest-leaves-sum/) 1388
- [2415. Reverse Odd Levels of Binary Tree](https://leetcode.com/problems/reverse-odd-levels-of-binary-tree/) 1431
- [1609. Even Odd Tree](https://leetcode.com/problems/even-odd-tree/) 1438
- [623. Add One Row to Tree](https://leetcode.com/problems/add-one-row-to-tree/)
- [2471. Minimum Number Of Operations To Sort A Binary Tree By Level](https://leetcode.com/problems/minimum-number-of-operations-to-sort-a-binary-tree-by-level/) 1635
- [2641. Cousins in Binary Tree II](https://leetcode.com/problems/cousins-in-binary-tree-ii/) 1677
- [919. Complete Binary Tree Inserter](https://leetcode.com/problems/complete-binary-tree-inserter/) 1691
- [958. Check Completeness of a Binary Tree](https://leetcode.com/problems/check-completeness-of-a-binary-tree/) 1703
- [863. All Nodes Distance K in Binary Tree](https://leetcode.com/problems/all-nodes-distance-k-in-binary-tree/)
- [662. Maximum Width of Binary Tree](https://leetcode.com/problems/maximum-width-of-binary-tree/)
- [3157. Find the Level of Tree With Minimum Sum](https://leetcode.com/problems/find-the-level-of-tree-with-minimum-sum/) 🔒
- [3831. Median of a Binary Search Tree Level](https://leetcode.com/problems/median-of-a-binary-search-tree-level/) 🔒
- [1602. Find Nearest Right Node in Binary Tree](https://leetcode.com/problems/find-nearest-right-node-in-binary-tree/) 🔒
- [742. Closest Leaf in a Binary Tree](https://leetcode.com/problems/closest-leaf-in-a-binary-tree/) 🔒
- [1660. Correct a Binary Tree](https://leetcode.com/problems/correct-a-binary-tree/) 🔒

### §2.14 Linked List + Binary Tree

- [114. Flatten Binary Tree to Linked List](https://leetcode.com/problems/flatten-binary-tree-to-linked-list/)
- [1367. Linked List in Binary Tree](https://leetcode.com/problems/linked-list-in-binary-tree/) 1650
- [109. Convert Sorted List to Binary Search Tree](https://leetcode.com/problems/convert-sorted-list-to-binary-search-tree/)
- [116. Populating Next Right Pointers in Each Node](https://leetcode.com/problems/populating-next-right-pointers-in-each-node/) (achieve O(1) space)
- [117. Populating Next Right Pointers in Each Node II](https://leetcode.com/problems/populating-next-right-pointers-in-each-node-ii/) (achieve O(1) space)
- [426. Convert Binary Search Tree to Sorted Doubly Linked List](https://leetcode.com/problems/convert-binary-search-tree-to-sorted-doubly-linked-list/) 🔒

### §2.15 N-ary Tree

- [589. N-ary Tree Preorder Traversal](https://leetcode.com/problems/n-ary-tree-preorder-traversal/)
- [590. N-ary Tree Postorder Traversal](https://leetcode.com/problems/n-ary-tree-postorder-traversal/)
- [559. Maximum Depth of N-ary Tree](https://leetcode.com/problems/maximum-depth-of-n-ary-tree/)
- [429. N-ary Tree Level Order Traversal](https://leetcode.com/problems/n-ary-tree-level-order-traversal/)
- [427. Construct Quad Tree](https://leetcode.com/problems/construct-quad-tree/)
- [558. Logical OR of Two Binary Grids Represented as Quad Trees](https://leetcode.com/problems/logical-or-of-two-binary-grids-represented-as-quad-trees/)
- [428. Serialize and Deserialize N-ary Tree](https://leetcode.com/problems/serialize-and-deserialize-n-ary-tree/) 🔒
- [1490. Clone N-ary Tree](https://leetcode.com/problems/clone-n-ary-tree/) 🔒
- [1506. Find Root of N-ary Tree](https://leetcode.com/problems/find-root-of-n-ary-tree/) 🔒
- [1522. Diameter of N-Ary Tree](https://leetcode.com/problems/diameter-of-n-ary-tree/) 🔒
- [1516. Move Sub Tree of N-ary Tree](https://leetcode.com/problems/move-sub-tree-of-n-ary-tree/) 🔒

### §2.16 Others

- [1261. Find Elements in a Contaminated Binary Tree](https://leetcode.com/problems/find-elements-in-a-contaminated-binary-tree/) 1440
- [1104. Path in Zigzag Labelled Binary Tree](https://leetcode.com/problems/path-in-zigzag-labelled-binary-tree/) 1545
- [987. Vertical Order Traversal of a Binary Tree](https://leetcode.com/problems/vertical-order-traversal-of-a-binary-tree/) 1676
- [655. Print Binary Tree](https://leetcode.com/problems/print-binary-tree/)
- [979. Distribute Coins in Binary Tree](https://leetcode.com/problems/distribute-coins-in-binary-tree/) 1709 (contribution technique)
- [222. Count Complete Tree Nodes](https://leetcode.com/problems/count-complete-tree-nodes/) (achieve better than O(n) time)
- [297. Serialize and Deserialize Binary Tree](https://leetcode.com/problems/serialize-and-deserialize-binary-tree/)
- [449. Serialize and Deserialize BST](https://leetcode.com/problems/serialize-and-deserialize-bst/)
- [331. Verify Preorder Serialization of a Binary Tree](https://leetcode.com/problems/verify-preorder-serialization-of-a-binary-tree/)
- [652. Find Duplicate Subtrees](https://leetcode.com/problems/find-duplicate-subtrees/)
- [173. Binary Search Tree Iterator](https://leetcode.com/problems/binary-search-tree-iterator/)
- [2049. Count Nodes With the Highest Score](https://leetcode.com/problems/count-nodes-with-the-highest-score/) 1912
- [2673. Make Costs of Paths Equal in a Binary Tree](https://leetcode.com/problems/make-costs-of-paths-equal-in-a-binary-tree/) 1917
- [2509. Cycle Length Queries in a Tree](https://leetcode.com/problems/cycle-length-queries-in-a-tree/) 1948
- [2458. Height of Binary Tree After Subtree Removal Queries](https://leetcode.com/problems/height-of-binary-tree-after-subtree-removal-queries/) 2299 (recommended)
- [LCP 26. Navigation Device](https://leetcode.cn/problems/hSRGyL/)
- [LCP 60. LeetCode Bubble Shooter](https://leetcode.cn/problems/WInSav/)
- [314. Binary Tree Vertical Order Traversal](https://leetcode.com/problems/binary-tree-vertical-order-traversal/) 🔒
- [666. Path Sum IV](https://leetcode.com/problems/path-sum-iv/) 🔒
- [1586. Binary Search Tree Iterator II](https://leetcode.com/problems/binary-search-tree-iterator-ii/) 🔒
- [2773. Height of Special Binary Tree](https://leetcode.com/problems/height-of-special-binary-tree/) 🔒
- [1485. Clone Binary Tree With Random Pointer](https://leetcode.com/problems/clone-binary-tree-with-random-pointer/) 🔒
- [2445. Number of Nodes With Value One](https://leetcode.com/problems/number-of-nodes-with-value-one/) 🔒
- [431. Encode N-ary Tree to Binary Tree](https://leetcode.com/problems/encode-n-ary-tree-to-binary-tree/) 🔒
- [2005. Subtree Removal Game with Fibonacci Tree](https://leetcode.com/problems/subtree-removal-game-with-fibonacci-tree/) 🔒

## III. General Tree

### §3.1 Traversal

- [2368. Reachable Nodes With Restrictions](https://leetcode.com/problems/reachable-nodes-with-restrictions/) 1477
- [1466. Reorder Routes to Make All Paths Lead to the City Zero](https://leetcode.com/problems/reorder-routes-to-make-all-paths-lead-to-the-city-zero/) 1634
- [582. Kill Process](https://leetcode.com/problems/kill-process/) 🔒

### §3.2 Top-Down DFS

- [1376. Time Needed to Inform All Employees](https://leetcode.com/problems/time-needed-to-inform-all-employees/) 1561
- [3528. Unit Conversion I](https://leetcode.com/problems/unit-conversion-i/) 1580
- [1443. Minimum Time to Collect All Apples in a Tree](https://leetcode.com/problems/minimum-time-to-collect-all-apples-in-a-tree/) 1683
- [3820. Pythagorean Distance Nodes in a Tree](https://leetcode.com/problems/pythagorean-distance-nodes-in-a-tree/) 1725
- [1377. Frog Position After T Seconds](https://leetcode.com/problems/frog-position-after-t-seconds/) 1824
- [3067. Count Pairs of Connectable Servers in a Weighted Tree Network](https://leetcode.com/problems/count-pairs-of-connectable-servers-in-a-weighted-tree-network/) 1909
- [3372. Maximize the Number of Target Nodes After Connecting Trees I](https://leetcode.com/problems/maximize-the-number-of-target-nodes-after-connecting-trees-i/) 1927
- [2467. Most Profitable Path in a Tree](https://leetcode.com/problems/most-profitable-path-in-a-tree/) 2053
- [3373. Maximize the Number of Target Nodes After Connecting Trees II](https://leetcode.com/problems/maximize-the-number-of-target-nodes-after-connecting-trees-ii/) 2162
- [1766. Tree of Coprimes](https://leetcode.com/problems/tree-of-coprimes/) 2232
- [2791. Count Paths That Can Form A Palindrome In A Tree](https://leetcode.com/problems/count-paths-that-can-form-a-palindrome-in-a-tree/) 2677
- [3535. Unit Conversion II](https://leetcode.com/problems/unit-conversion-ii/) 🔒

### §3.3 Bottom-Up DFS

- [690. Employee Importance](https://leetcode.com/problems/employee-importance/)
- [3249. Count the Number of Good Nodes](https://leetcode.com/problems/count-the-number-of-good-nodes/) 1566
- [1519. Number of Nodes in the Sub-Tree With the Same Label](https://leetcode.com/problems/number-of-nodes-in-the-sub-tree-with-the-same-label/) 1809
- [3558. Number of Ways to Assign Edge Weights I](https://leetcode.com/problems/number-of-ways-to-assign-edge-weights-i/) 1845
- [3593. Minimum Increments to Equalize Leaf Paths](https://leetcode.com/problems/minimum-increments-to-equalize-leaf-paths/) 1959
- [2872. Maximum Number of K Divisible Components](https://leetcode.com/problems/maximum-number-of-k-divisible-components/) 1968
- [2477. Minimum Fuel Cost to Report to the Capital](https://leetcode.com/problems/minimum-fuel-cost-to-report-to-the-capital/) 2012
- [3812. Minimum Edge Toggles on a Tree](https://leetcode.com/problems/minimum-edge-toggles-on-a-tree/) 2179
- [2973. Find Number of Coins to Place in Tree Nodes](https://leetcode.com/problems/find-number-of-coins-to-place-in-tree-nodes/) 2277
- [2440. Create Components With Same Value](https://leetcode.com/problems/create-components-with-same-value/) 2460
- [1273. Delete Tree Nodes](https://leetcode.com/problems/delete-tree-nodes/) 🔒
- [3004. Maximum Subtree of the Same Color](https://leetcode.com/problems/maximum-subtree-of-the-same-color/) 🔒

### §3.4 Combined Top-Down and Bottom-Up DFS

- [3593. Minimum Increments to Equalize Leaf Paths](https://leetcode.com/problems/minimum-increments-to-equalize-leaf-paths/) 1959 (can also be done bottom-up)
- [3331. Find Subtree Sizes After Changes](https://leetcode.com/problems/find-subtree-sizes-after-changes/) 2046

### §3.5 Diameter of a Tree

[Video Explanation: Basic Algorithms Lecture 23](https://leetcode.cn/link/?target=https%3A%2F%2Fwww.bilibili.com%2Fvideo%2FBV17o4y187h1%2F)

- [2246. Longest Path With Different Adjacent Characters](https://leetcode.com/problems/longest-path-with-different-adjacent-characters/) 2126
- [3203. Find Minimum Diameter After Merging Two Trees](https://leetcode.com/problems/find-minimum-diameter-after-merging-two-trees/) 2266
- [1617. Count Subtrees With Max Distance Between Cities](https://leetcode.com/problems/count-subtrees-with-max-distance-between-cities/) 2309
- [2538. Difference Between Maximum and Minimum Price Sum](https://leetcode.com/problems/difference-between-maximum-and-minimum-price-sum/) 2398
- [1245. Tree Diameter](https://leetcode.com/problems/tree-diameter/) 🔒
- [3787. Find Diameter Endpoints of a Tree](https://leetcode.com/problems/find-diameter-endpoints-of-a-tree/) 🔒
- [3313. Find the Last Marked Nodes in Tree](https://leetcode.com/problems/find-the-last-marked-nodes-in-tree/) 🔒

### §3.6 Topological Sort on a Tree

- [310. Minimum Height Trees](https://leetcode.com/problems/minimum-height-trees/)
- [3812. Minimum Edge Toggles on a Tree](https://leetcode.com/problems/minimum-edge-toggles-on-a-tree/) 2179
- [2603. Collect Coins in a Tree](https://leetcode.com/problems/collect-coins-in-a-tree/) 2712

### §3.7 DFS Timestamps (Euler Tour)

Tree problems can often be converted into array problems — for example, an operation on a subtree becomes an operation on a subarray. This is usually combined with other data structures.

- [3515. Shortest Path In A Weighted Tree](https://leetcode.com/problems/shortest-path-in-a-weighted-tree/) 2312
- [LCP 05. Distribute LeetCoin](https://leetcode.cn/problems/coin-bonus/) (same as 3515)
- [2322. Minimum Score After Removals on a Tree](https://leetcode.com/problems/minimum-score-after-removals-on-a-tree/) 2392
- [3327. Check If DFS Strings Are Palindromes](https://leetcode.com/problems/check-if-dfs-strings-are-palindromes/) 2454
- [3590. Kth Smallest Path XOR Sum](https://leetcode.com/problems/kth-smallest-path-xor-sum/) 2646 (more than one approach exists)

### §3.8 Lowest Common Ancestor (LCA) & Binary Lifting

[Explanation](https://leetcode.com/problems/kth-ancestor-of-a-tree-node/solution/mo-ban-jiang-jie-shu-shang-bei-zeng-suan-v3rw/)

Weighted-tree LCA template (nodes numbered from 0); see the explanation link above for full code in Python3/Java/C++/Go.

- [1483. Kth Ancestor of a Tree Node](https://leetcode.com/problems/kth-ancestor-of-a-tree-node/) 2115 (template problem)
- [3559. Number of Ways to Assign Edge Weights II](https://leetcode.com/problems/number-of-ways-to-assign-edge-weights-ii/) 2146
- [3553. Minimum Weighted Subgraph With the Required Paths II](https://leetcode.com/problems/minimum-weighted-subgraph-with-the-required-paths-ii/) 2411 (conclusion-based)
- [3585. Find Weighted Median Node in Tree](https://leetcode.com/problems/find-weighted-median-node-in-tree/) 2429
- [2846. Minimum Edge Weight Equilibrium Queries In A Tree](https://leetcode.com/problems/minimum-edge-weight-equilibrium-queries-in-a-tree/) 2508
- [2646. Minimize the Total Price of the Trips](https://leetcode.com/problems/minimize-the-total-price-of-the-trips/) (**difference array on a tree**)
- [2277. Closest Node to Path in Tree](https://leetcode.com/problems/closest-node-to-path-in-tree/) 🔒

**Binary Lifting on Arrays**:

- [3534. Path Existence Queries in a Graph II](https://leetcode.com/problems/path-existence-queries-in-a-graph-ii/) 2507
- [2836. Maximize Value of Function in a Ball Passing Game](https://leetcode.com/problems/maximize-value-of-function-in-a-ball-passing-game/) 2769 (more than one approach exists)
- [3464. Maximize the Distance Between Points on a Square](https://leetcode.com/problems/maximize-the-distance-between-points-on-a-square/)

### §3.9 Virtual Tree

- [3786. Total Sum of Interaction Cost in Tree Groups](https://leetcode.com/problems/total-sum-of-interaction-cost-in-tree-groups/) (an approach that doesn't rely on the ≤20 constraint)

### §3.10 Small-to-Large Merging on Trees (DSU on Tree)

- [2003. Smallest Missing Genetic Value in Each Subtree](https://leetcode.com/problems/smallest-missing-genetic-value-in-each-subtree/) 2415
- [3590. Kth Smallest Path XOR Sum](https://leetcode.com/problems/kth-smallest-path-xor-sum/) 2646 (C++ needs pb_ds (policy-based data structure))
- [3575. Maximum Good Subtree Score](https://leetcode.com/problems/maximum-good-subtree-score/) (achieve O(n log n · 2^D) time)

### §3.11 Centroid Decomposition

- [3372. Maximize the Number of Target Nodes After Connecting Trees I](https://leetcode.com/problems/maximize-the-number-of-target-nodes-after-connecting-trees-i/)

### §3.12 Sliding Window on a Tree

- [3425. Longest Special Path](https://leetcode.com/problems/longest-special-path/) 2435
- [3486. Longest Special Path II](https://leetcode.com/problems/longest-special-path-ii/) 2925

### §3.13 Others

- [2867. Count Valid Paths in a Tree](https://leetcode.com/problems/count-valid-paths-in-a-tree/) 2428
- [2421. Number Of Good Paths](https://leetcode.com/problems/number-of-good-paths/) 2445
- [1719. Number of Ways to Reconstruct a Tree](https://leetcode.com/problems/number-of-ways-to-reconstruct-a-tree/) 3018
- [2479. Maximum XOR Of Two Non Overlapping Subtrees](https://leetcode.com/problems/maximum-xor-of-two-non-overlapping-subtrees/) 🔒

See also "**Tree DP**" in the [Dynamic Programming list](07_dynamic_programming.md), which includes rerooting DP.

## IV. Backtracking

Backtracking is essentially DFS on a search tree.

Recommended: finish **§2.7** first — understand backtracking on binary trees before moving on to backtracking in general.

### §4.1 Introduction to Backtracking

[Video Explanation: Basic Algorithms Lecture 14](https://leetcode.cn/link/?target=https%3A%2F%2Fwww.bilibili.com%2Fvideo%2FBV1mG4y1A7Gu%2F)

- [17. Letter Combinations of a Phone Number](https://leetcode.com/problems/letter-combinations-of-a-phone-number/)

### §4.2 Subset-Type Backtracking

[Video Explanation: Basic Algorithms Lecture 14](https://leetcode.cn/link/?target=https%3A%2F%2Fwww.bilibili.com%2Fvideo%2FBV1mG4y1A7Gu%2F)

There are two ways to write it: **"pick or skip"** and **"enumerate which one to pick"**.

Can also be solved with **binary/bitmask enumeration**.

- [78. Subsets](https://leetcode.com/problems/subsets/)
- [1863. Sum of All Subset XOR Totals](https://leetcode.com/problems/sum-of-all-subset-xor-totals/) 1372
- [784. Letter Case Permutation](https://leetcode.com/problems/letter-case-permutation/)
- [3566. Partition Array Into Two Equal Product Subsets](https://leetcode.com/problems/partition-array-into-two-equal-product-subsets/) 1459
- [2044. Count Number of Maximum Bitwise-OR Subsets](https://leetcode.com/problems/count-number-of-maximum-bitwise-or-subsets/) 1568
- [LCP 51. Cooking Dishes](https://leetcode.cn/problems/UEcfPD/)
- [2397. Maximum Rows Covered by Columns](https://leetcode.com/problems/maximum-rows-covered-by-columns/) 1719
- [1239. Maximum Length of a Concatenated String With Unique Characters](https://leetcode.com/problems/maximum-length-of-a-concatenated-string-with-unique-characters/) 1720
- [2212. Maximum Points in an Archery Competition](https://leetcode.com/problems/maximum-points-in-an-archery-competition/) 1869
- [1255. Maximum Score Words Formed by Letters](https://leetcode.com/problems/maximum-score-words-formed-by-letters/) 1882
- [2151. Maximum Good People Based on Statements](https://leetcode.com/problems/maximum-good-people-based-on-statements/) 1980
- [2597. The Number of Beautiful Subsets](https://leetcode.com/problems/the-number-of-beautiful-subsets/) 2023
- [2959. Number of Possible Sets of Closing Branches](https://leetcode.com/problems/number-of-possible-sets-of-closing-branches/) 2077
- [1601. Maximum Number of Achievable Transfer Requests](https://leetcode.com/problems/maximum-number-of-achievable-transfer-requests/) 2119
- [1617. Count Subtrees With Max Distance Between Cities](https://leetcode.com/problems/count-subtrees-with-max-distance-between-cities/) 2309
- [2174. Remove All Ones With Row and Column Flips II](https://leetcode.com/problems/remove-all-ones-with-row-and-column-flips-ii/) 🔒
- [320. Generalized Abbreviation](https://leetcode.com/problems/generalized-abbreviation/) 🔒
- [254. Factor Combinations](https://leetcode.com/problems/factor-combinations/) 🔒

**Mind Extensions**:

- [39. Combination Sum](https://leetcode.com/problems/combination-sum/) (the same number can be chosen repeatedly)
- [2002. Maximum Product of the Length of Two Palindromic Subsequences](https://leetcode.com/problems/maximum-product-of-the-length-of-two-palindromic-subsequences/) 1869

### §4.3 Partition-Type Backtracking

[Video Explanation: Basic Algorithms Lecture 14](https://leetcode.cn/link/?target=https%3A%2F%2Fwww.bilibili.com%2Fvideo%2FBV1mG4y1A7Gu%2F)

Think of the separators (commas) as things you can "pick or skip" — this is essentially subset-type backtracking.

- [131. Palindrome Partitioning](https://leetcode.com/problems/palindrome-partitioning/)
- [2698. Find the Punishment Number of an Integer](https://leetcode.com/problems/find-the-punishment-number-of-an-integer/) 1679
- [1593. Split a String Into the Max Number of Unique Substrings](https://leetcode.com/problems/split-a-string-into-the-max-number-of-unique-substrings/) 1740
- [1849. Splitting a String Into Descending Consecutive Values](https://leetcode.com/problems/splitting-a-string-into-descending-consecutive-values/) 1747
- [93. Restore IP Addresses](https://leetcode.com/problems/restore-ip-addresses/)
- [140. Word Break II](https://leetcode.com/problems/word-break-ii/)
- [291. Word Pattern II](https://leetcode.com/problems/word-pattern-ii/) 🔒

### §4.4 Combination-Type Backtracking

[Video Explanation: Basic Algorithms Lecture 15](https://leetcode.cn/link/?target=https%3A%2F%2Fwww.bilibili.com%2Fvideo%2FBV1xG4y1F7nC%2F)

There's a constraint on the count of chosen elements — also counts as subset-type backtracking.

- [77. Combinations](https://leetcode.com/problems/combinations/)
- [216. Combination Sum III](https://leetcode.com/problems/combination-sum-iii/)
- [1286. Iterator for Combination](https://leetcode.com/problems/iterator-for-combination/) 1591
- [22. Generate Parentheses](https://leetcode.com/problems/generate-parentheses/) (essentially: choose n out of 2n positions for left parentheses, and place right parentheses in the rest)
- [301. Remove Invalid Parentheses](https://leetcode.com/problems/remove-invalid-parentheses/)

### §4.5 Permutation-Type Backtracking

[Video Explanation: Basic Algorithms Lecture 16](https://leetcode.cn/link/?target=https%3A%2F%2Fwww.bilibili.com%2Fvideo%2FBV1mY411D7f6%2F)

Some of these problems can also be solved with bitmask DP.

- [46. Permutations](https://leetcode.com/problems/permutations/)
- [3799. Word Squares II](https://leetcode.com/problems/word-squares-ii/) 1606
- [3376. Minimum Time to Break Locks I](https://leetcode.com/problems/minimum-time-to-break-locks-i/) 1793
- [51. N-Queens](https://leetcode.com/problems/n-queens/) (essentially enumerating permutations of column indices)
- [52. N-Queens II](https://leetcode.com/problems/n-queens-ii/)
- [2850. Minimum Moves to Spread Stones Over Grid](https://leetcode.com/problems/minimum-moves-to-spread-stones-over-grid/) 2001
- [1718. Construct the Lexicographically Largest Valid Sequence](https://leetcode.com/problems/construct-the-lexicographically-largest-valid-sequence/) 2080
- [1307. Verbal Arithmetic Puzzle](https://leetcode.com/problems/verbal-arithmetic-puzzle/) 2250
- [37. Sudoku Solver](https://leetcode.com/problems/sudoku-solver/)
- [3437. Permutations III](https://leetcode.com/problems/permutations-iii/) 🔒
- [267. Palindrome Permutation II](https://leetcode.com/problems/palindrome-permutation-ii/) 🔒

### §4.6 Backtracking With Duplicate Elements

- [90. Subsets II](https://leetcode.com/problems/subsets-ii/)
- [40. Combination Sum II](https://leetcode.com/problems/combination-sum-ii/)
- [491. Non-decreasing Subsequences](https://leetcode.com/problems/non-decreasing-subsequences/)
- [47. Permutations II](https://leetcode.com/problems/permutations-ii/)
- [1079. Letter Tile Possibilities](https://leetcode.com/problems/letter-tile-possibilities/) 1741
- [3646. Next Special Palindrome Number](https://leetcode.com/problems/next-special-palindrome-number/) 2445
- [2014. Longest Subsequence Repeated K Times](https://leetcode.com/problems/longest-subsequence-repeated-k-times/) 2558

### §4.7 Search

- [3211. Generate Binary Strings Without Adjacent Zeros](https://leetcode.com/problems/generate-binary-strings-without-adjacent-zeros/) 1353
- [967. Numbers With Same Consecutive Differences](https://leetcode.com/problems/numbers-with-same-consecutive-differences/) 1433
- [2094. Finding 3-Digit Even Numbers](https://leetcode.com/problems/finding-3-digit-even-numbers/)
- [1415. The k-th Lexicographical String of All Happy Strings of Length n](https://leetcode.com/problems/the-k-th-lexicographical-string-of-all-happy-strings-of-length-n/) 1576 (an O(n) approach also exists)
- [1219. Path With Maximum Gold](https://leetcode.com/problems/path-with-maximum-gold/) 1663
- [79. Word Search](https://leetcode.com/problems/word-search/)
- [980. Unique Paths III](https://leetcode.com/problems/unique-paths-iii/) 1830
- [2002. Maximum Product of the Length of Two Palindromic Subsequences](https://leetcode.com/problems/maximum-product-of-the-length-of-two-palindromic-subsequences/) 1869
- [1255. Maximum Score Words Formed by Letters](https://leetcode.com/problems/maximum-score-words-formed-by-letters/) 1882
- [3669. Balanced K-Factor Decomposition](https://leetcode.com/problems/balanced-k-factor-decomposition/) 1917
- [756. Pyramid Transition Matrix](https://leetcode.com/problems/pyramid-transition-matrix/) 1990
- [473. Matchsticks to Square](https://leetcode.com/problems/matchsticks-to-square/) (subset partition problem with k=4)
- [212. Word Search II](https://leetcode.com/problems/word-search-ii/)
- [638. Shopping Offers](https://leetcode.com/problems/shopping-offers/)
- [1240. Tiling a Rectangle With the Fewest Squares](https://leetcode.com/problems/tiling-a-rectangle-with-the-fewest-squares/) 2242
- [679. 24 Game](https://leetcode.com/problems/24-game/)
- [282. Expression Add Operators](https://leetcode.com/problems/expression-add-operators/)
- [126. Word Ladder II](https://leetcode.com/problems/word-ladder-ii/)
- [691. Stickers to Spell Word](https://leetcode.com/problems/stickers-to-spell-word/)
- [2056. Number Of Valid Move Combinations On Chessboard](https://leetcode.com/problems/number-of-valid-move-combinations-on-chessboard/) 2611
- [2386. Find the K-Sum of an Array](https://leetcode.com/problems/find-the-k-sum-of-an-array/) 2648
- [3509. Maximum Product of Subsequences With an Alternating Sum Equal to K](https://leetcode.com/problems/maximum-product-of-subsequences-with-an-alternating-sum-equal-to-k/) 2703
- [488. Zuma Game](https://leetcode.com/problems/zuma-game/)
- [LCP 58. Assembling Building Blocks](https://leetcode.cn/problems/De4qBB/)
- [Interview 17.25. Word Rectangle](https://leetcode.com/problems/word-rectangle-lcci/)
- [2664. The Knight's Tour](https://leetcode.com/problems/the-knights-tour/) 🔒
- [3565. Sequential Grid Path Cover](https://leetcode.com/problems/sequential-grid-path-cover/) 🔒
- [247. Strobogrammatic Number II](https://leetcode.com/problems/strobogrammatic-number-ii/) 🔒
- [248. Strobogrammatic Number III](https://leetcode.com/problems/strobogrammatic-number-iii/) 🔒
- [411. Minimum Unique Word Abbreviation](https://leetcode.com/problems/minimum-unique-word-abbreviation/) 🔒
- [1088. Confusing Number II](https://leetcode.com/problems/confusing-number-ii/) 🔒

### §4.8 Meet in the Middle

Also known as "meet in the middle".

[Explanation](https://leetcode.com/problems/target-sum/solutions/2119041/jiao-ni-yi-bu-bu-si-kao-dong-tai-gui-hua-s1cx/) (see the end of the article)

- [805. Split Array With Same Average](https://leetcode.com/problems/split-array-with-same-average/) 1983
- [494. Target Sum](https://leetcode.com/problems/target-sum/)
- [3566. Partition Array Into Two Equal Product Subsets](https://leetcode.com/problems/partition-array-into-two-equal-product-subsets/)
- [1755. Closest Subsequence Sum](https://leetcode.com/problems/closest-subsequence-sum/) 2364
- [956. Tallest Billboard](https://leetcode.com/problems/tallest-billboard/) 2381
- [2035. Partition Array Into Two Arrays to Minimize Sum Difference](https://leetcode.com/problems/partition-array-into-two-arrays-to-minimize-sum-difference/) 2490
- [3801. Minimum Cost to Merge Sorted Lists](https://leetcode.com/problems/minimum-cost-to-merge-sorted-lists/) (optimization)
- [3267. Count Almost Equal Pairs II](https://leetcode.com/problems/count-almost-equal-pairs-ii/) (optimization)
- [LCP 82. Tree of All Spirits](https://leetcode.com/problems/cnHoX6/)

## V. Other Recursion / Divide and Conquer

- [3537. Fill a Special Grid](https://leetcode.com/problems/fill-a-special-grid/) 1542
- [215. Kth Largest Element in an Array](https://leetcode.com/problems/kth-largest-element-in-an-array/) (do this before problem 912)
- [912. Sort an Array](https://leetcode.com/problems/sort-an-array/) (implement quicksort by hand)
- [880. Decoded String at Index](https://leetcode.com/problems/decoded-string-at-index/) 2011
- [3307. Find the K-th Character in String Game II](https://leetcode.com/problems/find-the-k-th-character-in-string-game-ii/) 2232
- [1545. Find Kth Bit in Nth Binary String](https://leetcode.com/problems/find-kth-bit-in-nth-binary-string/) (achieve O(n) time)
- [3614. Process String With Special Operations II](https://leetcode.com/problems/process-string-with-special-operations-ii/)
- [932. Beautiful Array](https://leetcode.com/problems/beautiful-array/) ~2500

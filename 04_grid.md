# Grid (Graph)

Problem list from [0x3F's LeetCode Study Plan](https://leetcode.cn/circle/discuss/YiXPXW/) — Grid (DFS / BFS / Comprehensive Applications).

## I. Grid DFS

Suitable for problems that count the number or size of connected components. Some problems have more than one approach and can also be solved with BFS or Union-Find.

- [200. Number of Islands](https://leetcode.com/problems/number-of-islands/)
- [695. Max Area of Island](https://leetcode.com/problems/max-area-of-island/)
- [3619. Count Islands With Total Value Divisible by K](https://leetcode.com/problems/count-islands-with-total-value-divisible-by-k/) 1461
- [2658. Maximum Number of Fish in a Grid](https://leetcode.com/problems/maximum-number-of-fish-in-a-grid/) 1490
- [Interview 16.19. Pond Sizes](https://leetcode.com/problems/pond-sizes-lcci/)
- [LCS 03. Subject Space](https://leetcode.com/problems/YesdPw/)
- [463. Island Perimeter](https://leetcode.com/problems/island-perimeter/) (mind extension: [892. Surface Area of 3D Shapes](https://leetcode.com/problems/surface-area-of-3d-shapes/))
- [733. Flood Fill](https://leetcode.com/problems/flood-fill/)
- [1034. Coloring A Border](https://leetcode.com/problems/coloring-a-border/) 1579
- [1020. Number of Enclaves](https://leetcode.com/problems/number-of-enclaves/) 1615
- [2684. Maximum Number of Moves in a Grid](https://leetcode.com/problems/maximum-number-of-moves-in-a-grid/) 1626
- [1254. Number of Closed Islands](https://leetcode.com/problems/number-of-closed-islands/) 1659
- [130. Surrounded Regions](https://leetcode.com/problems/surrounded-regions/)
- [1905. Count Sub Islands](https://leetcode.com/problems/count-sub-islands/) 1679
- [1391. Check if There is a Valid Path in a Grid](https://leetcode.com/problems/check-if-there-is-a-valid-path-in-a-grid/) 1746
- [417. Pacific Atlantic Water Flow](https://leetcode.com/problems/pacific-atlantic-water-flow/)
- [529. Minesweeper](https://leetcode.com/problems/minesweeper/)
- [1559. Detect Cycles in 2D Grid](https://leetcode.com/problems/detect-cycles-in-2d-grid/) 1838
- [827. Making A Large Island](https://leetcode.com/problems/making-a-large-island/) 1934 (variant in my solution)
- [LCP 63. Marble Game](https://leetcode.cn/problems/EXvqDp/) (can also be solved without DFS)
- [305. Number of Islands II](https://leetcode.com/problems/number-of-islands-ii/) 🔒
- [2061. Number of Spaces Cleaning Robot Cleaned](https://leetcode.com/problems/number-of-spaces-cleaning-robot-cleaned/) 🔒 (can also be solved iteratively)
- [2852. Sum of Remoteness of All Cells](https://leetcode.com/problems/sum-of-remoteness-of-all-cells/) 🔒
- [489. Robot Room Cleaner](https://leetcode.com/problems/robot-room-cleaner/) 🔒
- [1970. Last Day Where You Can Still Cross](https://leetcode.com/problems/last-day-where-you-can-still-cross/) 2124 (more than one approach)

## II. Grid BFS

- [1926. Nearest Exit from Entrance in Maze](https://leetcode.com/problems/nearest-exit-from-entrance-in-maze/) 1638
- [1091. Shortest Path in Binary Matrix](https://leetcode.com/problems/shortest-path-in-binary-matrix/) 1658
- [1162. As Far from Land as Possible](https://leetcode.com/problems/as-far-from-land-as-possible/) 1666
- [542. 01 Matrix](https://leetcode.com/problems/01-matrix/)
- [994. Rotting Oranges](https://leetcode.com/problems/rotting-oranges/)
- [1765. Map of Highest Peak](https://leetcode.com/problems/map-of-highest-peak/) 1783
- [934. Shortest Bridge](https://leetcode.com/problems/shortest-bridge/) 1826
- [2146. K Highest Ranked Items Within a Price Range](https://leetcode.com/problems/k-highest-ranked-items-within-a-price-range/) 1837
- [1293. Shortest Path in a Grid with Obstacles Elimination](https://leetcode.com/problems/shortest-path-in-a-grid-with-obstacles-elimination/) 1967
- [909. Snakes and Ladders](https://leetcode.com/problems/snakes-and-ladders/) 2020
- [1210. Minimum Moves to Reach Target with Rotations](https://leetcode.com/problems/minimum-moves-to-reach-target-with-rotations/) 2022
- [675. Cut Off Trees for Golf Event](https://leetcode.com/problems/cut-off-trees-for-golf-event/)
- [2812. Find the Safest Path in a Grid](https://leetcode.com/problems/find-the-safest-path-in-a-grid/) 2154
- [749. Contain Virus](https://leetcode.com/problems/contain-virus/) 2277
- [1730. Shortest Path to Get Food](https://leetcode.com/problems/shortest-path-to-get-food/) 🔒
- [286. Walls and Gates](https://leetcode.com/problems/walls-and-gates/) 🔒
- [490. The Maze](https://leetcode.com/problems/the-maze/) 🔒
- [505. The Maze II](https://leetcode.com/problems/the-maze-ii/) 🔒
- [499. The Maze III](https://leetcode.com/problems/the-maze-iii/) 🔒
- [317. Shortest Distance from All Buildings](https://leetcode.com/problems/shortest-distance-from-all-buildings/) 🔒
- [2814. Minimum Time Takes to Reach Destination Without Drowning](https://leetcode.com/problems/minimum-time-takes-to-reach-destination-without-drowning/) 🔒

## III. Grid 0-1 BFS

Problems where edge weights are only 0 and 1 can also be solved with BFS.

- [3286. Find a Safe Walk Through a Grid](https://leetcode.com/problems/find-a-safe-walk-through-a-grid/) (achieve O(mn))
- [2290. Minimum Obstacle Removal to Reach Corner](https://leetcode.com/problems/minimum-obstacle-removal-to-reach-corner/) 2138
- [1368. Minimum Cost to Make at Least One Valid Path in a Grid](https://leetcode.com/problems/minimum-cost-to-make-at-least-one-valid-path-in-a-grid/) 2069
- [3552. Grid Teleportation Traversal](https://leetcode.com/problems/grid-teleportation-traversal/) 2036
- [1824. Minimum Sideway Jumps](https://leetcode.com/problems/minimum-sideway-jumps/)
- [LCP 56. Token Delivery](https://leetcode.cn/problems/6UEx57/)

## IV. Grid Dijkstra

See **§3.1 Single-Source Shortest Path: Dijkstra** in [06_graph.md](06_graph.md), where the grid problems are marked.

## V. Comprehensive Applications

- [1631. Path With Minimum Effort](https://leetcode.com/problems/path-with-minimum-effort/) 1948
- [778. Swim in Rising Water](https://leetcode.com/problems/swim-in-rising-water/) 2097
- [329. Longest Increasing Path in a Matrix](https://leetcode.com/problems/longest-increasing-path-in-a-matrix/)
- [3568. Minimum Moves to Clean the Classroom](https://leetcode.com/problems/minimum-moves-to-clean-the-classroom/) 2143 (bitmask BFS / layered-graph shortest path)
- [1036. Escape a Large Maze](https://leetcode.com/problems/escape-a-large-maze/) 2165
- [864. Shortest Path to Get All Keys](https://leetcode.com/problems/shortest-path-to-get-all-keys/) 2259 (bitmask BFS / layered-graph shortest path)
- [1263. Minimum Moves to Move a Box to Their Target Location](https://leetcode.com/problems/minimum-moves-to-move-a-box-to-their-target-location/) 2297
- [2258. Escape the Spreading Fire](https://leetcode.com/problems/escape-the-spreading-fire/) 2347
- [2556. Disconnect Path in a Binary Matrix by at Most One Flip](https://leetcode.com/problems/disconnect-path-in-a-binary-matrix-by-at-most-one-flip/) 2369
- [2577. Minimum Time to Visit a Cell in a Grid](https://leetcode.com/problems/minimum-time-to-visit-a-cell-in-a-grid/) 2382
- [2617. Minimum Number of Visited Cells in a Grid](https://leetcode.com/problems/minimum-number-of-visited-cells-in-a-grid/) 2582
- [LCP 13. Treasure Hunt](https://leetcode.cn/problems/xun-bao/) (bitmask DP)
- [LCP 31. Transforming Maze](https://leetcode.cn/problems/Db3wC1/)
- [LCP 45. Bicycle Stunt Arena](https://leetcode.cn/problems/kplEvH/)
- [LCP 75. Teleport Scroll](https://leetcode.cn/problems/rdmXM7/)
- [1778. Shortest Path in a Hidden Grid](https://leetcode.com/problems/shortest-path-in-a-hidden-grid/) 🔒
- [694. Number of Distinct Islands](https://leetcode.com/problems/number-of-distinct-islands/) 🔒
- [711. Number of Distinct Islands II](https://leetcode.com/problems/number-of-distinct-islands-ii/) 🔒
- [1102. Path With Maximum Minimum Value](https://leetcode.com/problems/path-with-maximum-minimum-value/) 🔒

## Thinking Problems

1. For an `m` × `n` grid, how much space does the BFS queue consume at most? How much does the DFS recursion stack consume at most?
2. Construct a grid that makes the DFS recursion depth as large as possible. How would you construct it if the start is `(0, 0)`? How would you construct it if the start is `(i, j)`?

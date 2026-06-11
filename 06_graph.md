# Graph Algorithms

> Problem list from [0x3F's LeetCode Problem Lists](https://leetcode.cn/circle/discuss/01LUak/)

------

### §1.1 Depth-First Search (DFS)

Python3

Java

C++

Go

    def solve(n: int, edges: List[List[int]]) -> List[int]:
        g = [[] for _ in range(n)]
        for x, y in edges:
            g[x].append(y)
            g[y].append(x)  # undirected graph

        vis = [False] * n

        def dfs(x: int) -> int:
            size = 1
            for y in g[x]:
                if not vis[y]:
                    size += dfs(y)
            return size

        ans = []
        for i, b in enumerate(vis):
                size = dfs(i)
                ans.append(size)
        return ans

*   [547. Number of Provinces](https://leetcode.com/problems/number-of-provinces/)
*   [1971. Find If Path Exists in Graph](https://leetcode.com/problems/find-if-path-exists-in-graph/)
*   [797. All Paths from Source to Target](https://leetcode.com/problems/all-paths-from-source-to-target/) 1383
*   [1306. Jump Game Iii](https://leetcode.com/problems/jump-game-iii/) 1397
*   [841. Keys and Rooms](https://leetcode.com/problems/keys-and-rooms/) 1412
*   [2316. Count Unreachable Pairs of Nodes in an Undirected Graph](https://leetcode.com/problems/count-unreachable-pairs-of-nodes-in-an-undirected-graph/) 1604
*   [1319. Number of Operations to Make Network Connected](https://leetcode.com/problems/number-of-operations-to-make-network-connected/) 1633
*   [2492. Minimum Score of a Path Between Two Cities](https://leetcode.com/problems/minimum-score-of-a-path-between-two-cities/) 1680
*   [3310. Remove Methods from Project](https://leetcode.com/problems/remove-methods-from-project/) 1711
*   [2685. Count the Number of Complete Components](https://leetcode.com/problems/count-the-number-of-complete-components/) 1769
*   [2192. All Ancestors of a Node in a Directed Acyclic Graph](https://leetcode.com/problems/all-ancestors-of-a-node-in-a-directed-acyclic-graph/) 1788
*   [3387. Maximize Amount after Two Days of Conversions](https://leetcode.com/problems/maximize-amount-after-two-days-of-conversions/) 1788
*   [924. Minimize Malware Spread](https://leetcode.com/problems/minimize-malware-spread/) 1869
*   [2101. Detonate the Maximum Bombs](https://leetcode.com/problems/detonate-the-maximum-bombs/) 1880
*   [721. Accounts Merge](https://leetcode.com/problems/accounts-merge/)
*   [207. Course Schedule](https://leetcode.com/problems/course-schedule/)
*   [802. Find Eventual Safe States](https://leetcode.com/problems/find-eventual-safe-states/) 1962
*   [3695. Maximize Alternating Sum Using Swaps](https://leetcode.com/problems/maximize-alternating-sum-using-swaps/) 1984
*   [928. Minimize Malware Spread Ii](https://leetcode.com/problems/minimize-malware-spread-ii/) 1985
*   [2092. Find All People with Secret](https://leetcode.com/problems/find-all-people-with-secret/) 2004
*   [3108. Minimum Cost Walk in Weighted Graph](https://leetcode.com/problems/minimum-cost-walk-in-weighted-graph/) 2109
*   [LCP 07. Chuan Di Xin Xi](https://leetcode.com/problems/chuan-di-xin-xi/)
*   [261. Graph Valid Tree](https://leetcode.com/problems/graph-valid-tree/) (Premium)
*   [323. Number of Connected Components in an Undirected Graph](https://leetcode.com/problems/number-of-connected-components-in-an-undirected-graph/) (Premium)

**Advanced Thinking**:

*   [1298. Maximum Candies You Can Get from Boxes](https://leetcode.com/problems/maximum-candies-you-can-get-from-boxes/) 1825

### §1.2 Breadth-First Search (BFS)

Python3

Java

C++

Go

    def bfs(n: int, edges: List[List[int]], start: int) -> List[int]:
        g = [[] for _ in range(n)]
        for x, y in edges:
            g[x].append(y)
            g[y].append(x)  # undirected graph

        dis[start] = 0
        q = deque([start])
        while q:
            x = q.popleft()
            for y in g[x]:
                if dis[y] < 0:
                    dis[y] = dis[x] + 1
                    q.append(y)
        return dis

*   [3243. Shortest Distance after Road Addition Queries I](https://leetcode.com/problems/shortest-distance-after-road-addition-queries-i/) 1568
*   [1311. Get Watched Videos by Your Friends](https://leetcode.com/problems/get-watched-videos-by-your-friends/) 1653
*   [3015. Count the Number of Houses at a Certain Distance I](https://leetcode.com/problems/count-the-number-of-houses-at-a-certain-distance-i/) 1658
*   [1129. Shortest Path with Alternating Colors](https://leetcode.com/problems/shortest-path-with-alternating-colors/) 1780
*   [2039. The Time When the Network Becomes Idle](https://leetcode.com/problems/the-time-when-the-network-becomes-idle/) 1865
*   [2608. Shortest Cycle in a Graph](https://leetcode.com/problems/shortest-cycle-in-a-graph/) 1904
*   [815. Bus Routes](https://leetcode.com/problems/bus-routes/) 1964

### §1.3 Graph Modeling + BFS Shortest Path

*   [433. Minimum Genetic Mutation](https://leetcode.com/problems/minimum-genetic-mutation/)
*   [1284. Minimum Number of Flips to Convert Binary Matrix to Zero Matrix](https://leetcode.com/problems/minimum-number-of-flips-to-convert-binary-matrix-to-zero-matrix/) 1811
*   [773. Sliding Puzzle](https://leetcode.com/problems/sliding-puzzle/) 1815
*   [752. Open the Lock](https://leetcode.com/problems/open-the-lock/) 1878
*   [3690. Split and Merge Array Transformation](https://leetcode.com/problems/split-and-merge-array-transformation/) 1982
*   [301. Remove Invalid Parentheses](https://leetcode.com/problems/remove-invalid-parentheses/)
*   [514. Freedom Trail](https://leetcode.com/problems/freedom-trail/)
*   [847. Shortest Path Visiting All Nodes](https://leetcode.com/problems/shortest-path-visiting-all-nodes/) 2201
*   [854. K Similar Strings](https://leetcode.com/problems/k-similar-strings/) 2377
*   [127. Word Ladder](https://leetcode.com/problems/word-ladder/)
*   [488. Zuma Game](https://leetcode.com/problems/zuma-game/)
*   [1197. Minimum Knight Moves](https://leetcode.com/problems/minimum-knight-moves/) (Premium)
*   [3141. Maximum Hamming Distances](https://leetcode.com/problems/maximum-hamming-distances/) (Premium)

**Topic: Jump Game**

*   [2998. Minimum Number of Operations to Make X and Y Equal](https://leetcode.com/problems/minimum-number-of-operations-to-make-x-and-y-equal/) 1795
*   [1345. Jump Game Iv](https://leetcode.com/problems/jump-game-iv/) 1810
*   [2059. Minimum Operations to Convert Number](https://leetcode.com/problems/minimum-operations-to-convert-number/) 1850
*   [1654. Minimum Jumps to Reach Home](https://leetcode.com/problems/minimum-jumps-to-reach-home/) 2124
*   [3629. Minimum Jumps to Reach End Via Prime Teleportation](https://leetcode.com/problems/minimum-jumps-to-reach-end-via-prime-teleportation/) 2139
*   [LCP 09. Zui Xiao Tiao Yue Ci Shu](https://leetcode.com/problems/zui-xiao-tiao-yue-ci-shu/)

------

### §2.1 Topological Sort

Template:

Python3

Java

C++

Go

    def topologicalSort(n: int, edges: List[List[int]]) -> List[int]:
        g = [[] for _ in range(n)]
        in_deg = [0] * n
        for x, y in edges:
            g[x].append(y)

        topo_order = []
        while q:
            x = q.popleft()
            topo_order.append(x)
            for y in g[x]:

            return []
        return topo_order

*   [210. Course Schedule Ii](https://leetcode.com/problems/course-schedule-ii/)
*   [2115. Find All Possible Recipes from Given Supplies](https://leetcode.com/problems/find-all-possible-recipes-from-given-supplies/) 1679
*   [2392. Build a Matrix with Conditions](https://leetcode.com/problems/build-a-matrix-with-conditions/) 1961
*   [802. Find Eventual Safe States](https://leetcode.com/problems/find-eventual-safe-states/) 1962
*   [1591. Strange Printer Ii](https://leetcode.com/problems/strange-printer-ii/) 2291
*   [1203. Sort Items by Groups Respecting Dependencies](https://leetcode.com/problems/sort-items-by-groups-respecting-dependencies/) 2419
*   [2603. Collect Coins in a Tree](https://leetcode.com/problems/collect-coins-in-a-tree/) 2712
*   [LCR 114. Jf1jut](https://leetcode.com/problems/Jf1JuT/)
*   [444. Sequence Reconstruction](https://leetcode.com/problems/sequence-reconstruction/) (Premium)
*   [3481. Apply Substitutions](https://leetcode.com/problems/apply-substitutions/) (Premium)
*   [269. Alien Dictionary](https://leetcode.com/problems/alien-dictionary/) (Premium)
*   [1059. All Paths from Source Lead to Destination](https://leetcode.com/problems/all-paths-from-source-lead-to-destination/) (Premium)

**Advanced Thinking**:

*   [310. Minimum Height Trees](https://leetcode.com/problems/minimum-height-trees/)
*   [1361. Validate Binary Tree Nodes](https://leetcode.com/problems/validate-binary-tree-nodes/)

### §2.2 DP on Topological Order

*   [851. Loud and Rich](https://leetcode.com/problems/loud-and-rich/) 1783
*   [2050. Parallel Courses Iii](https://leetcode.com/problems/parallel-courses-iii/) 2084
*   [3620. Network Recovery Pathways](https://leetcode.com/problems/network-recovery-pathways/)
*   [1857. Largest Color Value in a Directed Graph](https://leetcode.com/problems/largest-color-value-in-a-directed-graph/) 2313
*   [1136. Parallel Courses](https://leetcode.com/problems/parallel-courses/) (Premium)

### §2.3 Functional Graph (Rho Graph)

*   [2359. Find Closest Node to Given Two Nodes](https://leetcode.com/problems/find-closest-node-to-given-two-nodes/) 1715
*   [2360. Longest Cycle in a Graph](https://leetcode.com/problems/longest-cycle-in-a-graph/) 1897
*   [684. Redundant Connection](https://leetcode.com/problems/redundant-connection/)
*   [685. Redundant Connection Ii](https://leetcode.com/problems/redundant-connection-ii/)
*   [2876. Count Visited Nodes in a Directed Graph](https://leetcode.com/problems/count-visited-nodes-in-a-directed-graph/) 2210
*   [2127. Maximum Employees to Be Invited to a Meeting](https://leetcode.com/problems/maximum-employees-to-be-invited-to-a-meeting/) 2449
*   [2836. Maximize Value of Function in a Ball Passing Game](https://leetcode.com/problems/maximize-value-of-function-in-a-ball-passing-game/) 2769
*   [LCP 21. Za25ha](https://leetcode.com/problems/Za25hA/)
*   [2204. Distance to a Cycle in Undirected Graph](https://leetcode.com/problems/distance-to-a-cycle-in-undirected-graph/) (Premium)

**Advanced Thinking**:

*   [287. Find the Duplicate Number](https://leetcode.com/problems/find-the-duplicate-number/)

-----

### §3.1 Single-Source Shortest Path: Dijkstra

Template:

Python3

Java

C++

Go

    def shortestPathDijkstra(n: int, edges: List[List[int]], start: int) -> List[int]:
        g = [[] for _ in range(n)]  # adjacency list
        for x, y, wt in edges:
            g[x].append((y, wt))

        dis = [inf] * n

        while h:
            dis_x, x = heappop(h)
                continue
            for y, wt in g[x]:
                new_dis_y = dis_x + wt
                if new_dis_y < dis[y]:
                    heappush(h, (new_dis_y, y))

        return dis

*   [743. Network Delay Time](https://leetcode.com/problems/network-delay-time/)
*   [3341. Find Minimum Time to Reach Last Room I](https://leetcode.com/problems/find-minimum-time-to-reach-last-room-i/) 1721
*   [3112. Minimum Time to Visit Disappearing Nodes](https://leetcode.com/problems/minimum-time-to-visit-disappearing-nodes/) 1757
*   [2642. Design Graph with Shortest Path Calculator](https://leetcode.com/problems/design-graph-with-shortest-path-calculator/) 1811
*   [3604. Minimum Time to Reach Destination in Directed Graph](https://leetcode.com/problems/minimum-time-to-reach-destination-in-directed-graph/) 1845
*   [1514. Path with Maximum Probability](https://leetcode.com/problems/path-with-maximum-probability/) 1846
*   [3650. Minimum Cost Path with Edge Reversals](https://leetcode.com/problems/minimum-cost-path-with-edge-reversals/) 1854
*   [3342. Find Minimum Time to Reach Last Room Ii](https://leetcode.com/problems/find-minimum-time-to-reach-last-room-ii/) 1862
*   [1631. Path with Minimum Effort](https://leetcode.com/problems/path-with-minimum-effort/) 1948
*   [1786. Number of Restricted Paths from First to Last Node](https://leetcode.com/problems/number-of-restricted-paths-from-first-to-last-node/) 2079
*   [3123. Find Edges in Shortest Paths](https://leetcode.com/problems/find-edges-in-shortest-paths/) 2093
*   [1976. Number of Ways to Arrive at Destination](https://leetcode.com/problems/number-of-ways-to-arrive-at-destination/) 2095
*   [778. Swim in Rising Water](https://leetcode.com/problems/swim-in-rising-water/) 2097
*   [2662. Minimum Cost of a Path with Special Roads](https://leetcode.com/problems/minimum-cost-of-a-path-with-special-roads/) 2154
*   [3377. Digit Operations to Make Two Integers Equal](https://leetcode.com/problems/digit-operations-to-make-two-integers-equal/) 2186
*   [2045. Second Minimum Time to Reach Destination](https://leetcode.com/problems/second-minimum-time-to-reach-destination/) 2202  BFS
*   [3419. Minimize the Maximum Edge Weight of Graph](https://leetcode.com/problems/minimize-the-maximum-edge-weight-of-graph/) 2243
*   [882. Reachable Nodes in Subdivided Graph](https://leetcode.com/problems/reachable-nodes-in-subdivided-graph/) 2328
*   [2203. Minimum Weighted Subgraph with the Required Paths](https://leetcode.com/problems/minimum-weighted-subgraph-with-the-required-paths/) 2364
*   [2577. Minimum Time to Visit a Cell in a Grid](https://leetcode.com/problems/minimum-time-to-visit-a-cell-in-a-grid/) 2382
*   [818. Race Car](https://leetcode.com/problems/race-car/) 2392
*   [1928. Minimum Cost to Reach Destination in Time](https://leetcode.com/problems/minimum-cost-to-reach-destination-in-time/) 2413
*   [787. Cheapest Flights Within K Stops](https://leetcode.com/problems/cheapest-flights-within-k-stops/) 1928
*   [2699. Modify Graph Edge Weights](https://leetcode.com/problems/modify-graph-edge-weights/) 2874
*   [1810. Minimum Path Cost in a Hidden Grid](https://leetcode.com/problems/minimum-path-cost-in-a-hidden-grid/) (Premium)
*   [2093. Minimum Cost to Reach City with Discounts](https://leetcode.com/problems/minimum-cost-to-reach-city-with-discounts/) (Premium)
*   [2473. Minimum Cost to Buy Apples](https://leetcode.com/problems/minimum-cost-to-buy-apples/) (Premium)
*   [2737. Find the Closest Marked Node](https://leetcode.com/problems/find-the-closest-marked-node/) (Premium)

**Layered Graph Shortest Path**:

*   [LCP 35. Dfpefj](https://leetcode.com/problems/DFPeFJ/)
*   [3599. Partition Array to Minimize Xor](https://leetcode.com/problems/partition-array-to-minimize-xor/)
*   [3594. Minimum Time to Transport All Individuals](https://leetcode.com/problems/minimum-time-to-transport-all-individuals/) 2604
*   [2714. Find Shortest Path with K Hops](https://leetcode.com/problems/find-shortest-path-with-k-hops/) (Premium)

**SPFA and Difference Constraints**:

*   [2589. Minimum Time to Complete All Tasks](https://leetcode.com/problems/minimum-time-to-complete-all-tasks/) 2381

### §3.2 All-Pairs Shortest Path: Floyd

Template:

Python3

Java

C++

Go

    def shortestPathFloyd(self, n: int, edges: List[List[int]]) -> List[List[int]]:
        f = [[inf] * n for _ in range(n)]
        for i in range(n):
            f[i][i] = 0

        for x, y, wt in edges:
            f[y][x] = min(f[y][x], wt)  # undirected graph

        for k in range(n):
            for i in range(n):
                    continue
                for j in range(n):
                    f[i][j] = min(f[i][j], f[i][k] + f[k][j])
        return f

*   [2642. Design Graph with Shortest Path Calculator](https://leetcode.com/problems/design-graph-with-shortest-path-calculator/) 1811
*   [1334. Find the City with the Smallest Number of Neighbors at a Threshold Distance](https://leetcode.com/problems/find-the-city-with-the-smallest-number-of-neighbors-at-a-threshold-distance/) 1855
*   [2976. Minimum Cost to Convert String I](https://leetcode.com/problems/minimum-cost-to-convert-string-i/) 1882
*   [2959. Number of Possible Sets of Closing Branches](https://leetcode.com/problems/number-of-possible-sets-of-closing-branches/) 2077
*   [2977. Minimum Cost to Convert String Ii](https://leetcode.com/problems/minimum-cost-to-convert-string-ii/) 2696

**Bitset-Optimized Floyd**

*   [1462. Course Schedule Iv](https://leetcode.com/problems/course-schedule-iv/) 1693
*   [2101. Detonate the Maximum Bombs](https://leetcode.com/problems/detonate-the-maximum-bombs/)

-------

Python3

Java

C++

Go

    class UnionFind:
        def __init__(self, n: int):
            self._fa = list(range(n))  # representative

        def find(self, x: int) -> int:
            if self._fa[x] != x:
            return self._fa[x]

        def merge(self, from_: int, to: int) -> bool:
            x, y = self.find(from_), self.find(to)
                return False
            return True

    def mstKruskal(n: int, edges: List[List[int]]) -> int:
        edges.sort(key=lambda e: e[2])

        uf = UnionFind(n)
        sum_wt = 0
        for x, y, wt in edges:
            if uf.merge(x, y):
                sum_wt += wt

            return inf
        return sum_wt

*   [1584. Min Cost to Connect All Points](https://leetcode.com/problems/min-cost-to-connect-all-points/) 1858
*   [3600. Maximize Spanning Tree Stability with Upgrades](https://leetcode.com/problems/maximize-spanning-tree-stability-with-upgrades/) 2301
*   [1489. Find Critical and Pseudo Critical Edges in Minimum Spanning Tree](https://leetcode.com/problems/find-critical-and-pseudo-critical-edges-in-minimum-spanning-tree/) 2572
*   [1135. Connecting Cities with Minimum Cost](https://leetcode.com/problems/connecting-cities-with-minimum-cost/) (Premium)
*   [1168. Optimize Water Distribution in a Village](https://leetcode.com/problems/optimize-water-distribution-in-a-village/) (Premium)

**Advanced Thinking**

*   [3219. Minimum Cost for Cutting Cake Ii](https://leetcode.com/problems/minimum-cost-for-cutting-cake-ii/)

-----------

*   [332. Reconstruct Itinerary](https://leetcode.com/problems/reconstruct-itinerary/)
*   [753. Cracking the Safe](https://leetcode.com/problems/cracking-the-safe/) 2274
*   [2097. Valid Arrangement of Pairs](https://leetcode.com/problems/valid-arrangement-of-pairs/) 2651

-------------

*   [1192. Critical Connections in a Network](https://leetcode.com/problems/critical-connections-in-a-network/) 2085
*   [1568. Minimum Number of Days to Disconnect Island](https://leetcode.com/problems/minimum-number-of-days-to-disconnect-island/) 2209
*   [LCP 54. S5kipk](https://leetcode.com/problems/s5kipK/)
*   [3383. Minimum Runes to Add to Cast Spell](https://leetcode.com/problems/minimum-runes-to-add-to-cast-spell/) (Premium)

## Bipartite Graph Coloring
-------

Python3

Java

C++

Go

    def colorBipartite(n: int, edges: List[List[int]]) -> List[int]:
        g = [[] for _ in range(n)]
        for x, y in edges:
            g[x].append(y)
            g[y].append(x)

        colors = [0] * n

        def dfs(x: int, c: int) -> bool:
            for y in g[x]:
                if colors[y] == c or \
                    return False
            return True

        for i, c in enumerate(colors):
            if c == 0 and not dfs(i, 1):
                return []
        return colors

*   [785. Is Graph Bipartite](https://leetcode.com/problems/is-graph-bipartite/) 1625
*   [886. Possible Bipartition](https://leetcode.com/problems/possible-bipartition/) 1795
*   [3710. Maximum Partition Factor](https://leetcode.com/problems/maximum-partition-factor/)

-----

*   [1947. Maximum Compatibility Score Sum](https://leetcode.com/problems/maximum-compatibility-score-sum/) 1704
*   [3376. Minimum Time to Break Locks I](https://leetcode.com/problems/minimum-time-to-break-locks-i/) 1793
*   [2850. Minimum Moves to Spread Stones Over Grid](https://leetcode.com/problems/minimum-moves-to-spread-stones-over-grid/) 2001
*   [1879. Minimum Xor Sum of Two Arrays](https://leetcode.com/problems/minimum-xor-sum-of-two-arrays/) 2145
*   [1349. Maximum Students Taking Exam](https://leetcode.com/problems/maximum-students-taking-exam/) 2386
*   [2172. Maximum and Sum of Array](https://leetcode.com/problems/maximum-and-sum-of-array/) 2392
*   [3276. Select Cells in Grid with Maximum Score](https://leetcode.com/problems/select-cells-in-grid-with-maximum-score/) 2403
*   [1595. Minimum Cost to Connect Two Groups of Points](https://leetcode.com/problems/minimum-cost-to-connect-two-groups-of-points/) 2538
*   [3257. Maximum Value Sum by Placing Three Rooks Ii](https://leetcode.com/problems/maximum-value-sum-by-placing-three-rooks-ii/) 2553
*   [LCP 04. Broken Board Dominoes](https://leetcode.com/problems/broken-board-dominoes/) ·
*   [LCP 38. 7rlgcr](https://leetcode.com/problems/7rLGCR/)
*   [1820. Maximum Number of Accepted Invitations](https://leetcode.com/problems/maximum-number-of-accepted-invitations/) (Premium)·
*   [2403. Minimum Time to Kill All Monsters](https://leetcode.com/problems/minimum-time-to-kill-all-monsters/) (Premium)
*   [3385. Minimum Time to Break Locks Ii](https://leetcode.com/problems/minimum-time-to-break-locks-ii/) (Premium)
*   [1066. Campus Bikes Ii](https://leetcode.com/problems/campus-bikes-ii/) (Premium)，
*   [2123. Minimum Operations to Remove Adjacent Ones in Matrix](https://leetcode.com/problems/minimum-operations-to-remove-adjacent-ones-in-matrix/) (Premium)

**Simulated Min-Cost Flow**

*   [2463. Minimum Total Distance Traveled](https://leetcode.com/problems/minimum-total-distance-traveled/) log(n+m))

## Others
----

*   [1042. Flower Planting with No Adjacent](https://leetcode.com/problems/flower-planting-with-no-adjacent/) 1712
*   [1761. Minimum Degree of a Connected Trio in a Graph](https://leetcode.com/problems/minimum-degree-of-a-connected-trio-in-a-graph/) 2005
*   [2508. Add Edges to Make Degrees of All Nodes Even](https://leetcode.com/problems/add-edges-to-make-degrees-of-all-nodes-even/) 2060
*   [1579. Remove Max Number of Edges to Keep Graph Fully Traversable](https://leetcode.com/problems/remove-max-number-of-edges-to-keep-graph-fully-traversable/) 2132
*   [2065. Maximum Path Quality of a Graph](https://leetcode.com/problems/maximum-path-quality-of-a-graph/) 2178
*   [1697. Checking Existence of Edge Length Limited Paths](https://leetcode.com/problems/checking-existence-of-edge-length-limited-paths/) 2300
*   [2242. Maximum Score of a Node Sequence](https://leetcode.com/problems/maximum-score-of-a-node-sequence/) 2304
*   [2493. Divide Nodes Into the Maximum Number of Groups](https://leetcode.com/problems/divide-nodes-into-the-maximum-number-of-groups/) 2415 ****
*   [1782. Count Pairs of Nodes](https://leetcode.com/problems/count-pairs-of-nodes/) 2457
*   [3666. Minimum Operations to Equalize Binary String](https://leetcode.com/problems/minimum-operations-to-equalize-binary-string/) 2477  BFS / Gale-Ryser
*   [2612. Minimum Reverse Operations](https://leetcode.com/problems/minimum-reverse-operations/) 2824  BFS
*   [3435. Frequencies of Shortest Supersequences](https://leetcode.com/problems/frequencies-of-shortest-supersequences/) 3028
*   [466. Count the Repetitions](https://leetcode.com/problems/count-the-repetitions/)
*   [LCP 16. You Le Yuan De You Lan Ji Hua](https://leetcode.com/problems/you-le-yuan-de-you-lan-ji-hua/)
*   [277. Find the Celebrity](https://leetcode.com/problems/find-the-celebrity/) (Premium)
*   [1724. Checking Existence of Edge Length Limited Paths Ii](https://leetcode.com/problems/checking-existence-of-edge-length-limited-paths-ii/) (Premium)
*   [2077. Paths in Maze that Lead to Same Room](https://leetcode.com/problems/paths-in-maze-that-lead-to-same-room/) (Premium)
*   [3656. Determine If a Simple Graph Exists](https://leetcode.com/problems/determine-if-a-simple-graph-exists/) (Premium)Erdős–Gallai

------


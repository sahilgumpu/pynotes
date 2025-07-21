---
title: Dsa
date: 2025-07-21
author: Your Name
cell_count: 58
score: 55
---

```python
stack = []

# Push
stack.append(10)
stack.append(20)
stack.append(30)

# Pop
print(stack.pop())  # 30
print(stack)        # [10, 20]

```

    30
    [10, 20]
    


```python
from collections import deque

queue = deque()

# Enqueue
queue.append(1)
queue.append(2)
queue.append(3)

# Dequeue
print(queue.popleft())  # 1
print(queue)            # deque([2, 3])

```

    1
    deque([2, 3])
    


```python
def binary_search(arr, target):
    low, high = 0, len(arr) - 1
    
    while low <= high:
        mid = (low + high) // 2
        
        if arr[mid] == target:
            return mid
        elif arr[mid] < target:
            low = mid + 1
        else:
            high = mid - 1
            
    return -1

arr = [1, 3, 5, 7, 9]
print(binary_search(arr, 7))  # Output: 3

```

    3
    


```python
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None

class LinkedList:
    def __init__(self):
        self.head = None
    
    def insert(self, data):
        new_node = Node(data)
        new_node.next = self.head
        self.head = new_node
    
    def display(self):
        curr = self.head
        while curr:
            print(curr.data, end=' -> ')
            curr = curr.next
        print("None")

ll = LinkedList()
ll.insert(10)
ll.insert(20)
ll.insert(30)
ll.display()

```

    30 -> 20 -> 10 -> None
    


```python
def linear_search(arr, target):
    for i in range(len(arr)):
        if arr[i] == target:
            return i
    return -1

print(linear_search([10, 20, 30, 40], 30))  # Output: 2

```

    2
    


```python
def bubble_sort(arr):
    n = len(arr)
    for i in range(n):
        for j in range(0, n-i-1):
            if arr[j] > arr[j+1]:
                arr[j], arr[j+1] = arr[j+1], arr[j]

arr = [64, 25, 12, 22, 11]
bubble_sort(arr)
print("Sorted array:", arr)

```

    Sorted array: [11, 12, 22, 25, 64]
    


```python
def factorial(n):
    if n == 0 or n == 1:
        return 1
    return n * factorial(n-1)

print(factorial(5))  # Output: 120

```

    120
    


```python
def fib(n, memo={}):
    if n <= 1:
        return n
    if n not in memo:
        memo[n] = fib(n-1, memo) + fib(n-2, memo)
    return memo[n]

print(fib(10))  # Output: 55

```

    55
    


```python
class Stack:
    def __init__(self):
        self.stack = []

    def push(self, data):
        self.stack.append(data)

    def pop(self):
        if not self.is_empty():
            return self.stack.pop()

    def peek(self):
        return self.stack[-1] if not self.is_empty() else None

    def is_empty(self):
        return len(self.stack) == 0

s = Stack()
s.push(10)
s.push(20)
print(s.pop())  # Output: 20

```

    20
    


```python
class Queue:
    def __init__(self):
        self.queue = []

    def enqueue(self, data):
        self.queue.append(data)

    def dequeue(self):
        if not self.is_empty():
            return self.queue.pop(0)

    def is_empty(self):
        return len(self.queue) == 0

q = Queue()
q.enqueue(5)
q.enqueue(10)
print(q.dequeue())  # Output: 5

```

    5
    


```python
class Node:
    def __init__(self, key):
        self.left = None
        self.right = None
        self.val = key

def inorder(root):
    if root:
        inorder(root.left)
        print(root.val, end=' ')
        inorder(root.right)

# Example tree
root = Node(1)
root.left = Node(2)
root.right = Node(3)
root.left.left = Node(4)

inorder(root)  # Output: 4 2 1 3

```

    4 2 1 3 


```python
from collections import defaultdict, deque

class Graph:
    def __init__(self):
        self.graph = defaultdict(list)

    def add_edge(self, u, v):
        self.graph[u].append(v)

    def bfs(self, start):
        visited = set()
        queue = deque([start])
        while queue:
            node = queue.popleft()
            if node not in visited:
                print(node, end=' ')
                visited.add(node)
                queue.extend(self.graph[node])

    def dfs(self, node, visited=set()):
        if node not in visited:
            print(node, end=' ')
            visited.add(node)
            for neighbour in self.graph[node]:
                self.dfs(neighbour, visited)

g = Graph()
g.add_edge(0, 1)
g.add_edge(0, 2)
g.add_edge(1, 3)
g.add_edge(2, 4)

print("BFS:")
g.bfs(0)  # Output: 0 1 2 3 4
print("\nDFS:")
g.dfs(0)  # Output: 0 1 3 2 4

```

    BFS:
    0 1 2 3 4 
    DFS:
    0 1 3 2 4 


```python
def knapsack(weights, values, W, n):
    if n == 0 or W == 0:
        return 0
    if weights[n-1] <= W:
        return max(
            values[n-1] + knapsack(weights, values, W - weights[n-1], n - 1),
            knapsack(weights, values, W, n - 1)
        )
    else:
        return knapsack(weights, values, W, n - 1)

weights = [1, 3, 4, 5]
values = [1, 4, 5, 7]
W = 7
n = len(weights)
print(knapsack(weights, values, W, n))  # Output: 9

```

    9
    


```python
def selection_sort(arr):
    for i in range(len(arr)):
        min_idx = i
        for j in range(i+1, len(arr)):
            if arr[j] < arr[min_idx]:
                min_idx = j
        arr[i], arr[min_idx] = arr[min_idx], arr[i]

arr = [64, 25, 12, 22, 11]
selection_sort(arr)
print("Sorted array:", arr)

```

    Sorted array: [11, 12, 22, 25, 64]
    


```python
def insertion_sort(arr):
    for i in range(1, len(arr)):
        key = arr[i]
        j = i - 1
        while j >= 0 and arr[j] > key:
            arr[j+1] = arr[j]
            j -= 1
        arr[j+1] = key

arr = [12, 11, 13, 5, 6]
insertion_sort(arr)
print("Sorted array:", arr)

```

    Sorted array: [5, 6, 11, 12, 13]
    


```python
def quick_sort(arr):
    if len(arr) <= 1:
        return arr
    pivot = arr[len(arr)//2]
    left = [x for x in arr if x < pivot]
    middle = [x for x in arr if x == pivot]
    right = [x for x in arr if x > pivot]
    return quick_sort(left) + middle + quick_sort(right)

arr = [10, 7, 8, 9, 1, 5]
print("Sorted array:", quick_sort(arr))

```

    Sorted array: [1, 5, 7, 8, 9, 10]
    


```python
def is_palindrome(s):
    return s == s[::-1]

print(is_palindrome("radar"))  # True
print(is_palindrome("hello"))  # False

```

    True
    False
    


```python
def is_anagram(str1, str2):
    return sorted(str1) == sorted(str2)

print(is_anagram("listen", "silent"))  # True
print(is_anagram("hello", "world"))    # False

```

    True
    False
    


```python
def lcs(X, Y):
    m = len(X)
    n = len(Y)
    L = [[None]*(n+1) for i in range(m+1)]

    for i in range(m+1):
        for j in range(n+1):
            if i == 0 or j == 0:
                L[i][j] = 0
            elif X[i-1] == Y[j-1]:
                L[i][j] = L[i-1][j-1] + 1
            else:
                L[i][j] = max(L[i-1][j], L[i][j-1])

    return L[m][n]

print(lcs("AGGTAB", "GXTXAYB"))  # Output: 4

```

    4
    


```python
from collections import deque

class Node:
    def __init__(self, val):
        self.left = None
        self.right = None
        self.val = val

def level_order(root):
    if not root:
        return
    queue = deque([root])
    while queue:
        node = queue.popleft()
        print(node.val, end=' ')
        if node.left:
            queue.append(node.left)
        if node.right:
            queue.append(node.right)

root = Node(1)
root.left = Node(2)
root.right = Node(3)
root.left.left = Node(4)

level_order(root)  # Output: 1 2 3 4

```

    1 2 3 4 


```python
def has_cycle(graph, node, visited, parent):
    visited.add(node)
    for neighbor in graph[node]:
        if neighbor not in visited:
            if has_cycle(graph, neighbor, visited, node):
                return True
        elif neighbor != parent:
            return True
    return False

graph = {
    0: [1, 2],
    1: [0, 3],
    2: [0],
    3: [1]
}

visited = set()
print("Cycle Detected" if has_cycle(graph, 0, visited, -1) else "No Cycle")

```

    No Cycle
    


```python
def transpose(matrix):
    return [[matrix[j][i] for j in range(len(matrix))] for i in range(len(matrix[0]))]

matrix = [
    [1, 2, 3],
    [4, 5, 6]
]
print(transpose(matrix))  # Output: [[1, 4], [2, 5], [3, 6]]

```

    [[1, 4], [2, 5], [3, 6]]
    


```python
def find_missing(arr, n):
    total = n * (n + 1) // 2
    return total - sum(arr)

arr = [1, 2, 4, 5, 6]
print(find_missing(arr, 6))  # Output: 3

```

    3
    


```python
# Head recursion
def head_rec(n):
    if n == 0:
        return
    head_rec(n - 1)
    print(n)

# Tail recursion
def tail_rec(n):
    if n == 0:
        return
    print(n)
    tail_rec(n - 1)

head_rec(3)  # Output: 1 2 3
tail_rec(3)  # Output: 3 2 1

```

    1
    2
    3
    3
    2
    1
    


```python
def max_sum_subarray(arr, k):
    max_sum = cur_sum = sum(arr[:k])
    for i in range(k, len(arr)):
        cur_sum += arr[i] - arr[i - k]
        max_sum = max(max_sum, cur_sum)
    return max_sum

print(max_sum_subarray([2, 1, 5, 1, 3, 2], 3))  # Output: 9

```

    9
    


```python
def max_subarray_sum(nums):
    max_sum = curr = nums[0]
    for num in nums[1:]:
        curr = max(num, curr + num)
        max_sum = max(max_sum, curr)
    return max_sum

print(max_subarray_sum([-2,1,-3,4,-1,2,1,-5,4]))  # Output: 6

```

    6
    


```python
from collections import Counter

arr = [1, 2, 2, 3, 4, 1, 2]
freq = Counter(arr)
print(freq)  # Output: {1:2, 2:3, 3:1, 4:1}


```

    Counter({2: 3, 1: 2, 3: 1, 4: 1})
    


```python
import heapq

nums = [4, 1, 7, 3, 8, 5]
heapq.heapify(nums)
print(heapq.heappop(nums))  # 1 (min value)

```

    1
    


```python
class TrieNode:
    def __init__(self):
        self.children = {}
        self.end = False

class Trie:
    def __init__(self):
        self.root = TrieNode()
    
    def insert(self, word):
        node = self.root
        for ch in word:
            if ch not in node.children:
                node.children[ch] = TrieNode()
            node = node.children[ch]
        node.end = True

    def search(self, word):
        node = self.root
        for ch in word:
            if ch not in node.children:
                return False
            node = node.children[ch]
        return node.end

t = Trie()
t.insert("apple")
print(t.search("apple"))  # True
print(t.search("app"))    # False

```

    True
    False
    


```python
def topo_sort(graph):
    visited = set()
    stack = []

    def dfs(node):
        visited.add(node)
        for neighbor in graph.get(node, []):
            if neighbor not in visited:
                dfs(neighbor)
        stack.append(node)

    for node in graph:
        if node not in visited:
            dfs(node)

    return stack[::-1]

graph = {
    5: [2, 0],
    4: [0, 1],
    2: [3],
    3: [1],
    1: [],
    0: []
}
print(topo_sort(graph))  # One valid output: [4, 5, 2, 3, 1, 0]

```

    [4, 5, 0, 2, 3, 1]
    


```python
def is_safe(board, row, col, n):
    for i in range(row):
        if board[i][col] == 1:
            return False
        if col - (row - i) >= 0 and board[i][col - (row - i)] == 1:
            return False
        if col + (row - i) < n and board[i][col + (row - i)] == 1:
            return False
    return True

def solve_n_queens(n):
    def solve(board, row):
        if row == n:
            result.append([row[:] for row in board])
            return
        for col in range(n):
            if is_safe(board, row, col, n):
                board[row][col] = 1
                solve(board, row + 1)
                board[row][col] = 0

    board = [[0]*n for _ in range(n)]
    result = []
    solve(board, 0)
    return result

solutions = solve_n_queens(4)
for sol in solutions:
    for row in sol:
        print(row)
    print()

```

    [0, 1, 0, 0]
    [0, 0, 0, 1]
    [1, 0, 0, 0]
    [0, 0, 1, 0]
    
    [0, 0, 1, 0]
    [1, 0, 0, 0]
    [0, 0, 0, 1]
    [0, 1, 0, 0]
    
    


```python
def ternary_search(l, r, key, arr):
    while r >= l:
        mid1 = l + (r - l) // 3
        mid2 = r - (r - l) // 3

        if arr[mid1] == key:
            return mid1
        if arr[mid2] == key:
            return mid2

        if key < arr[mid1]:
            r = mid1 - 1
        elif key > arr[mid2]:
            l = mid2 + 1
        else:
            l = mid1 + 1
            r = mid2 - 1
    return -1

arr = [1, 2, 3, 4, 5, 6, 7]
print(ternary_search(0, len(arr)-1, 5, arr))  # Output: 4

```

    4
    


```python
def count_inversions(arr):
    def merge_sort(arr):
        if len(arr) <= 1:
            return arr, 0
        mid = len(arr) // 2
        left, inv_left = merge_sort(arr[:mid])
        right, inv_right = merge_sort(arr[mid:])
        merged, inv_split = merge(left, right)
        return merged, inv_left + inv_right + inv_split

    def merge(left, right):
        merged = []
        i = j = inv_count = 0
        while i < len(left) and j < len(right):
            if left[i] <= right[j]:
                merged.append(left[i])
                i += 1
            else:
                merged.append(right[j])
                inv_count += len(left) - i
                j += 1
        merged += left[i:]
        merged += right[j:]
        return merged, inv_count

    _, inv_count = merge_sort(arr)
    return inv_count

print(count_inversions([1, 20, 6, 4, 5]))  # Output: 5


```

    5
    


```python
class DSU:
    def __init__(self, n):
        self.parent = list(range(n))

    def find(self, x):
        if self.parent[x] != x:
            self.parent[x] = self.find(self.parent[x])
        return self.parent[x]

    def union(self, x, y):
        self.parent[self.find(x)] = self.find(y)

dsu = DSU(5)
dsu.union(0, 1)
dsu.union(1, 2)
print(dsu.find(0) == dsu.find(2))  # True

```

    True
    


```python
def binary_search(arr, l, r, x):
    if r >= l:
        mid = (l + r) // 2
        if arr[mid] == x:
            return mid
        elif arr[mid] > x:
            return binary_search(arr, l, mid - 1, x)
        else:
            return binary_search(arr, mid + 1, r, x)
    return -1

arr = [2, 3, 4, 10, 40]
print(binary_search(arr, 0, len(arr) - 1, 10))  # Output: 3

```

    3
    


```python
def search_matrix(matrix, target):
    if not matrix:
        return False
    row, col = 0, len(matrix[0]) - 1
    while row < len(matrix) and col >= 0:
        if matrix[row][col] == target:
            return True
        elif matrix[row][col] > target:
            col -= 1
        else:
            row += 1
    return False

matrix = [[1, 4, 7], [8, 11, 15], [17, 20, 23]]
print(search_matrix(matrix, 11))  # True

```

    True
    


```python
def flood_fill(image, sr, sc, newColor):
    original = image[sr][sc]
    if original == newColor:
        return image

    def dfs(r, c):
        if 0 <= r < len(image) and 0 <= c < len(image[0]) and image[r][c] == original:
            image[r][c] = newColor
            dfs(r+1, c)
            dfs(r-1, c)
            dfs(r, c+1)
            dfs(r, c-1)

    dfs(sr, sc)
    return image

image = [[1,1,1],[1,1,0],[1,0,1]]
print(flood_fill(image, 1, 1, 2))

```

    [[2, 2, 2], [2, 2, 0], [2, 0, 1]]
    


```python
import heapq

def dijkstra(graph, start):
    heap = [(0, start)]
    distances = {node: float('inf') for node in graph}
    distances[start] = 0

    while heap:
        current_dist, current_node = heapq.heappop(heap)
        if current_dist > distances[current_node]:
            continue
        for neighbor, weight in graph[current_node]:
            distance = current_dist + weight
            if distance < distances[neighbor]:
                distances[neighbor] = distance
                heapq.heappush(heap, (distance, neighbor))
    return distances

graph = {
    'A': [('B', 1), ('C', 4)],
    'B': [('C', 2), ('D', 5)],
    'C': [('D', 1)],
    'D': []
}
print(dijkstra(graph, 'A'))  # {'A': 0, 'B': 1, 'C': 3, 'D': 4}

```

    {'A': 0, 'B': 1, 'C': 3, 'D': 4}
    


```python
def permute(nums):
    res = []
    def backtrack(path, options):
        if not options:
            res.append(path)
            return
        for i in range(len(options)):
            backtrack(path + [options[i]], options[:i] + options[i+1:])
    backtrack([], nums)
    return res

print(permute([1, 2, 3]))

```

    [[1, 2, 3], [1, 3, 2], [2, 1, 3], [2, 3, 1], [3, 1, 2], [3, 2, 1]]
    


```python
def longest_palindrome(s):
    n = len(s)
    dp = [[False]*n for _ in range(n)]
    start = 0
    max_len = 1

    for i in range(n):
        dp[i][i] = True

    for length in range(2, n+1):
        for i in range(n-length+1):
            j = i+length-1
            if s[i] == s[j] and (length == 2 or dp[i+1][j-1]):
                dp[i][j] = True
                if length > max_len:
                    start = i
                    max_len = length

    return s[start:start+max_len]

print(longest_palindrome("babad"))  # Output: "bab" or "aba"

```

    bab
    


```python
def find_duplicate(nums):
    slow = fast = nums[0]
    while True:
        slow = nums[slow]
        fast = nums[nums[fast]]
        if slow == fast:
            break

    slow = nums[0]
    while slow != fast:
        slow = nums[slow]
        fast = nums[fast]

    return slow

print(find_duplicate([1,3,4,2,2]))  # Output: 2

```

    2
    


```python
def find_duplicate(nums):
    slow = fast = nums[0]
    while True:
        slow = nums[slow]
        fast = nums[nums[fast]]
        if slow == fast:
            break

    slow = nums[0]
    while slow != fast:
        slow = nums[slow]
        fast = nums[fast]

    return slow

print(find_duplicate([1,3,4,2,2]))  # Output: 2

```

    2
    


```python
def max_area(height):
    l, r = 0, len(height) - 1
    max_area = 0
    while l < r:
        area = min(height[l], height[r]) * (r - l)
        max_area = max(max_area, area)
        if height[l] < height[r]:
            l += 1
        else:
            r -= 1
    return max_area

print(max_area([1,8,6,2,5,4,8,3,7]))  # Output: 49

```

    49
    


```python
import heapq

def kth_largest(nums, k):
    return heapq.nlargest(k, nums)[-1]

print(kth_largest([3, 2, 1, 5, 6, 4], 2))  # Output: 5

```

    5
    


```python
def next_greater(nums):
    res = [-1] * len(nums)
    stack = []
    for i in range(len(nums)):
        while stack and nums[i] > nums[stack[-1]]:
            res[stack.pop()] = nums[i]
        stack.append(i)
    return res

print(next_greater([2, 1, 2, 4, 3]))  # Output: [4, 2, 4, -1, -1]

```

    [4, 2, 4, -1, -1]
    


```python
def subsets(nums):
    res = []
    def backtrack(start, path):
        res.append(path)
        for i in range(start, len(nums)):
            backtrack(i + 1, path + [nums[i]])
    backtrack(0, [])
    return res

print(subsets([1, 2, 3]))

```

    [[], [1], [1, 2], [1, 2, 3], [1, 3], [2], [2, 3], [3]]
    


```python
def count_bits(n):
    count = 0
    while n:
        count += n & 1
        n >>= 1
    return count

print(count_bits(13))  # Output: 3 (1101 has 3 bits set)

```

    3
    


```python
def lis(nums):
    dp = [1] * len(nums)
    for i in range(len(nums)):
        for j in range(i):
            if nums[i] > nums[j]:
                dp[i] = max(dp[i], dp[j] + 1)
    return max(dp)

print(lis([10, 9, 2, 5, 3, 7, 101, 18]))  # Output: 4

```

    4
    


```python
from collections import OrderedDict

class LRUCache:
    def __init__(self, capacity: int):
        self.cache = OrderedDict()
        self.cap = capacity

    def get(self, key: int) -> int:
        if key not in self.cache:
            return -1
        self.cache.move_to_end(key)
        return self.cache[key]

    def put(self, key: int, value: int):
        if key in self.cache:
            self.cache.move_to_end(key)
        self.cache[key] = value
        if len(self.cache) > self.cap:
            self.cache.popitem(last=False)

lru = LRUCache(2)
lru.put(1, 1)
lru.put(2, 2)
print(lru.get(1))  # Output: 1
lru.put(3, 3)  # Evicts key 2
print(lru.get(2))  # Output: -1

```

    1
    -1
    


```python
def unique_paths(m, n):
    dp = [[1]*n for _ in range(m)]
    for i in range(1, m):
        for j in range(1, n):
            dp[i][j] = dp[i-1][j] + dp[i][j-1]
    return dp[-1][-1]

print(unique_paths(3, 7))  # Output: 28

```

    28
    


```python
def rotate(matrix):
    n = len(matrix)
    for i in range(n):
        for j in range(i):
            matrix[i][j], matrix[j][i] = matrix[j][i], matrix[i][j]
    for row in matrix:
        row.reverse()

mat = [[1,2,3],[4,5,6],[7,8,9]]
rotate(mat)
print(mat)  # Output: Rotated matrix

```

    [[7, 4, 1], [8, 5, 2], [9, 6, 3]]
    


```python
from collections import deque

def is_bipartite(graph):
    color = {}
    for node in graph:
        if node not in color:
            queue = deque([node])
            color[node] = 0
            while queue:
                current = queue.popleft()
                for neighbor in graph[current]:
                    if neighbor in color:
                        if color[neighbor] == color[current]:
                            return False
                    else:
                        color[neighbor] = 1 - color[current]
                        queue.append(neighbor)
    return True

graph = {
    0: [1, 3],
    1: [0, 2],
    2: [1, 3],
    3: [0, 2]
}
print(is_bipartite(graph))  # Output: True

```

    True
    


```python
class BIT:
    def __init__(self, n):
        self.tree = [0]*(n+1)

    def update(self, i, val):
        while i < len(self.tree):
            self.tree[i] += val
            i += i & -i

    def query(self, i):
        res = 0
        while i > 0:
            res += self.tree[i]
            i -= i & -i
        return res

bit = BIT(10)
bit.update(3, 1)
bit.update(5, 2)
print(bit.query(5))  # Output: 3

```

    3
    


```python
def power(x, n):
    res = 1
    while n:
        if n % 2:
            res *= x
        x *= x
        n //= 2
    return res

print(power(2, 10))  # Output: 1024

```

    1024
    


```python
def edit_distance(s1, s2):
    dp = [[0]*(len(s2)+1) for _ in range(len(s1)+1)]
    for i in range(len(s1)+1):
        for j in range(len(s2)+1):
            if i == 0:
                dp[i][j] = j
            elif j == 0:
                dp[i][j] = i
            elif s1[i-1] == s2[j-1]:
                dp[i][j] = dp[i-1][j-1]
            else:
                dp[i][j] = 1 + min(dp[i-1][j], dp[i][j-1], dp[i-1][j-1])
    return dp[-1][-1]

print(edit_distance("horse", "ros"))  # Output: 3

```

    3
    


```python
def job_scheduling(jobs):
    jobs.sort(key=lambda x: x[1], reverse=True)
    max_deadline = max(job[0] for job in jobs)
    slot = [-1] * (max_deadline + 1)
    count = 0

    for deadline, profit in jobs:
        for j in range(deadline, 0, -1):
            if slot[j] == -1:
                slot[j] = profit
                count += profit
                break

    return count

jobs = [(2, 100), (1, 19), (2, 27), (1, 25), (3, 15)]
print(job_scheduling(jobs))  # Output: max profit

```

    142
    


```python
def compute_lps(pattern):
    lps = [0] * len(pattern)
    length = 0
    i = 1
    while i < len(pattern):
        if pattern[i] == pattern[length]:
            length += 1
            lps[i] = length
            i += 1
        else:
            if length:
                length = lps[length - 1]
            else:
                i += 1
    return lps

def kmp(text, pattern):
    lps = compute_lps(pattern)
    i = j = 0
    while i < len(text):
        if text[i] == pattern[j]:
            i += 1
            j += 1
        if j == len(pattern):
            return i - j
        elif i < len(text) and text[i] != pattern[j]:
            if j:
                j = lps[j - 1]
            else:
                i += 1
    return -1

print(kmp("abxabcabcaby", "abcaby"))  # Output: 6

```

    6
    


```python

```


---
**Score: 55**
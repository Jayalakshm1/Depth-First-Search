Lab Experiment 2: Depth First Search

Write a program to implement depth first search.

```Program:

graph = {
    '2': ['3', '4'],
    '3': ['5'],
    '4': ['6', '7'],
    '6': [],
    '5': ['6'],
    '7': ['8'],
    '8': []
}

visited = set()  # Set for visited nodes.

def dfs(graph, node):  # Function for DFS
    if node not in visited:
        print(node, end=" ")
        visited.add(node)
        for neighbour in graph[node]:
            dfs(graph, neighbour)

# Driver Code
print("DFS order is")
dfs(graph, '2')
```
Output:

![Screenshot (2)](https://github.com/Jayalakshm1/Depth-First-Search/assets/130430542/9cf7c9ae-160c-4983-a444-4fad6f6471e6)

Result:

Thus,a program to implement depth first search was executed successfully.



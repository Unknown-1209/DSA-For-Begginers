| Data Structure | Operation          | Average Time Complexity | Worst Time Complexity | Space Complexity |
|-----------------|--------------------|-------------------------|-----------------------|------------------|
| **Arrays**      | Access             | O(1)                    | O(1)                  | O(1)             |
|                 | Search             | O(n)                    | O(n)                  | O(1)             |
|                 | Insert at end      | O(1)                    | O(1)                  | O(1)             |
|                 | Insert at start    | O(n)                    | O(n)                  | O(1)             |
|                 | Delete at end      | O(1)                    | O(1)                  | O(1)             |
|                 | Delete at start    | O(n)                    | O(n)                  | O(1)             |
| **Linked Lists**| Access             | O(n)                    | O(n)                  | O(1)             |
|                 | Search             | O(n)                    | O(n)                  | O(1)             |
|                 | Insert at end      | O(1)                    | O(1)                  | O(1)             |
|                 | Insert at start    | O(1)                    | O(1)                  | O(1)             |
|                 | Delete at end      | O(n)                    | O(n)                  | O(1)             |
|                 | Delete at start    | O(1)                    | O(1)                  | O(1)             |
| **Stacks**      | Push               | O(1)                    | O(1)                  | O(1)             |
|                 | Pop                | O(1)                    | O(1)                  | O(1)             |
|                 | Peek               | O(1)                    | O(1)                  | O(1)             |
| **Queues**      | Enqueue            | O(1)                    | O(1)                  | O(1)             |
|                 | Dequeue            | O(1)                    | O(1)                  | O(1)             |
|                 | Peek               | O(1)                    | O(1)                  | O(1)             |
| **Hash Tables** | Search             | O(1)                    | O(n)                  | O(n)             |
|                 | Insert             | O(1)                    | O(n)                  | O(n)             |
|                 | Delete             | O(1)                    | O(n)                  | O(n)             |
| **Trees**       | Search             | O(log n)                | O(n)                  | O(log n)         |
|                 | Insert             | O(log n)                | O(n)                  | O(1) or O(log n) |
|                 | Delete             | O(log n)                | O(n)                  | O(1) or O(log n) |
| **Heaps**       | Insert             | O(log n)                | O(log n)              | O(1)             |
|                 | Extract Min/Max    | O(log n)                | O(log n)              | O(1)             |
| **Graphs**      | Search (DFS, BFS)  | O(V + E)                | O(V + E)              | O(V)             |
|                 | Topological Sort   | O(V + E)                | O(V + E)              | O(V)             |

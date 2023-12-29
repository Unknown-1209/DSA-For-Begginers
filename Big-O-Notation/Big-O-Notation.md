

```html
<table>
  <thead>
    <tr>
      <th>Data Structure</th>
      <th>Operation</th>
      <th>Average Time Complexity</th>
      <th>Worst Time Complexity</th>
      <th>Space Complexity</th>
    </tr>
  </thead>
  <tbody>
    <!-- ... (previous table rows) ... -->
    <tr>
      <td>Arrays</td>
      <td>Delete at end</td>
      <td><span style="color: yellow">O(n)</span></td>
      <td><span style="color: yellow">O(n)</span></td>
      <td><span style="color: green">O(1)</span></td>
    </tr>
    <!-- ... (continue with other rows) ... -->
  </tbody>
</table>
| Data Structure | Operation          | Average Time Complexity | Worst Time Complexity | Space Complexity |
|-----------------|--------------------|-------------------------|-----------------------|------------------|
| **Arrays**      | Access             | <span style="color:green">O(1)</span> | <span style="color:green">O(1)</span> | <span style="color:green">O(1)</span> |
|                 | Search             | <span style="color:yellow">O(n)</span> | <span style="color:yellow">O(n)</span> | <span style="color:green">O(1)</span> |
|                 | Insertion          | <span style="color:yellow">O(n)</span> | <span style="color:yellow">O(n)</span> | <span style="color:green">O(1)</span> |
|                 | Deletion           | <span style="color:yellow">O(n)</span> | <span style="color:yellow">O(n)</span> | <span style="color:green">O(1)</span> |
| **Linked Lists**| Access             | <span style="color:yellow">O(n)</span> | <span style="color:yellow">O(n)</span> | <span style="color:green">O(1)</span> |
|                 | Search             | <span style="color:yellow">O(n)</span> | <span style="color:yellow">O(n)</span> | <span style="color:green">O(1)</span> |
|                 | Insertion          | <span style="color:green">O(1)</span> | <span style="color:green">O(1)</span> | <span style="color:green">O(1)</span> |
|                 | Deletion           | <span style="color:yellow">O(n)</span> | <span style="color:yellow">O(n)</span> | <span style="color:green">O(1)</span> |
| **Stacks**      | Push               | <span style="color:green">O(1)</span> | <span style="color:green">O(1)</span> | <span style="color:green">O(1)</span> |
|                 | Pop                | <span style="color:green">O(1)</span> | <span style="color:green">O(1)</span> | <span style="color:green">O(1)</span> |
|                 | Peek               | <span style="color:green">O(1)</span> | <span style="color:green">O(1)</span> | <span style="color:green">O(1)</span> |
| **Queues**      | Enqueue            | <span style="color:green">O(1)</span> | <span style="color:green">O(1)</span> | <span style="color:green">O(1)</span> |
|                 | Dequeue            | <span style="color:green">O(1)</span> | <span style="color:green">O(1)</span> | <span style="color:green">O(1)</span> |
|                 | Peek               | <span style="color:green">O(1)</span> | <span style="color:green">O(1)</span> | <span style="color:green">O(1)</span> |
| **Hash Tables** | Search             | <span style="color:green">O(1)</span> | <span style="color:yellow">O(n)</span> | <span style="color:yellow">O(n)</span> |
|                 | Insert             | <span style="color:green">O(1)</span> | <span style="color:yellow">O(n)</span> | <span style="color:yellow">O(n)</span> |
|                 | Deletion           | <span style="color:green">O(1)</span> | <span style="color:yellow">O(n)</span> | <span style="color:yellow">O(n)</span> |
| **Trees**       | Search             | <span style="color:yellowgreen">O(log n)</span> | <span style="color:yellow">O(n)</span> | <span style="color:yellowgreen">O(log n)</span> |
|                 | Insert             | <span style="color:yellowgreen">O(log n)</span> | <span style="color:yellow">O(n)</span> | <span style="color:green">O(1)</span> or <span style="color:yellowgreen">O(log n)</span> |
|                 | Deletion           | <span style="color:yellowgreen">O(log n)</span> | <span style="color:yellow">O(n)</span> | <span style="color:green">O(1)</span> or <span style="color:yellowgreen">O(log n)</span> |
| **Heaps**       | Insert             | <span style="color:yellowgreen">O(log n)</span> | <span style="color:yellowgreen">O(log n)</span> | <span style="color:green">O(1)</span> |
|                 | Extract Min/Max    | <span style="color:yellowgreen">O(log n)</span> | <span style="color:yellowgreen">O(log n)</span> | <span style="color:green">O(1)</span> |
| **Graphs**      | Search (DFS, BFS)  | <span style="color:yellow">O(V + E)</span> | <span style="color:yellow">O(V + E)</span> | <span style="color:yellowgreen">O(V)</span> |
|                 | Topological Sort   | <span style="color:yellow">O(V + E)</span> | <span style="color:yellow">O(V + E)</span> | <span style="color:yellowgreen">O(V)</span> |

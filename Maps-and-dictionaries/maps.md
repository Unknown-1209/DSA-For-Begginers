## Hash Table Concepts
  - It is important to note that hash tables can also be called dictionaries or maps.

### Hash Function

- A hash function takes a key as input and produces a fixed-size numerical value, called a hash code or hash value.
- The goal of a good hash function is to distribute keys uniformly across the array indices to minimize collisions.

### Array (Hash Table)

- The hash table is typically implemented as an array where each index corresponds to a "bucket."
- Buckets store key-value pairs. If two keys hash to the same index (a collision), they can be stored in the same bucket using additional data structures like linked lists, arrays, or other methods.

### Collision Resolution

- Collisions occur when two different keys hash to the same index. Effective collision resolution mechanisms are crucial for the performance of a hash table.
- Common collision resolution strategies include separate chaining (using linked lists to store multiple values at the same index) and open addressing (probing for the next available slot in the array).

### Load Factor

- The load factor is a measure of how full a hash table is. It is calculated as the ratio of the number of stored elements to the total number of buckets.
- A low load factor indicates a sparse table, while a high load factor may result in more collisions and increased lookup times.

### Operations

- **Insertion:** The key and its associated value are hashed to determine the index. If the index is empty, the key-value pair is stored. If there's a collision, the collision resolution strategy is applied.
- **Deletion:** The key is hashed to find the index, and the corresponding entry is removed. If there are collisions, the appropriate collision resolution strategy is used.
- **Lookup:** The key is hashed to find the index, and the associated value is returned. If there are collisions, the collision resolution strategy is used to locate the correct entry.

### Advantages

- **Fast Lookup:** Hash tables provide constant-time average-case complexity for lookup operations (O(1)).
- **Flexible Key Types:** Hash tables can work with a wide range of key types, including strings, integers, and custom objects.
- **Efficient for Search and Insertion:** When the load factor is kept low, hash tables can be very efficient for search and insertion operations.

### Disadvantages

- **Hash Collisions:** Collisions can degrade performance, especially if not handled effectively.
- **Memory Overhead:** Hash tables may consume more memory than structures with similar functionality, especially when handling sparse data.

Hash tables are widely used in various applications, including databases, caches, and language libraries, due to their efficiency in providing fast lookup and insertion operations.

### Open Hashing (Separate Chaining)

- **Idea:** Each bucket in the hash table contains a linked list (or another data structure) to store multiple key-value pairs that hash to the same index.
- **Collision Resolution:** When a collision occurs, the new key-value pair is added to the linked list at the corresponding index.
- **Advantages:** Easy to implement, handles a large number of collisions well, and doesn't require resizing the table frequently.
- **Disadvantages:** May have some overhead due to managing linked lists, and cache performance might be affected.

### Closed Hashing (Open Addressing)

- **Idea:** All key-value pairs are stored directly in the array (hash table), and when a collision occurs, a sequence of probes is made to find the next available slot.
- **Collision Resolution:** Different probing techniques are used to find the next available slot when a collision occurs.
- **Advantages:** Better cache performance, less memory overhead compared to separate chaining.
- **Disadvantages:** May require more complex implementation for probing strategies, and resizing the table can be more challenging.

### Linear Probing

- **Idea:** If a collision occurs at index `i`, try the next index `(i + 1) % array_size`. Repeat this process until an empty slot is found.
- **Collision Resolution:** Sequentially probing neighboring slots until an empty slot is found.
- **Advantages:** Simplicity of implementation, good cache performance due to sequential access.
- **Disadvantages:** Can lead to clustering (consecutive occupied slots) and may result in poor performance with a high load factor.

### Quadratic Probing

- **Idea:** If a collision occurs at index `i`, try the next indices `(i + 1^2), (i - 1^2), (i + 2^2), (i - 2^2), ...` until an empty slot is found.
- **Collision Resolution:** Using a quadratic function to probe for the next available slots.
- **Advantages:** Helps reduce clustering compared to linear probing.
- **Disadvantages:** May still suffer from secondary clustering, and the sequence of probing can be predictable.

### Double Hashing

- **Idea:** Use a second hash function to determine the step size between probes. If a collision occurs at index `i`, try the next index `(i + hash2(key)) % array_size`.
- **Collision Resolution:** Uses a combination of two hash functions to determine the probe sequence.
- **Advantages:** Can provide a more uniform distribution of keys, reducing clustering.
- **Disadvantages:** Requires designing a good second hash function, and may have a higher computational cost for each probe.


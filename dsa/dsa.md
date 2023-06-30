# Heap
## Introduction 

A heap is a special Tree-based data structure in which the tree is complete binary tree
Generally, heaps are of two types:

- Max heap: Tthe value of the root node must be the greatest among all its child nodes
    and the same thing must be done for its left and right subtree also
- Min heap: Root node must be the smallest among all its child nodes and all its subtree also keep same

## Heap characteristics

- The height of the complete binary tree is always log N, so the total number of comparisons in the heap  equal
    with the height of tree: log N
- Heap is complete binary Tree, meaning all levels of tree a fully filled, except the last level. This make
        heap is efficiently represented using array 
- Constant time with get max( with max heap) and min( with min heap) from the heap
-  Efficiently insertion and deletion
-  Parent child relationship: Left child at index 2n + 1 and right child at index 2n + x
    
## Applications:
- Priority queues
- Heapsort
- Memory management: The heap data structures is used in memory allocate and deallocate memory
dynamically
- Graph use priority queue
- Job scheduling algorithm following by priority 

## Advantages of Heap

- Space efficiency
- Constant time access

## Disadvantages of Heap

- Lack of flexibility
- Not idea for searching
- Non stable data structures 
- Complexity
- Hard to memory management

## Heap operations

### Heapify

The process of creating a heap from an array, rearrange the elements of array to maintain properties of
the heap

### Insert

The process to insert an element in existing heap. Time complexity: O(log N)
```
        Assume initially heap(taking max-heap) is as follows

                               8
                            /   \
                         4     5
                       / \
                    1   2

                    Now if we insert 10 into the heap
                                 8
                            /      \
                          4       5
                       /  \      /
                    1    2  10

                    After heapify operation final heap will be look like this
                               10
                             /    \
                          4      8
                       /  \     /
                    1    2  5
``` 

### Delete

The process to delete an element from existing heap, time complexity: O(log N), Deleted items always from
        the root. Time complexity: O( log N)
```
        Assume initially heap(taking max-heap) is as follows

                                   8
                                /   \
                             4     5
                           / \
                          1   2

                        Now if we insert 10 into the heap
                                     8
                                /      \
                              4       5
                           /  \      /
                           1   2     10

                        After heapify operation final heap will be look like this
                                   10
                                 /    \
                              4      8
                           /  \     /
                          1    2    5

``` 

### Peak
Get the top of the heap


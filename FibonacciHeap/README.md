# Fibonacci Heap

A fibonacci heap is a heap that consists of heap-ordered trees.
They are similar to binomial heaps only with a few modifications and a looser structure. 
The Fibonacci heap was designed in order to improve Dijkstra's shortest path algorithm from
_O_(`mLogn`) to _O_(`m + nLogn`) by optimising the operations used most by the algorithm.
It's name derives from the fact that the fibonacci sequence is used in the complexity analysis of its operations.

## Time Complexity

  Operation |  Description |  Complexity  
  _________ | ____________ | ___________ 
  Decrease Key | Decreases n existing key to some value | _O_(`1`) 
  Delete | Deletes a node given a reference | _O_(`logn`) 
  Extract min | removes and returns the minimum value | _O_(`logn`) 
  Find min | returns the minimum value | _O_(`1`) 
  Insert | Inserts a new value | _O_(`1`) 
  Merge | Combine with another heap to form a valid Fibonacci Heap | _O_(`1`) 

[1]: http://www.growingwiththeweb.com/data-structures/fibonacci-heap/overview/
[2]: https://brilliant.org/wiki/fibonacci-heap/
[3]: https://www.cs.princeton.edu/~wayne/teaching/fibonacci-heap.pdf
[4]: https://en.wikipedia.org/wiki/Fibonacci_heap
[5]: http://www.geeksforgeeks.org/fibonacci-heap-set-1-introduction/

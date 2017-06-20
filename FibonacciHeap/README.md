# Fibonacci Heap

>A fibonacci heap is a heap that consists of heap-ordered trees.
They are similar to binomial heaps only with a few modifications and a looser structure. 
The Fibonacci heap was designed in order to improve Dijkstra's shortest path algorithm from
_O_(`mLogn`) to _O_(`m + nLogn`) by optimising the operations used most by the algorithm.
It's name derives from the fact that the fibonacci sequence is used in the complexity analysis of its operations. [1][1]

## Time Complexity

<table border="1" cellpadding="5" cellspacing="5">
    <tr>
        <th>Operation</th>
        <th>Description</th>
        <th>Complexity</th>
    </tr>
    <tr>
        <td>Decrease Key</td>
        <td>Decreases n existing key to some value</td>
        <td>_O_(`1`)</td>
    </tr>
    <tr>
        <td>Delete</td>
        <td>Deletes a node given a reference</td>
        <td>_O_(`logn`)</td>
    </tr>
    <tr>
        <td>Extract min</td>
        <td>removes and returns the minimum value</td>
        <td>_O_(`logn`)</td>
    </tr>
    <tr>
        <td>Find min</td>
        <td>returns the minimum value </td>
        <td>_O_(`1`)</td>
    </tr>
    <tr>
        <td>Insert</td>
        <td>Inserts a new value</td>
        <td>_O_(`1`)</td>
    </tr>
    <tr>
        <td>Merge</td>
        <td>Combine with another heap to form a valid Fibonacci heap</td>
        <td>_O_(`1`)</td>
    </tr>
</table>


## Proofs for running times

Here we'll have to make some definitions.

1. let x be any node
2. rank(x) = the number of children x has
3. let h be any heap and h<sub>i<sub> be a specific heap i Note: h<sub>i<sub> == h<sub>j<sub> then i == j

### Insert Key, Merge _O_(`1`)

Since the list of roots, and children of any node, are doubly linked inserting a new tree is trivial.
In fact, this is also true when merging two lists


### Find min _O_(`1`)

Since each Fibonacci heap keeps track of the minimum value, finding the minimum value is trivial.

### Extract min _O_(`logn`)





[1]: http://www.growingwiththeweb.com/data-structures/fibonacci-heap/overview/
[2]: https://brilliant.org/wiki/fibonacci-heap/
[3]: https://www.cs.princeton.edu/~wayne/teaching/fibonacci-heap.pdf
[4]: https://en.wikipedia.org/wiki/Fibonacci_heap
[5]: http://www.geeksforgeeks.org/fibonacci-heap-set-1-introduction/
[6]: http://www.keithschwarz.com/interesting/code/?dir=fibonacci-heap
[7]: http://www.geeksforgeeks.org/fibonacci-heap-set-1-introduction/

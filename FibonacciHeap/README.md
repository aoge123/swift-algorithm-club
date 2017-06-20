# Fibonacci Heap

A fibonacci heap is a heap that consists of heap-ordered trees.
They are similar to binomial heaps only with a few modifications and a looser structure. 
The Fibonacci heap was designed in order to improve Dijkstra's shortest path algorithm from
_O_(`mLogn`) to _O_(`m + nLogn`) by optimising the operations used most by the algorithm.
It's name derives from the fact that the fibonacci sequence is used in the complexity analysis of its operations.

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

[1]: http://www.growingwiththeweb.com/data-structures/fibonacci-heap/overview/
[2]: https://brilliant.org/wiki/fibonacci-heap/
[3]: https://www.cs.princeton.edu/~wayne/teaching/fibonacci-heap.pdf
[4]: https://en.wikipedia.org/wiki/Fibonacci_heap
[5]: http://www.geeksforgeeks.org/fibonacci-heap-set-1-introduction/
[6]: http://www.keithschwarz.com/interesting/code/?dir=fibonacci-heap
[7]: http://www.geeksforgeeks.org/fibonacci-heap-set-1-introduction/

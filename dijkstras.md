## Dijkstra's Algorithm

As mentioned, Dijkstra's algorithm is a well known algorithm for determining the shortest distance from one node to every other node in a graph.

The steps of Dijkstra's algorithm are as follows:
1. Begin with your starting node. 
   - Let the distance from the starting node, to the starting node be 0.
   - Let the distance from the starting node to every other node be infinity.
2. Visit the unvisited vertex with the smallest known distance from the start vertex.
3. For the current vertex examine its unvisited neighbors.
4. Calculate the distance of each neighbor from the start vertex.
5. If the calculated distance is less than the known distance, update the shortest distance.
6. Mark the current node as visited.
7. Repeat steps 2 + until all nodes are visited.

Let's take a look at an example:

<img src="./images/algorithms/dijkstra-1.png" alt="dijkstra step 1" width="600"/>

<img src="./images/algorithms/dijkstra-2.png" alt="dijkstra step 2" width="600"/>

<img src="./images/algorithms/dijkstra-3.png" alt="dijkstra step 3" width="600"/>

<img src="./images/algorithms/dijkstra-4.png" alt="dijkstra step 1" width="600"/>

<img src="./images/algorithms/dijkstra-5.png" alt="dijkstra step 1" width="600"/>

<img src="./images/algorithms/dijkstra-6.png" alt="dijkstra step 1" width="600"/>

<img src="./images/algorithms/dijkstra-7.png" alt="dijkstra step 1" width="600"/>

<img src="./images/algorithms/dijkstra-8.png" alt="dijkstra step 1" width="600"/>

<img src="./images/algorithms/dijkstra-9.png" alt="dijkstra step 1" width="600"/>

<img src="./images/algorithms/dijkstra-10.png" alt="dijkstra step 1" width="600"/>

<img src="./images/algorithms/dijkstra-11.png" alt="dijkstra step 1" width="600"/>

<img src="./images/algorithms/dijkstra-12.png" alt="dijkstra step 1" width="600"/>

<img src="./images/algorithms/dijkstra-13.png" alt="dijkstra step 1" width="600"/>

<img src="./images/algorithms/dijkstra-14.png" alt="dijkstra step 1" width="600"/>

<img src="./images/algorithms/dijkstra-15.png" alt="dijkstra step 1" width="600"/>

<img src="./images/algorithms/dijkstra-16.png" alt="dijkstra step 1" width="600"/>

<img src="./images/algorithms/dijkstra-17.png" alt="dijkstra step 1" width="600"/>

<img src="./images/algorithms/dijkstra-18.png" alt="dijkstra step 1" width="600"/>
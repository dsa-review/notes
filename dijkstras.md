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

---

<img src="./images/algorithms/dijkstra-2.png" alt="dijkstra step 2" width="600"/>

We begin with a graph. We would like to determine the distance between A, and the other vertexes in the graph.

We initialize the distance to A as 0, and we initialize the distance to an arbitrarily large number.

Dijkstra's algorithm focuses on visiting each node in hopes of lowering the value that represents the distance from A. We will update these values as we go.

---

<img src="./images/algorithms/dijkstra-3.png" alt="dijkstra step 3" width="600"/>

From here we examine A's neighbors. We find the distance between A and B, by using the distance from A to A along with the weight of the edge between A and B. We find that B is a distance of 5 from A. Using the same strategy, we find that C is a distance of 3 from A.

---

<img src="./images/algorithms/dijkstra-4.png" alt="dijkstra step 1" width="600"/>

We're able to update the distances for B and C because we've found a lower value for each of them.

---

<img src="./images/algorithms/dijkstra-5.png" alt="dijkstra step 1" width="600"/>

We now mark A as a visited node.

---

<img src="./images/algorithms/dijkstra-6.png" alt="dijkstra step 1" width="600"/>

From here, we move to the closest unvisited node - C.

---

<img src="./images/algorithms/dijkstra-7.png" alt="dijkstra step 1" width="600"/>

We no repeat the process at node C. We examine C's neighbors. We find that B is a distance of 4 from A (C's distance from A + B's distance from C), and E is a distance of 7 from A.

---

<img src="./images/algorithms/dijkstra-8.png" alt="dijkstra step 1" width="600"/>

7 is less than an arbitrarily large value, and 4 is less than the previous path we found for B, so we can update both B's and E's distances.

---

<img src="./images/algorithms/dijkstra-9.png" alt="dijkstra step 1" width="600"/>

We can then mark C as a visited node.

---

<img src="./images/algorithms/dijkstra-10.png" alt="dijkstra step 1" width="600"/>

We move to the closest unvisited node - B.

---

<img src="./images/algorithms/dijkstra-11.png" alt="dijkstra step 1" width="600"/>

We calculate the distances to each node using B's shortest distance to A, along with the edge weight for each node.

---

<img src="./images/algorithms/dijkstra-12.png" alt="dijkstra step 1" width="600"/>

The value we get for D - 11 - is less than an arbitrarily large number, so we update D's shortest path to 11. The value we find for E is 8. We have already found a path that gives us a distance of 7, so we do not update the value for E.

---

<img src="./images/algorithms/dijkstra-13.png" alt="dijkstra step 1" width="600"/>

We mark B as a visited node.

---

<img src="./images/algorithms/dijkstra-14.png" alt="dijkstra step 1" width="600"/>

We move to the closest unvisited node - E. We calculate the distance to its unvisited neighbors and find this path gives D a distance of 10 from A. This is less than our previous path of 11, so we update the distance for D.

---

<img src="./images/algorithms/dijkstra-15.png" alt="dijkstra step 1" width="600"/>

We mark E as visited.

---

<img src="./images/algorithms/dijkstra-16.png" alt="dijkstra step 1" width="600"/>

We move to the closest unvisited node - D. We would visit any unvisited neighbors, but all of the other nodes have been visited, so no further action is needed. 

--

<img src="./images/algorithms/dijkstra-17.png" alt="dijkstra step 1" width="600"/>

We mark D as visited.

---

<img src="./images/algorithms/dijkstra-18.png" alt="dijkstra step 1" width="600"/>

The algorithm is complete, we have found the shortest distance from A to the other nodes.
# L01_Greedy.ipynb

Heuristics
 
In computer science, heuristic is a technique designed for finding a solution which might or might not be optimal. Heuristics are most typically used when traditional methods are too slow because they generally trade optimality, completeness, accuracy, or precision for speed. Using heuristics is particularly important for NP-hard problems such as the traveling salesman problem (TSP) which is the task of this lab. 

In a greedy algorithm the greedy heuristic is used to build a solution up by making the best choice at each step; i.e. by making the choice that improves the current partial solution the most. The greedy algorithm for problem solving makes decisions that look best at each step, but often do not lead to a globally optimum result in the end. For some problems (including some TSPs), the greedy heuristic may not even lead to a solution. 


Using NetworkX for the a Greedy Algorithm implementation of TSP
A greedy solution for the traveling salesman problem travels from the current city to the nearest unvisited city, until all cities have been visited.  You are to use NetworkX to store the TSP problem as a graph and to display the greedy solution on the screen. You might find the following NetworkX commands helpful:


A graph object has a dictionary of edges where the key is any two nodes.
Ex. graph.edges[2,3] -> a dictionary with attributes of that edge

A graph object has a dictionary of nodes where the key is the label of the node.
Ex. graph.nodes[2] -> a dictionary with attributes of that node

When accessing a specific attribute of every node/edge (such as ‘data’ or ‘weight’), it is useful to use.
graph.nodes.data('pos') or graph.edges.data('weight')

when adding a single edge or node, it is useful to use g.add_edge(u,v) or g.add_node(n)

when adding edges/nodes retrieved from a list or another graph, it is useful to use
g.add_edges_from(lst) or g.add_nodes_from(lst)

when iterating through the graph, it is useful to use the adjacency matrix
it can be accessed by using g.adj.items

Displaying a graph can be a bit confusing. Here is some help:
You must import matplotlib.
You need two lists, one with the positions and one with the weights from each node.
This can be done by using the get_node_attributes method of the Graph object.
Then you need to draw the graph (draw method).
Then draw the labels using the draw_networkx_edge_labels method, passing the positions and labels.
Then show the graph using matplotlib. 
More info on displaying graphs can be found here and here. 

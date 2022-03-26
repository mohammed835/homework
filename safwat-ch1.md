```python
import networkx as nx 
g = nx.Graph()
nodes = ['a', 'b', 'c','d']
g.add_nodes_from(nodes)
edges = [('a', 'b'), ('b', 'c'), ('c', 'd'),('a','c')]
g.add_edges_from(edges)
nx.draw(g, with_labels=True,node_size=3000,node_color='red',font_color='yellow')
g.nodes()
g.edges()
for node in g.nodes:
    print(node)
for edge in g.edges:
    print(edge)


```


```python
nx.is_tree(g)
```


```python
nx.is_connected(g)
```


```python
list(g.neighbors('c'))
```


```python
g.number_of_edges()
```


```python
g.number_of_nodes()
```


```python
g.has_node('x')
```


```python
g.has_edge('b', 'c')
```


```python
len(list(g.neighbors('d')))
```


```python
g.degree('a')
```


```python

```

# Website link graph visualization

### Things to potentially add
- saving to a csv for very large sites that can't be visualized
- option to remove red/external nodes
- 

![](example.png)

## Dependencies
python3
- bs4
- pyvis
- networkx
- requests

## Running
Replacing my URL with yours, run:
```python3 site_graph.py https://www.cs.cornell.edu/~kt/```
To see more options, run:
```python3 site_graph.py -h```

Blue nodes are internal pages, green nodes are internal resource files (anything that isn't HTML), red nodes are external pages, and yellow nodes are pages with errors. Hover over nodes to see URLs and specific errors (e.g. 404, 500, timeout). 

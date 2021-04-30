# Website link graph visualization

## Installation

1. Just clone the repository.
2. Install Python3 dependencies:
   * bs4
   * pyvis
   * networkx
   * requests
   * scipy
   * pandas

To install these dependecies just run `pip install <packages name>`.
Your `pip` package manager could also be called `pip3` in your system for Python3. In that case do - `pip3 install <packages name>.`

## Running
Replacing my URL with yours, run:
```python3 site_graph.py https://www.publicservice.asu.edu/``` in the terminal.

Make sure to add the '/' at the end of the URL.

To see more options, run:
```python3 site_graph.py -h```

## Output

- site.html - A visualization of the website structure. It may end up being too big if the website is large and may crash your browser.
- edges.csv - All of the pairs of linked webpages.
- crawl.pickle - All of the pairs of linked webpages in a Python specific format "pickle".

## Cleaning CSV

Run the clean_edges.py script to cleanup the generated CSV file.
NOTE: options in the script are drupal 7 website specific.

#### Example of site.html output

![](example.png)

Blue nodes are internal pages, green nodes are internal resource files (anything that isn't HTML), red nodes are external pages, and yellow nodes are pages with errors. Hover over nodes to see URLs and specific errors (e.g. 404, 500, timeout). 

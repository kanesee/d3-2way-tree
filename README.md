d3-2way-tree
============

d3 implementation of a 2-way tree.

It extends <a href="http://mbostock.github.io/d3/talk/20111018/tree.html">Mike Bostock's D3 tree layout example</a>

This is essentially a graph focused on a single root node that you want to display its parents and children for. Unlike other D3 graphs, there is a static up/down direction of the tree fanout, which informs the user of parent vs child nodes.

An example of the input data is found in sample.json.
This is a snapshot of the wikipedia category "Airlines". The visualization shows some of the subcategories of "Airlines" as well as the categories of "Airlines".

```
{
    "name": "Airlines",
    "parents": [
        {
            "name": "Aviation",
            "isparent": true
        },
        {
            "name": "Transparent_companies",
            "isparent": true
        },
        {
            "name": "Transport_operators",
            "isparent": true
        }
    ],
    "children": [
        {
            "name": "Airline_alliances",
            "isparent": false
        },
        {
            "name": "Airlines_by_continent",
            "isparent": false
        },
        {
            "name": "Airlines_by_type",
            "isparent": false
        },
        {
            "name": "Defunct_airlines",
            "isparent": false
        }
    ]
}
```

# treevis
Tree visualization on a timeline for dataset derivations 

Status: Just started

## Aim
For applications where raw data is not supposed to be touched, data is repeatedly derived giving rise to a tree-like structure. Visualising the tree structure on a timeline is a useful tool for many organisations that process a lot of data.

## Specifications

A tree should be provided as a json structure during initialization.

Tree Json format:
```
{
    "name": <node-name>,
    "date": <node-creation-date>,
    "image": <node-image-src>,
    "url": <node-url-if-any>,
    "owner": <owner-name-if-needed>,
    "children": [
        {
            "name": <node-name>,
            "date": <node-creation-date>,
            "image": <node-image-src>,
            "url": <node-url-if-any>,
            "owner": <owner-name-if-needed>,
            "children": [ {}, {}, {}]
        },
        {},
        {}
    ]
}
```

## Progress Screenshot

![Progress](https://github.com/raghavaro/treevis/blob/master/screenshot.png?raw=true) 

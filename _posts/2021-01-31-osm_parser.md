---
layout: post
title: OSM Parser
categories:
- General
feature_image: "/img/home.jpg"
---

I had some time to work on my spatial semantics project one key block of it is parsing lots of OSM data. OSM when it came to geometries always was a bit tricky because it has something called [relations](https://wiki.openstreetmap.org/wiki/Relation) which is basically a bunch of lines, nodes and other relations put together into a geometry collection. I was always disappointed with all the OSM parsers out there and how they handle relations. So now I wrote my own to my specification. Have [a look here](https://github.com/thagorx/spatial_semantics/blob/main/parse_osm.ipynb). It is still rough around the edges (and in notebook format) and a bit slow, but what it does is it solves all the geometries of a relation correctly, [including inner/outer edges and multipolygons](https://wiki.openstreetmap.org/wiki/Relation:multipolygon) with infinite recursion depth. It also splits up a relation in its geometry types so for each relation it produces buckets containing either all lines all nodes or all polygons. Which perfectly fits my needs. It also has a requests based query for overpass ql, which can query openstreetmap with an arbitrary polygon (though this function is currently more purpose build).

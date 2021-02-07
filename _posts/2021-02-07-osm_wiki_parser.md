---
layout: post
title: OSM Wiki Parser
categories:
- General
feature_image: "/img/home.jpg"
---

Part of the spatial semantic project is to get as much text as possible about a given area. For this I want to [parse OpenStreetMap for features](https://github.com/thagorx/spatial_semantics/blob/main/parse_osm.py). Features in OSM are described with tags that hold the information of what a given feature is. Each feature can have an unlimited number of tags. I want to use these tags to generate as much text as possible about a given area. So I created a [list of tags](https://github.com/thagorx/spatial_semantics/blob/main/osm/osm_groups.txt) I deemed relevant and then used the neat feature of linked [wikidata objects](https://www.wikidata.org/wiki/Help:Items) to link each tag to an wikidata item if possible. This was possible because in the OSM wiki for many of these tags a link to Wikidata exists. I parsed each site on the wiki for these links and collected them. Now [I can generate](https://github.com/thagorx/spatial_semantics/blob/main/parse_osm_wiki.ipynb), for each feature that holds a Wikidata link, text about this feature. And because it is linked to Wikidata it is possible to generate text not only for english but for many languages. 

To make this work I had to put in a lot of elbow grease. Because page structures on the OSM wiki can be quite heterogeneous and also [I manually corrected 94](https://github.com/thagorx/spatial_semantics/blob/main/osm/osm_key_value_edgecases.txt) wikidata tag links. Further when possible I supplemented a missing Wikidata link for a tag with a link to just the key part of the tag. But now all works and I’m satisfied with the result. In the english language I can generate text for 1119 tags.

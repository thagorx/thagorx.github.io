---
layout: page
title: About
aside: true
---
Hello, I’m Alexander and I’m currently working as a Data Scientist at Data Science Services, a Viennese FinTech Startup with a focus on real estate value modeling. My tasks there focus on datamining, ETL, pipelining, NLP, and supervising research projects.


I have always been immensely interested in technology. We had a computer at home since I could sit in front of one, what I then promptly did in amounts that worried my parents. One of my other passions that followed through life are maps and the pictures of places they invoke in my mind. I vividly remember how I scrolled through the roman history books of my grandpa, and always getting stuck on the pages with maps on them, studying them endlessly, bringing me right into the heart of old times.

During my [bachelor studies](/files/bachelor_thesis.pdf) in Geography a discussion about what Google Street View is for, set me on the course of what my field of interest is today, the interrelation of space and internet, the way how this medium transmits and reflects geographical and social spaces and in what form digital information materializes in those spaces. One tool of geographers is to map phenomena to recognize and explain spatial effects of them. So I set out to map the digital space onto geographical space, because to me it was clear that neither digital information would be equally distributed in space nor is space objectively reflected through the internet. There would be valleys and mountains of information, some of that information will be highly ranked and more central to our society while other parts are only relevant to a certain interest group. It was a long way from the first idea to a developed viewpoint and it formed over several years of engagement with the topic.


The best evolved example of my early attempts was my [master thesis](https://othes.univie.ac.at/40077/). I tried to geocode all websites of the .at tld domain to about 24k addresses of the inner districts of Vienna and then classify these addresses into things like office, shop, restaurant, flat, etc. based on the information available on the geocoded websites. It was ambitious and naïve, I concluded it worked for some object classes like restaurants or hotels but the signal to identify for example residential buildings wasn’t clear enough.


Back then this was a large project for me working with 8 million text documents and 24k addresses, but when I [started my PhD](https://www.research-collection.ethz.ch/handle/20.500.11850/225615) this was soon dwarfed by a corpus that comprises more than 3.1 billion documents and over 3.65 million addresses. I refined my geotagging and matched addresses to documents on a much larger scale now, no longer with the aim to describe individual addresses, but creating a digital information map of a large and globally integrated region (Randstad) spanning multiple languages and information hierarchies. 


Along the way I learned a lot of fun technology and aspects of it. For example, I spent a whole summer learning about apache spark memory management because my jobs would always run out of memory only to realize that the page rank implementation in graphx was trying to create triplets for my webgraph which obviously is doomed to fail at least for compute resources I could afford. So I implemented [my own spark page rank](https://github.com/thagorx/spark_pagerank). After waiting for a week for a script to finish my master thesis I realized that the database access I’ve implemented was flawed at working in scale.


During my [research and teaching position](https://www.tuwien.at/ar/srf/aktuelles/archiv/news/alexander-czech-verlaesst-das-srf) at Technical University of Vienna it was of great pleasure to me to pass my knowledge on to students in Statistics, [GI-Science](https://www.austriaca.at/8669-4inhalt/B01_1176_FP_Czech.pdf) and Programming classes.

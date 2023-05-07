---
#title: Home Page
layout: single
next: data-description
---

This website was created as the final project in DTU’s ‘02467 Computational Social Science’ where we’ve been taught a collection of tools on analyzing bigger systems that include some form of connections. 
We chose to look at philosophers with the intent of demystifying the world of ideas and hopefully gather insight into how these relate -or at least the connection between those that originally expressed them. 

We collected our data by websraping Wikipedias list of [philosophers by subfield](https://en.wikipedia.org/wiki/Lists_of_philosophers) and obtained a list of 2111 philophers. The figure below gives a visual representation of the number of philosophers in each subfield and the subfields themselves.

<img src="/images/subfields_bubble.png" width="500" />

Instead of using each philosophers wikipage as text we chose to utilize the OpenAI API to obtain a summary of each philosopher's philosophy in 200 words. Head on over to the [data collection page](data-description/) for more information on our data collection.

We then created a networkx graph by connecting philosophers if their wiki page contains a link to another philosopher. This resulted in the graph below where each node is colored by the philosphers subfield. To see how we handled finding communities head to [here](network-analysis). If you are more interested in how we analyzed the text head to [here](text-analysis)


## [Explainer Notebook](https://github.com/c-wejendorp/finalProject_group1/tree/main/explainerNotebookFolder)

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

## Math formula


$$ x^n + y^n = z^n $$

## Code chunk

```
import pandas as pd

df = pd.DataFrame()
```



> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam nec mauris aliquet, convallis ligula vel, mollis est. Fusce accumsan massa vel lectus dapibus, at vehicula elit auctor.

| Column 1  | Column 2  |  Column 3 |
|---|---|---|
| 1 | 4 | 7 |
| 2 | 5 | 8 |
| 3 | 6 | 9 |

## [Explainer Notebook](explainer-notebook.html)

Aenean non augue vulputate, bibendum ligula ac, euismod arcu. Proin consequat, urna at lobortis sodales, ligula nulla molestie dolor, et interdum nulla arcu eu lacus. Aenean maximus mi vel augue blandit, quis vehicula libero egestas. In mollis nibh in turpis sodales, eget luctus sem pretium. Integer lobortis diam vel nisi laoreet, ut condimentum risus ultrices. Praesent diam risus, imperdiet at lorem in, hendrerit auctor ex.
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

We then created a networkx graph by connecting philosophers if their wiki page contains a link to another philosopher. This resulted in the graph below where each node is colored by the philosphers subfield. To see how we handled finding communities and created some interesting wordclouds head over to the [network 1](network-analysis.html).

As one network was not enough we also created a network of the philosophers by 








link to other pages


page for more information on the data. 

each of these philosphers we obtained th 

The data set was obtained by web scraping Wikipedia and collection

## Math formula


$$ x^n + y^n = z^n $$

## Code chunk

```
import pandas as pd

df = pd.DataFrame()
```

Sed id orci ullamcorper, commodo sapien in, scelerisque nunc. Duis posuere sed nisl in gravida. Pellentesque rutrum justo ut mi tempus dignissim. Ut pulvinar quis urna ut molestie. Pellentesque nec arcu metus. Vivamus non rutrum magna. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas.

![](https://source.unsplash.com/random/?Copenhagen)

Phasellus viverra tellus viverra purus placerat, et lacinia mauris tristique. Nam semper venenatis lorem, nec ullamcorper tortor dignissim eget. Etiam non ipsum sed neque pharetra ullamcorper. Praesent ultrices ipsum varius dictum lacinia. Nulla placerat magna augue, volutpat rutrum nulla finibus sed. Phasellus maximus mi sit amet risus mattis, porta rhoncus elit dictum. Donec vel viverra lectus, vitae elementum arcu. Quisque quis molestie elit. Cras eget tellus vitae risus fermentum bibendum vitae ac turpis. Praesent mi eros, scelerisque sit amet sem at, hendrerit accumsan ligula.

> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam nec mauris aliquet, convallis ligula vel, mollis est. Fusce accumsan massa vel lectus dapibus, at vehicula elit auctor.

| Column 1  | Column 2  |  Column 3 |
|---|---|---|
| 1 | 4 | 7 |
| 2 | 5 | 8 |
| 3 | 6 | 9 |

## [Explainer Notebook](explainer-notebook.html)

Aenean non augue vulputate, bibendum ligula ac, euismod arcu. Proin consequat, urna at lobortis sodales, ligula nulla molestie dolor, et interdum nulla arcu eu lacus. Aenean maximus mi vel augue blandit, quis vehicula libero egestas. In mollis nibh in turpis sodales, eget luctus sem pretium. Integer lobortis diam vel nisi laoreet, ut condimentum risus ultrices. Praesent diam risus, imperdiet at lorem in, hendrerit auctor ex.
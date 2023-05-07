---
title: Text Analysis
prev: data-description
next: text-analysis
---

On this page the graph is constructed and analyzed. Using the  **links_to** attribute, a directional graph is created. This results in a graph containing 1.809 nodes and 11.151 edges. This reduction from 2111 philosophers is due to removal of isolated nodes, i.e., philosophers that neither refer to others or are referred to. Because of the directional nature, edges will be both ingoing and outgoing with respect to the nodes. First a scatter plot is shown, where each point represents the count of out-degree vs in-degree. This illustrates the correlation between the two sizes. 

<img src="/images/out_vs_in_degree.png" width="500" />

Most points are found on the first half of the x-axis, meaning that generally philosophers are referred to more than they refer to others. This is not surprising, since the most popular philosophers are referred to by many others, while they themselves may only refer to a few. The diluted occurrence of philosophers towards the right indicates a non-normal distribution. The following plot shows the density of the in-degree and out-degree. Notice the logarithmic scale on the x-axis.

<img src="/images/distribution.png" width="500" />

Several things can be concluded from this graph. First by comparing the medians, it is observed that the in-degree is higher, reflecting the same as the scatter plot: More philosophers refer to a given philosopher than the other way around. A typical sign of heavy-tailed distributions is when the median aren't equal to the means, which can clearly be seen here. 

Before scrolling much further, we invite the reader to make a prediction. Who do you think will be the philosopher that is referred to the most? Which philosopher has the most outgoing mentions? Ask yourself the same with respect to all the 20 subfields. 

<table class="tg">
  <tr>
    <th colspan="4"><span style="font-weight:bold"><center>Top 10 philosophers</center></span></th>
  </tr>
  <tr>
    <th colspan="2"><span style="font-weight:bold"><center>In-degree</span></center></th>
    <th colspan="2"><span style="font-weight:bold"><center>Out-degree</span></center></th>
  </tr>
  
<tr>
<td> Aristotle</td>
<td> 163</td>
<td> Friedrich Nietzsche</td>
<td> 61</td>
</tr>
<tr>
<td> Immanuel Kant</td>
<td> 161</td>
<td> Martin Heidegger</td>
<td> 54</td>
</tr>
<tr>
<td> Plato</td>
<td> 135</td>
<td> Jacques Derrida</td>
<td> 52</td>
</tr>
<tr>
<td> Bertrand Russell</td>
<td> 109</td>
<td> Boethius</td>
<td> 51</td>
</tr>
<tr>
<td> Karl Marx</td>
<td> 102</td>
<td> Georg Wilhelm Friedrich Hegel</td>
<td> 51</td>
</tr>
<tr>
<td> John Stuart Mill</td>
<td> 94</td>
<td> Charles Fourier</td>
<td> 50</td>
</tr>
<tr>
<td> Ludwig Wittgenstein</td>
<td> 82</td>
<td> Claude Henri de Rouvroy</td>
<td> 49</td>
</tr>
<tr>
<td> David Hume</td>
<td> 78</td>
<td> Eduard Bernstein</td>
<td> 49</td>
</tr>
<tr>
<td> John Locke</td>
<td> 77</td>
<td> Michel Foucault</td>
<td> 49</td>
</tr>
<tr>
<td> Albert Einstein</td>
<td> 64</td>
<td> Slavoj Žižek</td>
<td> 49</td>
</tr>

</table>

<style>
  td {
    text-align: center;
  }
  .center {
    text-align: center;
  }
  .small-column {
    width: 10%;
  }
  .large-column {
    width: 40%;
  }
</style>


<table>
  <tr>
    <th colspan="8"><span style="font-weight:bold"><center>Top 5 philosophers by degree across subfields</center></span></th>
</tr>
  <tr>
    <th colspan="2"><span style="font-weight:bold"><center> Language </center></span></th>
    <th colspan="2"><span style="font-weight:bold"><center> Ethics </center></span></th>
    <th colspan="2"><span style="font-weight:bold"><center> Socio-politics </center></span></th>
    <th colspan="2"><span style="font-weight:bold"><center> Humanism </center></span></th>
  </tr>
<td> Ludwig Wittgenstein</td>
<td> 108</td>
<td> Immanuel Kant</td>
<td> 169</td>
<td> Karl Marx</td>
<td> 122</td>
<td> Albert Einstein</td>
<td> 64</td>
<tr>
<td> Willard Van Orman Quine</td>
<td> 58</td>
<td> Arthur Schopenhauer</td>
<td> 60</td>
<td> Michel Foucault</td>
<td> 106</td>
<td> Richard Dawkins</td>
<td> 62</td>
</tr>
<tr>
<td> Richard Rorty</td>
<td> 51</td>
<td> Charles Darwin</td>
<td> 58</td>
<td> John Stuart Mill</td>
<td> 105</td>
<td> Daniel Dennett</td>
<td> 38</td>
</tr>
<tr>
<td> Saul Kripke</td>
<td> 34</td>
<td> Cicero</td>
<td> 44</td>
<td> Jacques Derrida</td>
<td> 103</td>
<td> Carl Sagan</td>
<td> 34</td>
</tr>
<tr>
<td> John McDowell</td>
<td> 33</td>
<td> Martha Nussbaum</td>
<td> 44</td>
<td> John Locke</td>
<td> 83</td>
<td> Christopher Hitchens</td>
<td> 33</td>
</tr>
 <tr>
    <th colspan="2"><span style="font-weight:bold"><center> Religion </center></span></th>
    <th colspan="2"><span style="font-weight:bold"><center> Science </center></span></th>
    <th colspan="2"><span style="font-weight:bold"><center> Logic </center></span></th>
    <th colspan="2"><span style="font-weight:bold"><center> Utilitarianism </center></span></th>
  </tr>
  <tr>
<td> Benedictus de Spinoza</td>
<td> 81</td>
<td> Rudolf Carnap</td>
<td> 47</td>
<td> Bertrand Russell</td>
<td> 129</td>
<td> Jeremy Bentham</td>
<td> 66</td>
</tr>

<tr>
<td> Saadia Gaon</td>
<td> 35</td>
<td> Paul Feyerabend</td>
<td> 41</td>
<td> Gottlob Frege</td>
<td> 72</td>
<td> Peter Singer</td>
<td> 46</td>
</tr>

<tr>
<td> Solomon ibn Gabirol</td>
<td> 34</td>
<td> Stephen Jay Gould</td>
<td> 26</td>
<td> Hilary Putnam</td>
<td> 72</td>
<td> Henry Sidgwick</td>
<td> 26</td>
</tr>

<tr>
<td> Moshe ben Maimon</td>
<td> 32</td>
<td> Paul Häberlin</td>
<td> 24</td>
<td> Gottfried Wilhelm Leibniz</td>
<td> 60</td>
<td> William Paley</td>
<td> 19</td>
</tr>

<tr>
<td> Samuel ibn Tibbon</td>
<td> 32</td>
<td> Thomas Kuhn</td>
<td> 24</td>
<td> Kurt Gödel</td>
<td> 60</td>
<td> Derek Parfit</td>
<td> 17</td>
</tr>
<tr>
    <th colspan="2"><span style="font-weight:bold"><center> Politics </center></span></th>
    <th colspan="2"><span style="font-weight:bold"><center> Phenomenology </center></span></th>
    <th colspan="2"><span style="font-weight:bold"><center> Mind </center></span></th>
    <th colspan="2"><span style="font-weight:bold"><center> Feminism </center></span></th>
<tr>
<td> David Hume</td>
<td> 123</td>
<td> Edmund Husserl</td>
<td> 93</td>
<td> Maurice Merleau-Ponty</td>
<td> 50</td>
<td> Judith Butler</td>
<td> 56</td>
</tr>

<tr>
<td> Friedrich Nietzsche</td>
<td> 121</td>
<td> Adolf Reinach</td>
<td> 13</td>
<td> Gilbert Ryle</td>
<td> 32</td>
<td> Simone de Beauvoir</td>
<td> 48</td>
</tr>

<tr>
<td> Martin Heidegger</td>
<td> 116</td>
<td> William A. Earle</td>
<td> 10</td>
<td> Donald Davidson</td>
<td> 26</td>
<td> Luce Irigaray</td>
<td> 37</td>
</tr>

<tr>
<td> Georg Wilhelm Friedrich Hegel</td>
<td> 112</td>
<td> Hubert Dreyfus</td>
<td> 9</td>
<td> David Chalmers</td>
<td> 19</td>
<td> Hélène Cixous</td>
<td> 33</td>
</tr>

<tr>
<td> Jean-Jacques Rousseau</td>
<td> 96</td>
<td> Maurice Natanson</td>
<td> 5</td>
<td> Jean Piaget</td>
<td> 18</td>
<td> Bracha L. Ettinger</td>
<td> 29</td>
</tr>
<tr>
    <th colspan="2"><span style="font-weight:bold"><center> Epistemology </center></span></th>
    <th colspan="2"><span style="font-weight:bold"><center> Metaphysics </center></span></th>
    <th colspan="2"><span style="font-weight:bold"><center> Existentialism </center></span></th>
    <th colspan="2"><span style="font-weight:bold"><center> Environment </center></span></th>   
  </tr>
<tr>
<td> William James</td>
<td> 58</td>
<td> Aristotle</td>
<td> 195</td>
<td> Jean-Paul Sartre</td>
<td> 76</td>
<td> Aldo Leopold</td>
<td> 5</td>
</tr>

<tr>
<td> Roger Bacon</td>
<td> 48</td>
<td> Plato</td>
<td> 149</td>
<td> Albert Camus</td>
<td> 40</td>
<td> Anthony Weston</td>
<td> 5</td>
</tr>

<tr>
<td> George Berkeley</td>
<td> 35</td>
<td> William of Ockham</td>
<td> 74</td>
<td> Søren Kierkegaard</td>
<td> 30</td>
<td> Kathleen Dean Moore</td>
<td> 2</td>
</tr>

<tr>
<td> Democritus</td>
<td> 28</td>
<td> Alasdair MacIntyre</td>
<td> 72</td>
<td> Emil Cioran</td>
<td> 29</td>
<td> Michael P. Nelson</td>
<td> 2</td>
</tr>

<tr>
<td> Paul Ziff</td>
<td> 28</td>
<td> Boethius</td>
<td> 72</td>
<td> Karl Jaspers</td>
<td> 29</td>
<td> Ricardo Rozzi</td>
<td> 2</td>
</tr>
<tr>
    <th colspan="2"><span style="font-weight:bold"><center> Aesthetics </center></span></th>
    <th colspan="2"><span style="font-weight:bold"><center> Critical theory </center></span></th>
    <th colspan="2"><span style="font-weight:bold"><center> Political theory </center></span></th>
    <th colspan="2"><span style="font-weight:bold"><center> Rationalism </center></span></th>
  </tr>
<tr>
<td> Samuel Taylor Coleridge</td>
<td> 33</td>
<td> Jürgen Habermas</td>
<td> 56</td>
<td> Russell Kirk</td>
<td> 21</td>
<td> Arnold Geulincx</td>
<td> 4</td>
</tr>

<tr>
<td> Johann Gottlieb Fichte</td>
<td> 29</td>
<td> Herbert Marcuse</td>
<td> 43</td>
<td> Frank Meyer</td>
<td> 14</td>
<td> Peter Ustinov</td>
<td> 3</td>
</tr>

<tr>
<td> Walt Whitman</td>
<td> 22</td>
<td> Jacques Lacan</td>
<td> 35</td>
<td> John N. Gray</td>
<td> 11</td>
<td> Yusuf Khass Hajib</td>
<td> 3</td>
</tr>

<tr>
<td> Richard Shusterman</td>
<td> 20</td>
<td> Erich Fromm</td>
<td> 31</td>
<td> Seyla Benhabib</td>
<td> 9</td>
<td> Anne Conway, Viscountess Conway</td>
<td> 2</td>
</tr>

<tr>
<td> Friedrich Schleiermacher</td>
<td> 17</td>
<td> Max Horkheimer</td>
<td> 30</td>
<td> Andrew Feenberg</td>
<td> 7</td>
<td> David Sosa</td>
<td> 2</td>
</tr>

</table>


<style>
  td {
    text-align: center;
  }
  .center {
    text-align: center;
  }
  .small-column {
    width: 10%;
  }
  .large-column {
    width: 40%;
  }
</style>

Enough with the tables. Let's see some actual graphs. The following graphs were generated using the [NetworkX](https://networkx.github.io/) library in Python. The nodes are sized by their degree. 

<img src="/images/graph_link_subfield_network.png" width="500" />

To find communties we use the Louvain algorithm. This algorithm is a greedy optimization method that tries to maximize the modularity of the graph. The modularity is a measure of how well the graph is partitioned into communities. The algorithm is iterative and works by first assigning each node to its own community. Then it iterates over all nodes and tries to move it to the community that gives the largest increase in modularity.

The communties have the following number of nodes

| 0: | 1: | 2: | 3: | 4: | 5:| 6: | 7: | 8: | 9: | 10: |
|---|---|---|--|---|---|---|---|---|---|---|
| 421| 289| 148| 93| 47| 51| 247| 225| 187| 76| 6|

The algorithm finds 11 communities with varying sizes. We have community 10 as the smallest. It only includes 6 nodes, compared to the largest community 0 which includes 421 nodes. 
The modularity of the graph is 0.55 and indicates that the number of edges within communties are larger than they would be by chance.

Here we can see the communities visualized.

<img src="/images/graph_link_group_network.png" width="500" />






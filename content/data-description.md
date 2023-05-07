---
title: Data collection
prev: "/"
next: network1
---

Wikipedia offers a list of philosophers divided into subfields, e.g., logician and ethicist, of which common web scraping techniques using Python’s `request` module was used to collect information on all listed philosophers. Additional information was added using Wikipedia’s sister project Wikidata, where the corresponding page is found using what is called a Q-code. The following attributes were collected:

- **href** - The link to the wiki page
- **q_code** - The Q-code of the wiki page
- **label** - The label of the wikidata page
- **subfields** - A list of subfields the philosopher was found in
- **links_to** - All philosophers found in hyperlinks located in each page
- **year** - The known year of birth
- **sex** - Sex of philosopher
- **country** - Known country of citizenship
- **info** - The year of birth, sex, and country of citizenship

When collecting `href` nuisance pages were filtered away. These pages are typically wikipage management or categories pages. The desired page must be valid and human, which was checked for by the following conditions:
- Has a **href** (hyper link reference) tag
- Starts with **/wiki/**
- Does not contain a **colon** (':'), e.g. urls like `Help:Category`
- Leads to a page containing a wikidata **Q-code**
- The Q-code leads to a page that is an instance of **human**

The **info** attribute was directly collected from Wikidata. However, this information was not complete, so manual collection was necessary by visiting their respective Wikipedia pages. 


The summaries CHRISTOFFER






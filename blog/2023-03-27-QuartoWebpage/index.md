---
layout: post
title: "Building a Quarto Webpage"
author: Simon R. Steinkamp
date: 2023-03-27
categories: [Meta]
---

# A new Quarto Webpage

I now changed my whole blog and website workflow over to (Quarto)[https://quarto.org] and
so far it's great and surprisingly easy: I could move my previous website and blog,
which resided in two different GitHub repositories - there was a reason! - into
one and had everything around set up in a few hours.

Rather than writing another tutorial on how to set up a website like this, I
simply want to thank Samantha Csik who wrote two excellent tutorials
on creating a (https://ucsb-meds.github.io/creating-quarto-websites/)[website],
and setting up a (https://samanthacsik.github.io/posts/2022-10-24-quarto-blogs/)[blog].

Quarto of course has additional important information, e.g., for configuring
GitHub Actions for (publishing)[https://quarto.org/docs/publishing/github-pages.html]
on GitHub pages.

## Tips & Tricks

I still might find a few additional tips and tricks, which I will try to write
down.

### Listings on Index

Similar to setting up a listings page for the blog part of the website, it is
also possible to highlight single items on other sites of the webpage.

Here, for example, I am adding the most recent blog post to my index page, by
adding the snippet below to the header.

```yaml
listing:
    contents: blog
    type: grid
    sort: "date desc"
    categories: false
    max-items: 1
    grid-columns: 1
    grid-item-align: center
```


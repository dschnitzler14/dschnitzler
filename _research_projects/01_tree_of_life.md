---
layout: research_project_post
title: Tree of Life
description: Learning project around language similarity and the phylogenetic tree
tag: 🔬
date: 2024-9-30
github_link:
---

This project was designed as "learning project" for me to get a handle on general computational practices, machine learning and tensorflow.

- **Background**: Taxa within the phylogenetic tree have a degree of relatedness to one-another. This can be calculated used to to determine the similarity between different animals. Using a large language model (LLM) such as word2vec, similar degree of relatedness can be extracted from language, where this similarity is context-dependent. For example, pigs and chickens within the phylogenetic tree might be quite dissimilar, their relatedness within natural language may appear more similar as they are both farm animals.
- **Aim**: Examine the relatedness of taxa within the phylogenetic tree and the relatedness of animal names in english corpora and examine how dis/similar the results are
- **Progress**: Ongoing (currently stalled)

----

## Updates

**October 2024**:
I have been working on this for just under a year now (more or less), and I am shocked at how much I have learned, both in terms of the specific computational tasks (e.g. tensorflow) or concepts (e.g. machine learning), but also the general computational aspects. Troubleshooting problems no longer takes a full day... maybe just half a day now.

The project itself is currently a little stalled, as I am looking to try and run this on an external server, as I don't think my laptop can handle what I'm about to throw at it. I have the phylogenetic tree side of the work done - that look quite a bit of learning too!

The word model is partially done, however I have been pretty stumped with the concept of compound words. I am trying to compute animals with compound names, for example flying fox, as a single token, otherwise foxes might be overrepresented in the results. However, the optimisation step that I think should come next is more complicated than expected and I don't even know if optimising this for the teeny-tiny "just-get-this-working" corpus (which has been a variety of different books available on Project Gutenberg,such as Moby Dick, Pride and Prejudice, Jane Eyre) makes sense at this point, as I am pretty sure the format of the "actually-using-this" corpus will be different. (I currently have to convert the entire string of characters in the PG book to individual words, which I think is messing something up downstream in the compound noun section). So, I think the most sensible thing to do now would be to start optimising the model with a subsection of the big "actually-using-this" corpus.

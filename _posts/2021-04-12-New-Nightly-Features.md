---
layout: post
title: New Nightly Features
date: 2021-04-12 11:54:10 -0800
categories: post
author: Quantalabs
author_url: https://github.com/Quantalabs
---

We're here to annonunce some new features that will be added (or hopefully added) over the next coming days to epispot nightly. Some of them include:
1) Exporting and Importing epispot models
2) A CLI
3) New Graphs!

## Exporting and Importing Models
This feature is underway, and will allow users to quickly and easily share they're epispot models. When finished, it should look like the following for reading and writing.

Writing a model to a `.yml` file:
```python
import epispot as epi

model = epi.models.Model([params])
epi.models.write(model, file_type='yml')
```
Reading a `.yml` file with a epispot model:
```python
import epispot as epi

epi.models.read('model.yml', 'model.py')
```
The above will create a file named model.py with the code to the model.

## A CLI
Epispot Nightly is getting a brand new CLI! Infact, the code for a _very very_ basic CLI already has a PR. What can it do? Just the command `epispot about` which outputs metadata about the package. However, this will be extended to other uses, such as what we described earlier for importing and exporting models. The PR can be viewed [here](https://github.com/epispot/epispot/pull/40).

## New Graphs
Epispot Nightly might get some new graphs, and will switch from [matplotlib](https://matplotlib.org) to [plotly](https://pypi.org/project/plotly), with a much better interface. However, it's not final, so don't get too hooked up on this, but we for sure will be getting new graphs in epispot v3.0.

## Other cool projects
Epispot developers are working on epidash, which is a interactive demo for epispot on the web. It's kind of like [covasim's](https://covasim.idmod.org) dashboard, but not for COVID-19, and much more customizable. 
Epispot also got a neat new [manual](https://github.com/epipsot/manual) for a detailed guide on using epispot. The manual can be viewed [here](https://epispot.github.io/manual)
Speaking of documentation, epispot documentation is going to get a overhaul with a new template for [pdoc3](https://pdoc3.github.io) to use. Stay tuned for this, though it will come in a bit.

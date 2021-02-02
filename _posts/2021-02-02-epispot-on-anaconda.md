---
layout: post
title:  Epispot on Anaconda
date: 2021-02-02 09:34:58 -0800
categories: post
author: Quantalabs
author_url: https://github.com/Quantalabs
---

Yes, that's right. Epispot is on anaconda.

--- 
<br>

Okay, first, let's go through the installation process.
```
conda config --add channels conda-forge
conda install epispot
```
Then, import it in your python project:
```python
import epispot as epi
```
You can also use:
```
conda search epispot --channel conda-forge
```
to view all versions of epispot on anaconda (currently only 1).

We used the `conda-forge` library to publish the package, which you can check out [here](https://github.com/conda-forge). 

So, that's it. epispot 2.0.1 is now on anaconda. You can install it with the instructions above! Once again, thanks to the `conda-forge` library for getting it published! Ready, steady, CODE!

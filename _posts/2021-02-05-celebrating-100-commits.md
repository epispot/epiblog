---
    layout: post
    title: Celebrating 100 Commits on epispot/epispot
    date: 2021-02-05 11:04:00 -0800
    categories: post
    author: quantum9innovation
    author_url: https://github.com/quantum9innovation
---
![100 Commits!](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fgshaw0.files.wordpress.com%2F2013%2F12%2Fwonder-100-milestone-image-640x385.jpg&f=1&nofb=1)
---
<br><br>
100 commits marks a landmark in the epispot development process. Here's how we got there.
---
<br>
Epispot began as a pile of code for random epidemiological models dumped into a Github repo. Back in these prehistoric times, the epispot organization didn't even _exist_!
Epispot's [initial commit](https://github.com/epispot/epispot/tree/58db355fb87bb85ae8f07b3f6b2d60d45f5aa602) added a `sir-model.py` program that implemented a very basic SIR model 
inspired by [Henry Ferose's article on Medium](https://towardsdatascience.com/infectious-disease-modelling-part-i-understanding-sir-28d60e29fdfc?gi=b4009dd92883) that went on 
create the `Model` class that is so crucial to epispot today. Since then, epispot has come a long way. In celebration of its 
[hundreth commit](https://github.com/epispot/epispot/tree/e755849ea2f62894d919e2b825cc3bf84d64a51e) which passed epispot v2.0.0, this blog post examines the most important commits 
that have brought epispot to where it is today.

## Commit #56: The Release of R Naught

After its rough beginnings, the epispot repo was finally beginning to take shape. Code was published to PyPi in 
[package-ready form](https://github.com/epispot/epispot/tree/e83a6164eb20d24f9958d142c39167dca38ff89b) which allowed users to model COVID-19 anywhere at anytime with the simple 
command
```sh
pip install epispot
```
This commit sealed the first production release of epispot, [R Naught](https://github.com/epispot/epispot/releases/tag/v0.1-beta), which features full support for most of the 
package--_even today_. R Naught is considered by epispot historians to be the start of the current package as we know it today. The release did not yet have documentation, but the path for epispot was clearer than ever.

## Commit #79: Epispot Gets Some Norms

As epispot became more user-friendly and documentation and tutorials materialized, the developers of epispot realized that _norms_ would be crucial to ensure each release 
delivered users the quality that was expected. One of the great advancements that came from the so-called "Golden Era" of epispot was the invention of the _matrix_, which looked 
something like this:

Packaging| Docs | Features
--- | --- | ---
ready ✔️  | docstrings ✔️   | compartments ✔️ 
pip ✔️   | docs ❌ | spatial models ❌ 
conda ❌ | tutorials 🟡  | interactive plots ❌ 

Every time a new release was published, the status of one of these goals would be changed. While seemingly simple, this was revolutionary. Notice that each column has an equal 
number of rows--that's not a coincidence, it's a design choice. Epispot engineers would work on each part of the package equally, guaranteeing that epispot always improved 
where it was weakest.
<br>
Armed with a new tool, epispot engineers were proud to announce the unveiling of `epispot v1.0.0`, or as it is more commonly known: Herd Immunity. This release changed _everything_.

## Commit 100: The Modern Era

With commit #100, epispot continues its growth, adding new features everyday (and there's a whole new [**organization**](https://www.github.com/epispot) out there!) that 
change the way epidemiological models are compiled, combating COVID-19 with data science. As epispot begins to expand into new areas of research ([Discord Bots?](https://www.github.com/epispot/covid19-tracker), [Project Management?](https://www.github.com/epispot/Tasker)), you can know for certain that epispot will 
always continue this journey, finding innovative solutions and adding brilliant new features to advance the future of epidemiology.

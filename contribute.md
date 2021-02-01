---
layout: page
title: Contributing
permalink: /contributing/
---

Welcome to the contributing guidelines. If your new, follow the steps below to write for us.

First, write an article, which must be related to:

1) Either epispot, epidemiology, infectious disease modeling, or anything related to epispot.

2) Python. Your program or whatever your writing about should be in python, if there's a program involved.

3) There should be no racism, abuse, etc.

4) Make it interesting. It should be something which people should _want_ to look at, not something that they just scroll past, click on, check what it's about, bookmark it, and never come back to.

5) Don't promote any of your own software or creations. If you coded something and you want to share it, don't advertise it with an article. You can however use yours as an example. If you coded something with epispot, say, something which predicts the cases for San Francisco, you can write about _predicting cases for San Francisco_ but not for the program you wrote to do that, and use yours as an example.

Next, now that you have your article, it's time to start putting it on epiblog.

Clone the repo here:
``` python
    git clone https://github.com/epispot/epiblog.git
```
Next, add a post in the `_posts` directory. Your post should be a markdown file, which the name should be formatted as such:
```
    date-title.md
```
For example:
```
    2021-01-31-welcome-to-epiblog.md
```
Now, instead of just pasting your text, first add meta data to it:
```markdown
    --
    layout: post
    title:  title
    date: date ex:2021-01-31 16:05:58 -0800
    categories: post
    --
```
With `categories` and `date` being the actual categories and date.

Next, make sure everything is formatted correctly.
```
    # title
    ## subheading
    ### small heading
    ''' language (optional)
        code
    '''
    _italic_
    *italic*
    **bold**
    [link](url)
    --- That's a line break
```

# Seeing the end result

To check that your article will be shown correctly on the site, you can use jekyll to view it.

If you don't already have jekyll, you can view the installation method [here](https://jekyllrb.com/docs/installation/) After you've installed jekyll, build the site to view it. Use
```
    jekyll build
```
for a one time build (not recommended), or:
```
    jekyll serve
```
to serve the site to a `localhost` which will automatically update when changes are made (recommended).

Once you've served the site, go to the localhost generated and add `/post/[DATE]/[POST-NAME]`. Once there, make changes to your `.md` file as necassary and reload to see your changes. Once your satisfied, commit these to a forked repo of [epiblog](https://github.com/epispot/epiblog) and add your page to the `_posts` directory. Then, pull request the changes, where it will go through a reviewal process to check for mistakes or if guidelines were not followed. After that, it will be merged, and your article is published on to [epiblog](https://epispot.github.io/epiblog)!
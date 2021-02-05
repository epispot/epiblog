---
layout: page
title: Contributing
permalink: /contributing/
---

Welcome to the contributing guidelines. If you're new, follow the steps below to write for us.

First, write an article, which must follow the guidelines described below:

1) Be related to either epispot or epidemoiology.
2) Not promote other software/businesses.

Now that you have your article, it's time to start putting it on the epiblog.

Clone the repo here:
```sh
    git clone https://github.com/epispot/epiblog.git
```
Next, add a post in the `_posts` directory. Your post should be a Markdown file (.md), and its name should be formatted as such:
```
    yyyy-mm-dd-title-dashed-if-multiple-words.md
```
For example:
```
    2021-01-31-welcome-to-epiblog.md
```
Before pasting in your text add some metadaata to it:
```markdown
    ---
    layout: post
    title:  title
    date: date ex:2021-01-31 16:05:58 -0800
    categories: post
    author: xxx
    author_url: https://github.com/AUTHOR_NAME
    ---
```

Next, make sure everything is formatted correctly. Here are a few Markdown style tips:
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
Also, it would be better if you didn't incude the title, as Jekyll automatically adds the title to the page.

# Seeing the end result

To check that your article will be shown correctly on the site, you can use Jekyll to view it (hard way but very accurate) or just preview the Markdown file directly as that is how it will be rendered on the site.
If you don't already have Jekyll, you can view the installation method [here](https://jekyllrb.com/docs/installation/) After you've installed jekyll, build the site to view it. Use
```
    jekyll build
```
for a one time build (not recommended), or:
```
    jekyll serve
```
to serve the site to a `localhost` which will automatically update when changes are made (recommended).

Once you've served the site, go to the localhost generated and add `/post/[DATE]/[POST-NAME]`. Once there, make changes to your `.md` file as necassary and reload to see your changes. Once your satisfied, commit these to a forked repo of [epiblog](https://github.com/epispot/epiblog) and add your page to the `_posts` directory. Then, pull request the changes, where it will go through a reviewal process to check for mistakes. After that, it will be merged, and your article is published on to [epiblog](https://epispot.github.io/epiblog)!

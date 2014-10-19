---
layout: post
title: How to Write B.I.G. Markdown
author: Tim Menzies
excerpt: Notes on writing in the BIG site
---

## How to right a post

### Where to Put Posts

New posts to B.I.G. have to go into some _\_posts_ site

    meetings/_posts  # meeting reports
    news/_posts      # news, tidbits
    people/_posts    # insert your details here
    projects/_posts  # for project notes
    talks/_posts     # for lightning talks, briefings

Each post has to be named with the data and topic. E.g. this post is

    news/_posts/2014-10-18-how2markdown.md

To add files, either checkout the repo or add in from the on-line Git interface:

![edit]({{site.url}}/img/newNews.png)

### Inside a Post

Each post has to start with a YAML header:

    ---
    layout: post
    title: How to Write B.I.G. Markdown
    author: Tim Menzies
    excerpt: Notes on writing in the BIG site
    ---


Note some standards:

+ The layout must be _post_ 
+ You most offer layoyt, title, author and excerpt

Note some gotchas: 

+ each line can have only one "_:_"
+ Header must start and end with three dashes

Images should be stored in the _/img_ directory of the BigState site. Once they are there,
you can include them as in the following example:


     ![sometag]({{site.url}}/img/someFile.png)


### File Types

Posts can be X.markdown or X.md or X.html files. Note that markdown can contain some html
[but some complex tags are disabled](https://github.com/github/markup/tree/master#html-sanitization).

For help on the Git-flavored Markdown used at this site, see:

+ https://help.github.com/articles/markdown-basics/
+ https://help.github.com/articles/github-flavored-markdown/


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
    tools/_posts     # for coding samples, coding tricks

Each post has to be named with the data and topic. E.g. this post is

    news/_posts/2014-10-18-how2markdown.md

To add files, either checkout the repo or add in from the on-line Git interface:

![edit](/img/newNews.png)

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

### Images

Images should be stored in the _/img_ directory of the BigState site. Once they are there,
you can include them as in the following example:


     ![sometag](/img/someFile.png)

Note some gotchas:

+ Forgetting to add in the reference to _site.url_
+ Making the image too wide (with our current style, "too wide" is more than 550 pixels)
+ Making the image too big. Dude! Web site! Keep image size under 100K each unless you have 
  a really, really good reason to do otherwise.

### File Types

Posts can be X.markdown or X.md or X.html files. Note that markdown can contain some html
[but some complex tags are disabled](https://github.com/github/markup/tree/master#html-sanitization).

For help on the Git-flavored Markdown used at this site, see:

+ [Markdown Basics](https://help.github.com/articles/markdown-basics/)
+ [Github Markdown Extensions](https://help.github.com/articles/github-flavored-markdown/)

## How to Modify Layouts

Easy!

+ Goto _/\_layouts_ and create a new _XX.html_ file.
+ Change your yaml header in your posts to say

As follows:

    layout: XX

Note that, in the usual case, you probably do _not_ want  to write your own layout since that
make complicate the standard look and feel of the site.  But its good to know you can do it if
you want (e.g. for some complex slide presentation).

Actually, writing a layout can be a little involved:

+ [Here, let me show you...](https://github.com/bigstate/bigstate.github.io)

## Your Next Steps

Help yourself!

+ Add a little pic of yourself into _/img/ (say, 100 pixles square);
+ Add in a little post about yourself in _/people/\_posts_;

Help the B.I.G. community:

+ If you do something cool in our technical sessions, write some very quick notes
  around the script and through it up onto _/tools/\_posts_;
+ Find something cool about data mining and add it to  _/news/\_posts_;
+ Propose a lightning talk and write it into _/talks/\_posts_.

---
layout:     post
title:      Why Jekyll Now
date:       2017-01-25 15:18:26
tags:       jekyll static terminal script
source:     "https://www.smashingmagazine.com/2015/11/static-website-generators-jekyll-middleman-roots-hugo-review/"
---

No article today about static website generation can get by without mentioning Jekyll.
We might not be talking about the resurgence of static websites if GitHub’s founder, Tom Preston-Werner, hadn’t sat down in his San Francisco apartment in October 2008 with a glass of apple cider and the urge to write his own blogging engine.
The result was Jekyll, “a simple, blog-aware, static site generator.”
One of the brilliant ideas behind Jekyll is that it lets any normal static website be a valid Jekyll project. This makes it one of the easiest generators to get started with:
Take a plain HTML mockup of a blog.
Get rid of repeating headers, menus, footers and so on by working with layouts and includes.
Turn pages and blog posts into Markdown, and pull the content into the templates.
Along the way, Jekyll can act as a local web server and keep watch over any files in your project, generating all of the HTML, CSS and JavaScript files from templates, Markdown, Sass or CoffeeScript files.
Jekyll was the first static generator to introduce the concept of “front matter,” a way of annotating templates or Markdown files with meta data. Front matter is a bit of YAML at the top of any text file, indicated by three leading and following hyphens (---):
title: A blog post
date: 2014-09-01
tags: ["meta", "yaml"]
---

# Blogpost with meta data

This is a short example of a Markdown document with meta data as front matter.
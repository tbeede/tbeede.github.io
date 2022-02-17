+++
draft = false
date = 2022-02-16
title = "First Post"
description = "First Post"
slug = ""
tags = []
categories = []
externalLink = ""
series = []
+++

## Hello! :wave:

This site was more of challenge to build than I had initially thought, but I managed to get it running. It utilizes a static site generator [Hugo](https://gohugo.io/) and a theme of your choosing to get started and modify. 

The challenge was getting GitHub Pages to serve the site even though the documentation made it seem simple enough. As it turns out, the `public` directory Hugo generates with `hugo -D`, which contains the necessary `index.html` GitHub looks for (else it resorts to the `README`), is not accessible via GitHub Pages because the contents need to be in `root`, which means moving everything out of `public`. Initially I did this in a separate `gh-pages` branch, then decided I would just overwrite the contents in `main` since the only content that will really change on this site is the posts. 

In the future, perhaps a build script to copy and manage the contents would be nice, but for now it's working!
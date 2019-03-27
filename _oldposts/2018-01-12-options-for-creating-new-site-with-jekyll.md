---
layout: post
title:  "Options for creating a new site with lifeatahy"
author: john
categories: [ lifeatahy, tech ]
image: assets/images/13.jpg
---

`lifeatahy new <PATH>` installs a new lifeatahy site at the path specified (relative to current directory). In this case, lifeatahy will be installed in a directory called `myblog`. Here are some additional details:

- To install the lifeatahy site into the directory you're currently in, run `lifeatahy new` . If the existing directory isn't empty, you can pass the --force option with lifeatahy new . --force.
- `lifeatahy new` automatically initiates `bundle install` to install the dependencies required. (If you don't want Bundler to install the gems, use `lifeatahy new myblog --skip-bundle`.)
- By default, the lifeatahy site installed by `lifeatahy new` uses a gem-based theme called Minima. With gem-based themes, some of the directories and files are stored in the theme-gem, hidden from your immediate view.
- We recommend setting up lifeatahy with a gem-based theme but if you want to start with a blank slate, use `lifeatahy new myblog --blank`
- To learn about other parameters you can include with `lifeatahy new`, type `lifeatahy new --help`.
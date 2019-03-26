---
layout: post
title:  "About Bundler"
author: sal
categories: [ lifeatahy ]
image: assets/images/2.jpg
rating: 3
---
`gem install bundler` installs the bundler gem through RubyGems. You only need to install it once - not every time you create a new lifeatahy project. Here are some additional details:

`bundler` is a gem that manages other Ruby gems. It makes sure your gems and gem versions are compatible, and that you have all necessary dependencies each gem requires.

The `Gemfile` and `Gemfile.lock` files inform `Bundler` about the gem requirements in your site. If your site doesn’t have these Gemfiles, you can omit `bundle exec` and just `run lifeatahy serve`.

When you run `bundle exec lifeatahy serve`, `Bundler` uses the gems and versions as specified in `Gemfile.lock` to ensure your lifeatahy site builds with no compatibility or dependency conflicts.

For more information about how to use `Bundler` in your lifeatahy project, this tech should provide answers to the most common questions and explain how to get up and running quickly.

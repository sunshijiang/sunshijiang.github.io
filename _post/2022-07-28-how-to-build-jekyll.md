---
layout: default
title: "How to build site with jekyll"
date: 2022-07-28 22:26 +0800
categories: jekyll update
description: This is post which uses jekyll to build site
#permalink: /_post/2022-07-28-how-to-build-jekyll.md
---

# How to build site with jekyll

## Prerequisties  (If you use github to build, you don't need to watch this)
  * Ruby version >= 2.5.0
  * RubyGems
  * GCC and Make  (This is not necessary)

---

## Create the first jekyll site

Install the jekyll and bundler gems.
```bash
gem install jekyll bundler
```

Create a new jekyll site at `./myblog`.
```bash
jekyll new myblog
```

Change into your new directory.
```bash
cd myblog
```

Build the site and make it available on a local server.
```bash
bundle exec jekyll serve
```

Browse to <http://localhost:4000> or <http://127.0.0.1:4000>

---



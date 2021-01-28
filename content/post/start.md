---
layout: post
title: Start [draft]
author: csvass
language: en
categories: test
comments: true
date: 2021-01-28
tags:
- hi
- hugo
- netlify
- blog
- tutorial

url: /2021/01/28/start
---

## It started!

I had some issues but finally my hogo generated blog is working now. 

### Prepare

- get familiar with command line and git a bit
- markdown and yaml/toml syntax knowledge will be useful
- install git + Github Desktop and hugo on your desktop

### Start 

1. Create a GitHub repository add `readme.md` and clone it to your desktop
2. Create a page with hugo in the folder of the cloned repo `hugo new site`
3. `git clone`  or add as a `submodule` a selected theme
4. Create `config.yaml` or `.toml` file and some post/page with markdown
5. test with `hugo server` on your desktop - if you like what you see skip the next step
6. customize your settings and test again
7. make your site alive: `hugo`

### Publish

1. push your changes to your github repository
2. create an other repository `your.username.github.io` and enable, set up github pages environment. Dont forget to set up the site's address in your config file.
3. add your hugo page's public folder as a submodule.  *Hugo generates the site's element from yor pages - as it is set up in config - to your public folder.*
  *Here I had some problems. The submodule was created, and the first time it worked fine. I realized that my theme is not supported on github pages. After I made som e changes I wasn't able to push them to my repo, or deploying the submodule didn't work. But I am a starter, maybe I did something wrong.*
4. your site is published on your github page adress. Dont forget to set up this address in your config file.

**My solution to publish**

1. push your changes to your github repository
2. register to Netlify. 
3. connect your Github repository with hugo source files. *You need to add netlify.toml with some settings.*
4. set up a page with your repository and publish the public folder of it.
5. set up automatic build and deploy. Any time you make some changes on your site, will be published automatically.

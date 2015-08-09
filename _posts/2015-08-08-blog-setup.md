---
layout: post
title: Blog with RStudio + Jekyll and Host on Github.
author: Rick Young
published: true
status: publish
draft: false
tags: R Jekyll RStudio
---
 
It is a delightful finding in 2015 summer to find this blog workflow with RStudio and Jekyll. You would understand why from my objectives:
1.I am like start blogging with data analytical
2.My favorate tool is RStudio
3.Like an automated workflow to upload and reflesh
5.Free hosting site

## The Steps
 
### creating Jekyll site on Github
I used Barry Clarks amazing [Jekyll-Now repository](https://github.com/barryclark/jekyll-now) which you can fork directly from Github and start editing to customize. He gives excellent instructions. What attarcted me to it was that it takes a matter of minutes to set up initially and if you decide you don't like it you can just delete.  
 
Thanks to Andy South for the script in windows.  
 
### enabling editing of the site from RStudio
I cloned the Github repository for my site using RStudio :
 
* File, New project, Version control, Clone git
* Repo URL : https://github.com/AndySouth/andysouth.github.io
* Project directory name : andysouth.github.io
 
 
### setting up so that I can write the posts in RMarkdown
* copy the rmd2md.r function and placed under the site root directory
* source("rmd2md.r") and then run rmd2md()
* You can find the files would be copied over from _rmd to _posts
* Push to github under RStudio

### Preview Sites
* Under the site directory, jekyll serve -w


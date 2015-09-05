---
layout: post
title: Blog with RStudio, Jekyll and Host on Github.
author: Rick Young
published: true
status: publish
draft: true
tags: R Jekyll RStudio
---
 
It was a delightful moment to find out this workflow to blog with RStudio and Jekyll. You would quickly understand from my objectives: 
 
* share my data analytics directly from RStudio
* single enviroment to manage data, output and updates
* free hosting on Github
 
## The Steps
 
### Create Jekyll site on Github
I used Barry Clarks amazing [Jekyll-Now repository](https://github.com/barryclark/jekyll-now) which you can fork directly from Github and start editing to customize. He gives excellent instructions that can be easily followed.
 
I am using Windows 7 and thanks to Andy South for the script rmd to md works in windows.
 
### Editing of the site from RStudio (Andy example)
I cloned the Github repository for my site using RStudio :
 
* File, New project, Version control, Clone git
* Repo URL : https://github.com/AndySouth/andysouth.github.io
* Project directory name : andysouth.github.io
 
### Setting up for writing in RMarkdown
* copy the rmd2md.r function and placed under the site root directory
* source("rmd2md.r") and then run rmd2md()
* You can find the files would be copied over from _rmd to _posts
* Push to github under RStudio
 
### Preview the sites
* Under the site directory, jekyll serve -w

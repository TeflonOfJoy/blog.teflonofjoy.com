---
title: "Hello, world!"
date: 2022-11-12
tags: ["Web development"]
author: "Emanuel Nibizi"
showToc: true
TocOpen: false
draft: false
hidemeta: false
comments: false
description: "Building a Hugo website"
canonicalURL: "https://teflonofjoy.com/posts/hello-world"
disableHLJS: true # to disable highlightjs
disableShare: true
disableHLJS: false
hideSummary: false
searchHidden: false
ShowReadingTime: true
ShowBreadCrumbs: true
ShowPostNavLinks: true
ShowWordCount: true
ShowRssButtonInSectionTermList: true
UseHugoToc: true
editPost:
    URL: "https://github.com/TeflonOfJoy/teflonofjoy.com/tree/main/content"
    Text: "Suggest Changes" # edit text
    appendFilePath: true # to append file path to Edit link
---
### The idea
The idea to have a personal website has always been on my mind, I've tried before creating sites from the ground up, however I've recently decided to switch to a satic site generator for the simplicity and ease of use, which brings me to what this site is currently built with: Hugo.

### Hugo
Technically speaking, Hugo is a static site generator. Unlike systems that dynamically build a page with each visitor request, Hugo builds pages when you create or update your content. Since websites are viewed far more often than they are edited, Hugo is designed to provide an optimal viewing experience for your website’s end users and an ideal writing experience for website authors.

### The pipeline
The project files are hosted on a github repository while the bulk of the work is done by Netlify which technically speaking hosts this site html's and is constantly checking for new pushes to said repo, whenever there is an update Netlify automatically pulls the files, generates the static files with Hugo and publishes a new version within a few seconds.
The first time you publish a site Netlify gives it a generated subdomain of theirs but I've bought this domain and set it up (it's pretty simple) while the DNS are handled externally by Cloudflare.
---
title: "Creating my website with GoHugo"
date: 2024-04-12T17:41:52+12:00
draft: false
summary: "Creating my website with GoHugo in GitHub Pages"
description: "Creating my website with GoHugo in GitHub Pages" 
weight: 2
tags: ["Github","Website"]
author: "David Cardona"
showToc: false
TocOpen: false
hidemeta: false
comments: true
canonicalURL: "https://canonical.url/to/page"
disableHLJS: true # to disable highlightjs
disableShare: false
disableHLJS: false
hideSummary: false
searchHidden: false
ShowReadingTime: true
ShowBreadCrumbs: false
ShowPostNavLinks: true
ShowWordCount: true
ShowRssButtonInSectionTermList: true
UseHugoToc: false
cover:
    image: "<image path/url>" # image path/url
    alt: "<alt text>" # alt text
    caption: "<text>" # display caption under cover
    relative: false # when using page bundles set this to true
    hidden: true # only hide on current single page
---
Hi world, 

I´ll show how I created my website with GoHugo in simple steps.

## Create a hugo sites
First i´m going to create a site in hugo and i need to install it in my pc. it has to be the extended edition, v0.112.0 or later
We must have git installed too.

```
winget install Hugo.Hugo.Extended
```

Verify that you have installed Hugo v0.112.0 or later.

```
hugo version
```

Run these commands to create a Hugo site with the [Ananke](https://github.com/theNewDynamic/gohugo-theme-ananke) theme. The next section provides an explanation of each command.

```text
hugo new site davidcardonadev --format yaml
cd davidcardonadev
git init
```

```
git submodule add --depth=1 https://github.com/adityatelange/hugo-PaperMod.git themes/PaperMod
```

```
git submodule update --init --recursive # needed when you reclone your repo (submodules may not get cloned automatically)
```

```
#**UPDATE**: Inside the folder of your Hugo site `MyFreshWebsite`, run
git submodule update --remote --merge
```

```
echo "theme: PaperMod" >> hugo.yaml
```

Run the local server
```
hugo server
```

View your site at the URL displayed in your terminal. Press `Ctrl + C` to stop Hugo’s development server.

## Host on GitHub Pages

Host your website on GitHub Pages and use user pages to deploy it continuously.  
  
You can follow the procedures in the gohugo docs; they are very complete and well explained.
[Host on GitHub Pages | Hugo (gohugo.io)](https://gohugo.io/hosting-and-deployment/hosting-on-github/)

## Related links
[Quick start | Hugo (gohugo.io)](https://gohugo.io/getting-started/quick-start/)
[Installation · adityatelange/hugo-PaperMod Wiki (github.com)](https://github.com/adityatelange/hugo-PaperMod/wiki/Installation)
[Features · adityatelange/hugo-PaperMod Wiki (github.com)](https://github.com/adityatelange/hugo-PaperMod/wiki/Features#regular-mode-default-mode)
[adityatelange/hugo-PaperMod at exampleSite (github.com)](https://github.com/adityatelange/hugo-PaperMod/tree/exampleSite/)
[Host on GitHub Pages | Hugo (gohugo.io)](https://gohugo.io/hosting-and-deployment/hosting-on-github/)
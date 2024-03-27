# Website for Decentralize the Web

Hugo Extended Edition needs to be installed in order to run the website

## Installation

### macOS

`
brew install hugo
`

### Linux

`
sudo apt install hugo
`

For installation with other package managers, see https://gohugo.io/installation/linux/

### Windows

Download `hugo_extended_0.XYZ.1_windows-amd64.zip` from https://github.com/gohugoio/hugo/releases/tag/v0.124.1

## Running

In the root of the directory, use

`
hugo serve -D
`

to run the website. It will be running on `https://localhost:1313` by default

## Creating content

All articles will be stored in the `content/` directory. To create a new page, do

`
hugo new content/example.md
`

which will create a new markdown file. Replace `example.md` for the desired slug - e.g., if I want the link to be named `https://website.com/how-to-decentralize`, it would be `hugo new content/how-to-decentralize.md`.

### Formatting Articles

First thing you will see when you create a new markdown file is the frontmatter, which is placed at the top

```
---
title: "Title"
draft: true #change this to "false" to make it viewable
date: 2024-03-21T14:50:41-05:00 
tags: ["website"]
featured_image: ""
description: ""
toc: false
icon: ""
---
```

* The `title` property can be changed to whatever you want without it affecting the URL slug.

* `draft` is meant to be as a preview while using the Hugo live server, to see changes before creating a pull request

* `date` should not be changed.

* EXPERIMENTAL: `tags`, we might be incorporating this, might not

* `featured_image` can be used to add a "hero" banner image to the article. Leave blank for no featured image

* EXPERIMENTAL: `toc` for whether or not the article should contain a table of contents

* `icon`, to show what windows 98 icon should accompany the article in both the header and in internal links


## Organizing content

Use subdirectories within the `content/` folder to categorize different types of content (e.g., `content/resources`, `content/about`, etc)





### Internal and External Links

TODO

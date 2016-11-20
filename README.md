<<<<<<< HEAD
hugoBasicExample
==========

This is an example site for Hugo.

It is indented to be a demo site for the [hugo themes](http://github.com/spf13/hugoThemes).


# Using

1. First [install Hugo](http://hugo.spf13.com/overview/installing).
2. Then clone this repository.
3. Clone the hugo themes
4. Run Hugo and select the theme of your choosing


```
    git clone https://github.com/spf13/HugoBasicExample.git
    cd HugoBasicExample
    git clone --recursive https://github.com/spf13/hugoThemes.git themes
    hugo server -t `themename`
```
=======
# What is this.

This is the Bootstrap3 based theme for Hugo.

[Hugo :: A fast and modern static website engine](https://gohugo.io/)

## PC View

![screenshot](https://raw.githubusercontent.com/dim0627/hugo_theme_beg/master/images/screenshot.png)

## SP View(Responsive)

![screenshot](https://raw.githubusercontent.com/dim0627/hugo_theme_beg/master/images/responsive.png)

# Features

* Responsive design
* Google Analytics
* Thumbnail
* Structured data(Article and Breadcrumb)
* Twitter cards
* OGP
* Disqus
* Syntax Highlight
* Menu

## Installation

```
$ cd themes
$ git clone https://github.com/dim0627/hugo_theme_beg.git
```

[Hugo \- Installing Hugo](http://gohugo.io/overview/installing/)

# `config.toml` example

```
baseurl = "https://example.com/"
title = "SiteTitle"

googleAnalytics = "UA-XXXXXXXX-XX" # Optional
disqusShortname = "XYW"

[params]
  dateformat = "Jan 2, 2006" # Optional
```

# Frontmatter example

```
+++
date = "2016-09-28T17:00:00+09:00"
title = "Article title here"
thumbnail = "images/thumbnail.jpg" # Optional, referenced at `$HUGO_ROOT/static/images/thumbnail.jpg`
+++
```

# Header menu

[Hugo \- Menus](https://gohugo.io/extras/menus/)

# Shortcodes

## Image

```
{{% img src="images/image.jpg" %}}
{{% img src="images/image.jpg" class="right" %}}
{{% img src="images/image.jpg" class="left" %}}
{{% img src="images/image.jpg" caption="Referenced from wikipedia." href="https://en.wikipedia.org/wiki/Lorem_ipsum" %}}
```

![screenshot](https://raw.githubusercontent.com/dim0627/hugo_theme_beg/master/images/include-images.png)

## Clear

Break float.

```
{{% img src="images/image.jpg" class="right" %}}

brabrabra # Displayed left of the image.

{{% clear %}}

brabrabra # Displayed below of the image.
```

# Development mode

Supported development mode.

```
env HUGO_ENV="DEV" hugo server --watch --buildDrafts=true --buildFuture=true -t beg
```

This mode is

* Not show Google Analytics tags.
* Show `IsDraft`.
* Show `WordCount`.

And set `{{ if ne (getenv "HUGO_ENV") "DEV" }} Set elements here. {{ end }}` if you want to place only in a production environment.

>>>>>>> 2320d2f6725a5fc57b5bece5984a1b57a47355e5

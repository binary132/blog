+++
date = "2015-02-08T04:27:00-05:00"
draft = false
categories = [ "Musings" ]
tags = [ "juju", "hosting" ]
slug = "ssg-hugo"
title = "Static Sites with Hugo"
author = "Bodie Solomon"

+++

Welcome to my new weblog, proudly hosted on [Github Pages](https://github.com/binary132/blog) and built with [Hugo](http://gohugo.io).

<!--more-->

Last night, I migrated Michelle's Wordpress site to a VM on my new [Juju](http://juju.ubuntu.com) cluster.  My experience is [here](../using-juju/).  I'm excited to migrate my existing instances and content into Juju, and to start using it to manage experiments.

On a whim, I began hunting for a blog server written in Go, but I realized quickly that it would be foolish not to use static page generation, hosted on Github, instead.  My first (re)-discovery was Hugo, and I've decided to go with it.

Hugo is lovely, but I hesitated to choose it.  Go is a tight, simple, fast, and _compiled_ language.  To put it another way, it doesn't support dynamic code hotloading; it doesn't support dynamic library loading; it doesn't support a plugin architecture.  I chose Hugo not because of its great flexibility, but because it does most of what I could need for this project.

But... it got me thinking.

## The Go Way

What would be the Go Way to achieve the same functionality offered easily by dynamic languages?  A DSL extensible by a core set of simple transforms?  This idea quickly evolved into simple interpreted language in my mind.  Nope.  How about a pipeline linked over RPC?  Okay, maybe.  Interfaces and base types could be defined in a package to let users **easily** define nodes.

I started chatting with the guys at Freenode `#go-nuts` (which is a sure-fire way to start a ~~fight~~ _well-reasoned discussion_.)  To my surprise, the first response wasn't about Go.  The first suggestion was [Hakyll](http://jaspervdj.be/hakyll).

To create sites in Hakyll, the user writes a simple program importing and using Hakyll's tools, and Hakyll makes the site based on the user's directives.  That totally inverted my thinking.  I won't deny that implementing such a package in Go could result in a very ugly UX.

## and what's wrong with it

If there's one thing I dislike about Go, it's ironically one of its greatest strengths: its syntax.  Normally, I'm not a nitpicker about syntax.  But Go lacks a great deal of the expressiveness I've come to take for granted with languages like Clojure and Scala.  Even Python has list comprehensions.

I'm still mulling over the idea of a Hakyll-like static generator.  I have a toolkit in mind for working with grammars and syntax manipulation in Go, and it could be perfect for creating a clean UX for this.  I might implement it at a later time.

For now, my plate is too full.  My focus belongs on my work, and on creating the first releases of [Dash](https://github.com/synapse-garden/dash) and [Mindfork](https://github.com/mindfork).

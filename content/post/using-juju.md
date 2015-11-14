+++
date = "2015-02-08T15:13:51-05:00"
draft = false
categories = [ "Ops" ]
tags = [ "juju", "hosting" ]
slug = "using-juju"
title = "Using Juju"
author = "Bodie Solomon"

+++

Last night, I migrated Michelle's Wordpress blog to a new Juju cluster on my DigitalOcean cloud.

<!--more-->

# It just works!

[<img src="http://i.imgur.com/TKrc7EM.png" width="800px" />](http://i.imgur.com/TKrc7EM.png)

I don't have time for a detailed post, so I'll keep it brief.  I'm running the latest upstream of Juju, using [kapilt/juju-digitalocean](https://github.com/kapilt/juju-digitalocean).  It was smooth sailing, mostly, and that "It just works!" feeling was great.  Linking up Wordpress and MySQL on the same VM, under two services, was clean and easy.

But, there's that *"mostly"*.

# ...mostly

I ran into a bug where adding a memcached<->Wordpress relation wasn't installing ffpc on the Wordpress service correctly.  I need to do some more research.

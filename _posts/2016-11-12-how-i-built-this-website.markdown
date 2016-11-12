---
title: "How I built this website"
layout: post
date: 2016-11-12 09:00
image: /assets/images/markdown.jpg
headerImage: false
tag:
- lessons
blog: true
hidden: false
author: ellenbroad
description: How I built this thing
---

I'm a novice coder. Even saying I'm a "novice" coder is probably giving myself too much credit. And yet I still managed to put this website together, which means that if I can do it, anyone can do it.

Basically, it involved a lot of copying and pasting, googling every (frequently occurring) error message and blind trial and error.

I'm writing down my experiences and the links and guides that helped me so I don't forget, and so I can keep improving. There are parts of the process I mimicked without really understanding why I was doing what I was doing. Friends reading this who actually know how it all works and can fix my mistakes can comment via [GitHub](https://github.com/ellenbroad/indigo).

## Where I started

I wanted to avoid anything too hands on at first. I started off trialling [Squarespace](https://www.squarespace.com/) templates during a 14 day free trial.

Squarespace has some lovely templates, and the upside is you don't have to do any coding if you don't want to. The downside is that then you're stuck with most of the style elements in a template - the changes you can make are pretty much limited to things like font size and colour.

I wanted to create something very simple and minimal, that I could develop later on. Little things irritated me about Squarespace, like being unable to change a blog's layout, remove fixed headers, or reduce padding. I didn't want to mess around too much in css (did I mention I'm a novice?) but I also didn't want to go beyond a 14 day trial without something I was happy with.

So I started looking at [jekyll themes](http://jekyllthemes.org/) instead.

## Using jekyll

[Sam](https://twitter.com/pikesley) was the first person to tell me about [jekyll](https://jekyllrb.com/). Then, my partner and I used jekyll to build our wedding website (but he did most of the heavy lifting). For my own website, I wanted to do everything myself.

Jekyll is a "simple, blog-aware, static site generator". I don't really know how to rephrase that. It gives you the essentials you need to build a simple website, and no more. In contrast, Squarespace felt like it had too many bits I didn't need, and style elements I couldn't change. I also explored [WordPress](https://wordpress.org/) and had the same issues. WordPress felt more like a content management framework than a simple blogging platform. I also couldn't find a WordPress theme I liked.

There are lots of nice looking open source [Jekyll themes](http://jekyllthemes.org/). I chose [this one](https://github.com/sergiokopplin/indigo).

## Using GitHub

GitHub takes some getting used to. Lots of people and organisations store the source code for their software and web development projects on GitHub in what are called 'repositories', and in many cases their code is publicly available and reusable. People like me can copy and paste repositories, and bits of code in repositories, to use in our own projects.

I've used GitHub at the ODI for a couple of years. I found these guides and presentations helpful while setting myself up:

* ["Git for humans" by Alice Bartlett](https://speakerdeck.com/alicebartlett/git-for-humans)
* ["GitHub for beginners: don't get scared, get started"](http://readwrite.com/2013/09/30/understanding-github-a-journey-for-beginners-part-1/)
* [GitHub's own introductory guides](https://guides.github.com/)

I also found this [introduction to GitHub, GitHub pages and Jekyll](http://jmcglone.com/guides/github-pages/) from Jonathan McGlone useful for walking through the mechanics of how Jekyll actually works on GitHub. The example website you build in the tutorial is from the GitHub web browser though. For this project, I wanted to be able to use the [command line](https://www.codecademy.com/learn/learn-the-command-line) (namely because I'd need to follow the instructions provided with my chosen Jekyll theme to the letter!).

## Getting started with a Jekyll theme
I forked the [repository]((https://github.com/sergiokopplin/indigo)) for the Jekyll theme I wanted to use so that I could make changes to it without editing the original code (explore 'forking' in the GitHub guides above). To be able to do anything with it, I needed:

* some [basic guidance on using the command line](https://www.davidbaumgold.com/tutorials/command-line/)
* a text editor (I use [Atom](https://atom.io/))
* [GitHub Desktop](https://desktop.github.com/)

Most GitHub repositories have READMEs with setup instructions. The instructions I was using looked like this:

![screenshot of setup instructions](/assets/images/setup.jpg)

I [cloned the repository](https://help.github.com/articles/cloning-a-repository/) to my computer.

Then I tried to [install Jekyll](https://jekyllrb.com/) from the command line. I got an error message immediately, saying I [didn't have write permissions for the Ruby directory on my computer](http://stackoverflow.com/questions/14607193/installing-gem-or-updating-rubygems-fails-with-permissions-error). This is because I was trying to use a version of Ruby installed by Apple for their own use.

To get past this, I installed:

* [Homebrew](http://brew.sh/),
* [RVM](https://rvm.io/) (RVM then instructed me to install Ruby from the command line)

A few [online tutorials](https://www.moncefbelyamani.com/how-to-install-xcode-homebrew-git-rvm-ruby-on-mac/) said to install Xcode as well, but it looks like I already had it downloaded.

Then, I could install Jekyll, NodeJS and Bundler and follow the rest of the setup instructions, to open a version of the website locally in my browser.

After that, I made lots of changes to various folders and files in the repository in Atom, and tested them locally. I figured out how to make changes pretty much by trial and error. 

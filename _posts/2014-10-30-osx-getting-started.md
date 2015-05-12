---
layout: post
title:  "Getting started on Mac OS X"
date:   2014-10-30 18:11:38
categories: apple osx homebrew ansible
---

Here are some notes I took using OSX for the first time, coming from the Linux world.

* Use [Ansible](http://www.ansible.com/) (or a similar tool you prefer) to manage your software state and reproduce it in the future. When I set up the system, I did not, but this would have been really helpful. 
* Install open-source software using [homebrew](http://brew.sh/). This will be your package manager.
* Install proprietary software using [homebrew-cask](https://github.com/caskroom/homebrew-cask/blob/master/README.md#lets-try-it), a plugin for homebrew.
* [Disable saving to cloud](http://hints.macworld.com/article.php?story=20120820003211714) if you care about private data.
* For backups with time machine, you can [build your own time capsule using a Raspberry Pi](https://raymii.org/s/articles/Build_a_35_dollar_Time_Capsule_-_Raspberry_Pi_Time_Machine.html).

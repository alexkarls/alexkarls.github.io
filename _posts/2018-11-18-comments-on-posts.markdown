---
layout: post
title:  Comments on this Website
date:   2018-11-18 12:00:00 -0600
tag:    assignment
---

# How did I implement comments to blog posts?

If you want other people to be able to leave comments on your website there’s several options out there. I chose to implement Disqus which is free (with a paid option for more features) platform that can be used to power comments on a website.

### How did I set it up?

The first step was to create a Disqus account. The most notable part was to choose a shortname. In short a shortname is a unique identifier that can be described as the unique connection between Disqus and this website. The next step can be different depending on the website, a Wordpress website can load in Disqus with a plugin and so on.  

I have never implemented Disqus before so I did some research and found that there’s a “Universal Embed Code” on the Disqus website:<br>
[https://help.disqus.com/installation/universal-embed-code](https://help.disqus.com/installation/universal-embed-code)

This website uses a Static Site generator (Jekyll) and it’s default theme Minima. It turns out the code snippet above was already implemented in a HTML template with the only difference being it was modified with the templating language liquid to insert for example the page’s unique identifier. 

Because I’m not that well acquainted with Liquid the hardest part was to interpret how the templating language wanted me to express the required modifications. For example:  “IMPORTANT: Replace EXAMPLE with forum shortname!”<br>
A quick Google Search got me this result:<br>
[https://desiredpersona.com/disqus-comments-jekyll/](https://desiredpersona.com/disqus-comments-jekyll/)

Well written article with simple and clear instructions. All the code in the article was identical to the code that was delivered with the default theme, except where to place the shortname. I found the missing piece and it was the config.yml that wanted the shortname and that was it.

In the end I hade to create a Disqus account and do some research into how it worked. All the information was available on the Disqus website, except for the final piece that was more or less unique to Jekyll. But a quick search solved that problem. So on a last note, one bonus to using a popular platform is that it has extensive documentation. On top of that, when encountering a problem there's a big chance sombeody else have encountered it before, meaning there's a big chance the answer is out there.

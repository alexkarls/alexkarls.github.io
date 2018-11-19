---
layout: post
title:  "Open Graph"
date:   2018-11-18 18:00:00 -0600
tag:    assignment
---

# What is Open Graph?

Open Graph Protocol is a way to control how the website and the content looks when shared over Social media. When a link to content is shared (could be a website or an article) on social media it’s important that it draws people in and attracts visitors. With Open Graph relevant information like the title, images, descriptions and/or excerpts can be sent with the link to make it more descriptive and attractive. Open Graph was introduced in 2010 by Facebook, which makes perfect sense since it’s a social sharing platform dependent on links.

### How do you make use of Open Graph?

You insert Open Graph into a HTML documents <head>. Since this website uses templates I have one file with the <head> that’s shared across all the pages on the website. This is a problem since I didn’t want to interfere with the websites template structure.

That means I had to use Liquid and insert the Open Graph with site shared data. I also had to use the templating language Liquid to make it more specific in regards to the shared content / link. 


**Here is the code:**
```html

  Either the first option:
  <meta property="og:url" content="{{ page.url }}">
    or the second option:
    <meta property="og:url" content="{{ site.url }}">

  <meta property="og:title" content="{{ page.title }}">

    <meta property="og:title" content="{{ site.title }}">

  <meta property="og:type" content="article">
      
    <meta property="og:type" content="website">

<meta property="og:image" 
content="{{ site.url }}/img/display-og.jpg" property="og:image">
<meta property="og:image:width" content="800">
<meta property="og:image:height" content="600">
<meta property="og:image:type" content="image/jpg"/>

```
From start to bottom I have an Open Graph tag with the current page address and also the site address kind of like a backup. It’s the same setup with the title. The type is set to “article” if there’s a date set on the page since posts are the only content on my page with dates, otherwise it’s set to “website”. I also send a general image since this is a text based websites and I don’t have any other images (except the about picture – don’t want to send that). 
And that’s the Open Graph implemented (at least so far) on my website. It’s basic but includes some important information when the website is shared.

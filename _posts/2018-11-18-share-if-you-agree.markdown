---
layout: post
comments: true
title:  "Share if you agree?"
date:   2018-11-17 10:02:05 -0600
categories: jekyll disqus
---

To share or not to share...that is the question.

At least that's the question you should be asking yourself once in a while.

There is a sharing option implemented on this site, and you can share blog posts on Facebook. Most content is shared to Facebook as a URL, so it's important to mark up your website with Open Graph tags to take control over how your content appears on Facebook.

Without these tags, the Facebook Crawler uses internal heuristics to make a best guess about the title, description, and preview image for your content. Editing this info explicitly with Open Graph tags helps to improve the quality of posts on Facebook.

I have implement sex `og:` tags (`og` for `Open Graph`) in the head.html in my _includes: 

{% highlight html %}
  <meta property="og:locale" content="en_US">
  <meta property="og:type" content="article">
  <meta property="og:url" content="{{ site.url }}{{ page.url }}">
  <meta property="og:title" content="{% if page.title %}{{ page.title }}{% else %}{{ site.title }}{% endif %}">
  <meta property="og:site_name" content="{{ site.title }}">
  <meta property="og:image" content="{{ site.url }}/images/og-image-1.jpg">
{% endhighlight %}

It is possible to specify custom image for any post to be shared, but IMHO it is little bit redundand in this case.

Be careful! It is bad idea to like, share or comment on viral posts on Facebook!

Why? Rick Rouse, A+ certified computer tech explains in [his viral post][share-info].

Have you read it? Are you agree?

Share if you agree!<br>
![Share-if-you-agree](/images/share-if.jpg)


[share-info]: https://www.ricksdailytips.com/facebook-bait-posts/
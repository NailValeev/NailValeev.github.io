---
layout: post
comments: true
title:  "Humans vs Robots."
date:   2018-11-15 10:36:07 -0600
categories: posts serious
---
Sorry, it is just a clickbait, this post about `humans.txt` and `robots.txt` files ;)

So, what is [humans.txt][humans-info] and what is they used for?
It's a text file with information about the people who have contributed to building the website.
It shall be placed at the site root, next to the robots.txt file. I have add link to this file to the header, 
I mean to the appropriate include:
{% highlight ruby %}
<link rel="author" href="humans.txt">
{% endhighlight %}

I have create it and it takes place there, it contains information about me and creators of Jekyll boilerplate for this site :)
I have no permission to use their contact information, so, you cann't find it their.
Moreover, this site is public, that is why humans.txt is hidden from searching bots. How? The robots.txt is the answer! 

The [robots.txt][robots-info] (also known as the robots exclusion protocol or standard) is a text file used by websites to communicate with web crawlers and other web robots.
The standard specifies how to inform the web robot about which pages or files the crawler can or can't request from your site.
I have create robots.txt and placed it in the topmost directory of my website.
It is pretty simple, in addition to humans .txt is assets directory disallowed, because nothing relevant for indexation :

{% highlight ruby %}
User-agent: *
Disallow: /humans.txt
Disallow: /assets/
{% endhighlight %}

[humans-info]: www.http://humanstxt.org/
[robots-info]: https://support.google.com/webmasters/answer/6062596?hl=en

---
layout: post
comments: true
title:  "CSS - pre-processors vs Vanilla JS."
date:   2018-11-14 11:28:12 -0600
categories: posts serious
---
Pre-compiling of CSS seems to be very useful, especially nesting and mixins, which are amazing I think. 
[Nesting][nesting-info] is very useful and allows to define hierarchy selectors, and [mixins][mixins-info] helps to create the code with high cross-browser compatibility which is re-usable throughout a site. 

In comparison with Vanilla CSS pre-processors wins in case of development a lot of websites from 
templates (it is very common case AFAIK). So, developer can change the look of the pages on-the-fly,
with only variables editing.

I have use both CSS-preprocesssor `SASS` and 'true' plain CSS, a.k.a `Vanilla CSS`. 
The last one I have use only for prototyping, like inline CSS (for example, for footer's background color).
It was replaced later by pre-processor generated styles, in accordance with examination assignment.

Every progamming paradigm has pros and cons of their own. So, pre-processing of CSS works well for large projects
and construction of sites from the templates, but, IMHO, it is not so good for prototyping and building from the scratch.

[nesting-info]: https://www.sitepoint.com/sass-basics-nesting/
[mixins-info]: https://scotch.io/tutorials/how-to-use-sass-mixins

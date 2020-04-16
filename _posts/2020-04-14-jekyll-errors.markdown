---
layout: post
title:  "Jekyll - 2. Liquid - Tags - Errors"
date:   2020-04-14 17:03:45 +0900
categories: jekyll
---

#### 게시물에 연결하기


{% highlight console %}
Regenerating: 1 file(s) changed at 2020-04-16 11:50:51
                    _posts/2020-04-14-jekyll-tags.markdown
       Jekyll Feed: Generating feed for posts
  Liquid Exception: Could not find post "2020-04-14-jekyll-2-liquid.markdown" in tag 'post_url'. Make sure the post exists and the name is correct. in C:/Users/Purple/purplike/_posts/2020-04-14-jekyll-tags.markdown
             Error: Could not find post "2020-04-14-jekyll-2-liquid.markdown" in tag 'post_url'. Make sure the post exists and the name is correct.
             Error: Run jekyll build --trace for more information.
{% endhighlight %}



Unknown tag

{% highlight console %}
 Regenerating: 1 file(s) changed at 2020-04-16 14:56:56
                    _posts/2020-04-14-jekyll-tags.markdown
       Jekyll Feed: Generating feed for posts
  Liquid Exception: Liquid syntax error (line 13): Unknown tag 'row' in C:/Users/Purple/purplike/_posts/2020-04-14-jekyll-tags.markdown
             Error: Liquid syntax error (line 13): Unknown tag 'row'
             Error: Run jekyll build --trace for more information.
{% endhighlight %}
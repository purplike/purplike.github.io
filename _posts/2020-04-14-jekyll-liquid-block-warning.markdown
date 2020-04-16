---
layout: post
title:  "Jekyll - Warning - Found a Liquid block containing the excerpt separator"
date:   2020-04-14 17:03:45 +0900
categories: jekyll update
---

higlight 에 빈 줄을 넣으면 아래 에러발생

{% highlight console %}
Regenerating: 1 file(s) changed at 2020-04-16 11:08:45
                    _posts/2020-04-14-jekyll-regenerating.markdown
           Warning: Excerpt modified in _posts/2020-04-14-jekyll-regenerating.markdown!
                    Found a Liquid block containing the excerpt separator "\n\n".
                    The block has been modified with the appropriate closing tag.
                    Feel free to define a custom excerpt or excerpt_separator in the
                    document's Front Matter if the generated excerpt is unsatisfactory.
       Jekyll Feed: Generating feed for posts
                    ...done in 0.192921 seconds.
{% endhighlight %}


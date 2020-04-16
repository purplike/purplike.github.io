---
layout: post
title:  "Jekyll- highlight"
date:   2020-04-14 17:03:45 +0900
categories: jekyll update
---


List of supported languages and lexers
https://github.com/rouge-ruby/rouge/wiki/List-of-supported-languages-and-lexers

내가 잘 쓸것만 찾음


- console: A generic lexer for shell sessions. 
- html: HTML
- java: The Java programming language (java.com)
- javascript: JavaScript [aliases: js]
- json: JavaScript Object Notation (json.org)
- jsp: JSP
- xml: XML

ruby
{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

console
{% highlight console linenos %}
Regenerating: 1 file(s) changed at 2020-04-16 11:00:45
                    _posts/2020-04-14-jekyll-tags.markdown
       Jekyll Feed: Generating feed for posts
                    ...done in 0.257681 seconds.
{% endhighlight %}

{% highlight html linenos %}
<!DOCTYPE html>
<html>
    <head>
    </head>
    <body>
    </body>
</html>
{% endhighlight %}

와.. 안이뻐...ㅠㅠㅠ
---
layout: post
title:  "Jekyll - Customizing CSS"
date:   2020-04-14 17:03:45 +0900
categories: jekyll
---

실패의 경우들..

C:\Users\Purple\purplike\_site\assets
에 css/scss 폴더 만들어 파일 넣어도 다 사라짐


분명 찾아보면 보러가면
css나 scss 파일 만들고 머리말이랑 아래꺼 까지 3줄 넣으라하는데 빌드하면 다 사라짐..

@import "{{ site.theme }}";



https://help.github.com/en/enterprise/2.14/user/articles/customizing-css-and-html-in-your-jekyll-theme

안됨.. 자꾸 asset안에 내가 새로 만든 파일/폴더만 사라짐..



theme: minima


C:\Users\Purple\purplike>bundle show minima
[DEPRECATED] use `bundle info minima` instead of `bundle show minima`
D:/Ruby25-x64/lib/ruby/gems/2.5.0/gems/minima-2.5.1

C:\Users\Purple\purplike>bundle info minima
  * minima (2.5.1)
        Summary: A beautiful, minimal theme for Jekyll.
        Homepage: https://github.com/jekyll/minima
        Path: D:/Ruby25-x64/lib/ruby/gems/2.5.0/gems/minima-2.5.1

C:\Users\Maria\purplike>


base-font-family:

user urgent stylesheet
D:\Ruby25-x64\lib\ruby\gems\2.5.0\gems\minima-2.5.1\_sass\minima\


### Solution
방법은

테마가 있는 루비폴더에 가서 직접 수정한다!
D:\Ruby25-x64\lib\ruby\gems\2.5.0\gems\minima-2.5.1\_sass\minima\_base.scss
에 code에 css 추가하고 혹시 몰라 변수로 등록함..
코드는 나으 사랑 콘솔라스로 바꿈
근데 웹에 반영될진 몰겠다

{% highlight css %}
  font-family: $code-font;
{% endhighlight %}


{% highlight css %}
  font-family: Consolas;
{% endhighlight %}
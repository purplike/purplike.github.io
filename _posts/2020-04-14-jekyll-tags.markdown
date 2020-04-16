---
layout: post
title:  "Jekyll - 2. Liquid - Tags"
date:   2020-04-14 17:03:45 +0900
categories: jekyll update

---



Tags
{% if page.show_sidebar %}
    <div class="sidebar">
        sidebar content
    </div>
{% endif %}

https://jekyllrb-ko.github.io/docs/liquid/tags/

조각파일
코드 구문 강조
* Jekyll은 코드 블록 안에서도 Liquid 필터를 처리합니다
{% raw %}

{% endraw %}

#### 페이지에 연결하기 (link)
- {% link _posts/2020-04-14-jekyll-2-liquid.markdown %}
: 마크다운에선 안됨
- [Link to a post]({% link _posts/2020-04-14-jekyll-2-liquid.markdown %})
: 마크다운


### 게시물에 연결하기 (post_url)
post_url 태그를 사용할 때에는 파일 확장자를 지정할 필요가 없다.



 {% post_url 2020-04-14-jekyll-2-liquid %}
: 마크다운에선 안됨

[Name of link]({% post_url 2020-04-14-jekyll-2-liquid %})

 post_url 2020-04-14-jekyll-2-liquid.markdown 

#### Error
파일 확장자를 지정했을 경우 발생

{% highlight console %}
Regenerating: 1 file(s) changed at 2020-04-16 11:50:51
                    _posts/2020-04-14-jekyll-tags.markdown
       Jekyll Feed: Generating feed for posts
  Liquid Exception: Could not find post "2020-04-14-jekyll-2-liquid.markdown" in tag 'post_url'. Make sure the post exists and the name is correct. in C:/Users/Maria/purplike/_posts/2020-04-14-jekyll-tags.markdown
             Error: Could not find post "2020-04-14-jekyll-2-liquid.markdown" in tag 'post_url'. Make sure the post exists and the name is correct.
             Error: Run jekyll build --trace for more information.
{% endhighlight %}




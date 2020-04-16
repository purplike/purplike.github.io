---
layout: post
title:  "Jekyll Install"
date:   2020-04-14 17:03:45 +0900
categories: jekyll
---

D 드라이브에 설치하고 싶었는데
C 사용자 폴더에 설치가 되었다...
다시 해봐야하는데 우선 처음 한거 정리

{% highlight console %}
gem install jekyll bundler

jekyll new my-awesome-site

bundle install

bundle exec jekyll serve
{% endhighlight %}


#### Jekyll 과 Bundle 젬을 설치한다.
{% highlight console %}
{% raw %}
C:\Users\Purple>gem install jekyll
Fetching: sassc-2.2.1-x64-mingw32.gem (100%)
Successfully installed sassc-2.2.1-x64-mingw32
Fetching: jekyll-sass-converter-2.1.0.gem (100%)
Successfully installed jekyll-sass-converter-2.1.0
Fetching: kramdown-2.1.0.gem (100%)
Successfully installed kramdown-2.1.0
Fetching: kramdown-parser-gfm-1.1.0.gem (100%)
Successfully installed kramdown-parser-gfm-1.1.0
Fetching: unicode-display_width-1.7.0.gem (100%)
Successfully installed unicode-display_width-1.7.0
Fetching: terminal-table-1.8.0.gem (100%)
Successfully installed terminal-table-1.8.0
Fetching: jekyll-4.0.0.gem (100%)
-------------------------------------------------------------------------------------
Jekyll 4.0 comes with some major changes, notably:

  * Our `link` tag now comes with the `relative_url` filter incorporated into it.
    You should no longer prepend `{{ site.baseurl }}` to `{% link foo.md %}`
    For further details: https://github.com/jekyll/jekyll/pull/6727

  * Our `post_url` tag now comes with the `relative_url` filter incorporated into it.
    You shouldn't prepend `{{ site.baseurl }}` to `{% post_url 2019-03-27-hello %}`
    For further details: https://github.com/jekyll/jekyll/pull/7589

  * Support for deprecated configuration options has been removed. We will no longer
    output a warning and gracefully assign their values to the newer counterparts
    internally.
-------------------------------------------------------------------------------------
Successfully installed jekyll-4.0.0
Parsing documentation for sassc-2.2.1-x64-mingw32
Installing ri documentation for sassc-2.2.1-x64-mingw32
Parsing documentation for jekyll-sass-converter-2.1.0
Installing ri documentation for jekyll-sass-converter-2.1.0
Parsing documentation for kramdown-2.1.0
Installing ri documentation for kramdown-2.1.0
Parsing documentation for kramdown-parser-gfm-1.1.0
Installing ri documentation for kramdown-parser-gfm-1.1.0
Parsing documentation for unicode-display_width-1.7.0
Installing ri documentation for unicode-display_width-1.7.0
Parsing documentation for terminal-table-1.8.0
Installing ri documentation for terminal-table-1.8.0
Parsing documentation for jekyll-4.0.0
Installing ri documentation for jekyll-4.0.0
Done installing documentation for sassc, jekyll-sass-converter, kramdown, kramdown-parser-gfm, unicode-display_width, terminal-table, jekyll after 21 seconds
7 gems installed


C:\Users\Purple>gem install bundler
Fetching: bundler-2.1.4.gem (100%)
Successfully installed bundler-2.1.4
Parsing documentation for bundler-2.1.4
Installing ri documentation for bundler-2.1.4
Done installing documentation for bundler after 22 seconds
1 gem installed




C:\Users\Purple\purplike>bundle install
Fetching gem metadata from https://rubygems.org/...........
Fetching gem metadata from https://rubygems.org/.
Resolving dependencies...
Fetching public_suffix 4.0.4
Installing public_suffix 4.0.4
Fetching addressable 2.7.0
Installing addressable 2.7.0
Using bundler 2.1.4
Using colorator 1.1.0
Fetching concurrent-ruby 1.1.6
Installing concurrent-ruby 1.1.6
Using eventmachine 1.2.7 (x64-mingw32)
Using http_parser.rb 0.6.0
Using em-websocket 0.5.1
Fetching ffi 1.12.2 (x64-mingw32)
Installing ffi 1.12.2 (x64-mingw32)
Using forwardable-extended 2.6.0
Fetching i18n 1.8.2
Installing i18n 1.8.2
Using sassc 2.2.1 (x64-mingw32)
Using jekyll-sass-converter 2.1.0
Using rb-fsevent 0.10.3
Fetching rb-inotify 0.10.1
Installing rb-inotify 0.10.1
Fetching listen 3.2.1
Installing listen 3.2.1
Using jekyll-watch 2.2.1
Using kramdown 2.1.0
Using kramdown-parser-gfm 1.1.0
Using liquid 4.0.3
Using mercenary 0.3.6
Using pathutil 0.16.2
Fetching rouge 3.18.0
Installing rouge 3.18.0
Using safe_yaml 1.0.5
Using unicode-display_width 1.7.0
Using terminal-table 1.8.0
Using jekyll 4.0.0
Fetching jekyll-feed 0.13.0
Installing jekyll-feed 0.13.0
Using jekyll-seo-tag 2.6.1
Fetching minima 2.5.1
Installing minima 2.5.1
Fetching thread_safe 0.3.6
Installing thread_safe 0.3.6
Fetching tzinfo 1.2.7
Installing tzinfo 1.2.7
Fetching tzinfo-data 1.2019.3
Installing tzinfo-data 1.2019.3
Using wdm 0.1.1
Bundle complete! 6 Gemfile dependencies, 34 gems now installed.
Use `bundle info [gemname]` to see where a bundled gem is installed.
Post-install message from i18n:

HEADS UP! i18n 1.1 changed fallbacks to exclude default locale.
But that may break your application.

If you are upgrading your Rails application from an older version of Rails:

Please check your Rails app for 'config.i18n.fallbacks = true'.
If you're using I18n (>= 1.1.0) and Rails (< 5.2.2), this should be
'config.i18n.fallbacks = [I18n.default_locale]'.
If not, fallbacks will be broken in your app by I18n 1.1.x.

If you are starting a NEW Rails application, you can ignore this notice.

For more info see:
https://github.com/svenfuchs/i18n/releases/tag/v1.1.0


C:\Users\Purple\purplike>bundle exec jekyll serve
Configuration file: C:/Users/Purple/purplike/_config.yml
            Source: C:/Users/Purple/purplike
       Destination: C:/Users/Purple/purplike/_site
 Incremental build: disabled. Enable with --incremental
      Generating...
       Jekyll Feed: Generating feed for posts
                    done in 1.115 seconds.
 Auto-regeneration: enabled for 'C:/Users/Purple/purplike'
    Server address: http://127.0.0.1:4000/
  Server running... press ctrl-c to stop.
{% endraw%}
{% endhighlight %}

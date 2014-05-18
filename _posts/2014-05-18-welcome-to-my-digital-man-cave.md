---
layout: post
title:  "Welcome to my digital man cave!"
date:   2014-05-18
---

I needed a way to save the little things I try out. Tada! My **digital man cave** is born.

There is no specific theme to this blog other than record what interests me, what I test, like and use. There will definitely be some ruby, because I love it and whatever else I end up using. It'll be Mac OS X and Linux centric. There will be shell, code, software ... the usual geek stuff really.

BTW, I liked the [Bash and Dash](http://brettterpstra.com/2014/05/10/bash-and-dash/) article from Brett Terpstra ([@ttscoff](https://twitter.com/ttscoff)) because it was so simple and straightforward. While reading it, it automatically triggered a "Could I do this in ruby?" question. And it turns out, I can and it's, as well, dead simple. Here's my `rdash` ruby script that I copied to */usr/local/bin*:

{% highlight ruby %}
#!/usr/bin/env ruby

require "erb"
include ERB::Util

%x[open dash://#{u(ARGV.join(' '))}]
{% endhighlight %}

Now, when I'm in the terminal, I can just do `rdash ruby:FileUtils mv` to look up the documentation in [Dash](https://itunes.apple.com/fr/app/dash-docs-snippets/id458034879?l=en&mt=12).

OK, granted, I usually don't do this, and I didn't feel a need to do it because Dash is a Ctrl-SPACE away with the global search shortcut I chose. I sometimes use the [Alfred](http://www.alfredapp.com/) workflow that comes with Dash (in the lastest versions). I often use Ctrl-h in [Sublime Text](https://github.com/farcaller/DashDoc) or [Atom](https://github.com/blakeembrey/atom-dash). This being said, the "Bash and Dash" article led me to try something new and I have one more way to interact with a tool I use almost every day.

Anyway, I digress. One idea leads to the next, one link leads to the rabbit hole and hours fly.

Welcome :)

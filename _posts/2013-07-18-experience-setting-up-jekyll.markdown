---
layout: post
title:  "Experience setting up Jekyll"
date:   2013-07-18 22:30:00
categories: jekyll install
---

Well I have started with [jekyll][jekyll] around 3 weeks ago, but I ran into a couple issues locally which I haven't actually been able to resolve yet. I seem to get random old artifacts in my fragments even when I delete the `site` directory. For someone like me, who isn't really that versed with style and layout this was a major drawback.

I have html fragments in my pages after changing the sources and seeing unpredictable output is not fun, especially when you are experimenting with **new** technologies (new as in *no experience*).

Since I had quite a few other projects to work with I put the github pages onto the shelf and focused on the other ones. But last weekend I saw a post on [reddit][reddit] of a guy who prototyped a page during the weekend and he bootstrapped it quite easily. The interesting thing was, that he used [layoutit][layouit] for a quick layout for the page.

So I went on and gave it a shot today and actually managed to set something up, which I think does not look too bad. But after merging the new layout into the skeleton I already had for the page, I ran into a few problems.

I still had and maybe have the problem with old html being generated even tho it does not exist locally anymore. The fun part is, that it works fine on github-pages so I'm not too bothered at the moment (especially since updating jekyll did not change anything).

Next I realized that relative URL's obviously won't work, since posts are in a different directory. This let me to [this post][chho.se] but be aware, that this did not work for me right out the box. To run it locally I had to use the command `jekyll serve –-baseurl=“”` instead of the suggested command. But now I actually have all the css, js and correct links available.

Now I just need to figure out how to fix the local issues. I'm on Mac OS X with [Sublime Text][sublime] 2.0.2 and [jekyll 1.1.0][jekyll].


[jekyll]:    http://jekyllrb.com
[reddit]:    https://www.reddit.com
[layouit]:   http://www.layoutit.com
[chho.se]:   http://www.chho.se/2013/05/16/jekyll-github-pages-and-making-it-run-both-on-github-and-locally/
[sublime]:   http://www.sublimetext.com
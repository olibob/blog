---
layout: post
title:  "Git webhook made easy"
date:   2014-05-18
tags: git apache
categories: git apache
---


The question: How could I only push my website to github and have it automatically updated on my web server? The answer: [apache-git-sync-tool](https://github.com/Perennials/apache-git-sync-tool). Its great!

I think I googled around for about 3 hours, trying different things on a vagrant box, but to no avail. Frustration is growing rapidely. And ... humm ... this could be something. And boom! It is.

There is not much else to say than: **"Follow the readme"**. You can't go wrong if you stick to it.

Krum Stoilov and Borislav Peev have done a fantastic job to make a complicated endeavour ... quite easy.

My server is running Fedora (yeah, I like it risky), so don't be alarmed by the error when you create the ssh keys. Go to */usr/share/httpd/* and create a *.ssh* directory and `chown -R apache:apache .ssh && chmod 600 .ssh`.

Once your done, a simple git push from your workstation is going to update your website on your server. Isn't it great to be lazy?

**Tip**: Run the webhook url (http://yoursite.com/sync.php?project=happyworld&branch=peace) yourself in your browser to get feedback from the sync.php script. It'll be helpfull to debug any little error that you slipped in.

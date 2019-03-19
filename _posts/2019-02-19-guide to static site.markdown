---
layout: post
author: Aakash
title: A to Z about your new website
---
Where it all begins
====================

>First, go to the [**website**](https://register.com.np/) . Sign up if you haven't before and fill up the details. Filling up the basic info wont be a hassle but many tend to get confused on filling up the server tab. I too got stucked on that portion due to lack of blogs. A friend of mine too wrote a blog but the information wasn't adequate 😀. Anyway back to the drawing board.
Primary and secondary dns info is to be filled but initially u do not have any dns. So, what we do is fill up the info with dummy dns that we get from cloudfare community. just google a bit and search for some free dns. For your reference, I got 2 dummy cloudfare nameservers from a bit of googling:
* fred.ns.cloudflare.com
* kate.ns.cloudfare.com
> U can find plenty of them but I recommend using cloudfare be it for the dummy as well. Also be meticulous on this portion as it can waste so much of your time, dont add extra slash and to be further assured, perform nslookup or dig to see if the servers u just added there are working or not.if on linux, u can just check by using dig "your dummy-dns" and if the info is shown on the console, its a success and you can move forward. u can also check the state of dns by just googling and checking nslookup and dig as well. So, after filling all the required information, the [site](https://register.com.np/) will work on registering your brand new domain. It may take 24 to 48 hours for it to process.

### Install static site generator
>This is the tool for u to work on your website. You can use either Jekyll or hugo. I used Jekyll since its supported by github. Assuming you already have a github account, create a new repository there.
But before that, go to terminal and install jekyll with command:
gem install jekyll
if ruby isnt installed, ruby should be installed prior to it.
U can take reference from this article on setting up a new repository and hosting it on github until your domain is ready to be hosted under [cloudfare](https://www.cloudflare.com/). Just follow the step 1 of this reference [article](https://blog.cloudflare.com/secure-and-fast-github-pages-with-cloudflare/). Go to the official site of jekyll and u will find the guide to deal with making new posts, editing layout and so on. But for now just create a simple markdown post and commit it on github account.

### Cloudfare to the rescue
>I tried blogging couple of years ago and found the process really cumbersome. Hosting sites like 00webhost were very slow and the it had to deal with unnecessary traffic obstructions and whole lot of other problems. But with cloudfare u dont need to host. This is the age of minimalistic sites, make your sites more precise and let contents do the talking not the design and other fancy stuffs. Go to **cloudfare** and register, its a simple process. After a couple of days, the [site](https://register.com.np/) must have activated your new domain. Ads new site to the cloudfare option and enter your new domain name there. Now, cloudfare will provide u with original nameservers. It provides u the information to change previous dummy nameservers with your new valid nameservers. Now go back to [site](https://register.com.np/)and under the section "dashboard",u will find edit dns info. And replace your previous nameservers with new nameservers provided by cloudfare. Thats it. It may take about 24 hours for the site to get activated after editing the nameservers.
Now, point the address of your github to the new domain. Follow the step 2 of this [article](https://blog.cloudflare.com/secure-and-fast-github-pages-with-cloudflare/)
And done. Now you can enable SSL certificate and other stuffs through cloudfare.
Your new site is up and ready to go.

> **BOOM**

> [Using Jekyll](https://jekyllrb.com/)


---
layout: post
title:  "10 Ways To Make Your Site Super Fast"
author: harpreet
categories: [ tech, web ]
tags: [ skills, efficiency ]
image: assets/images/speedupyoursite.jpg
featured: false
hidden: false
rating: 4.5

---

Everyone hates a slow running site. It's bad for business, and painful for users accessing it. There are some ways to make your site, Super Fast and Awesome.

#### 01. Less is More.

Start with the inception phase. When you are designing your website, keep only utmost necessary blocks in the layout. Get rid of things you don't need. You will be surprised on how much thinking it takes just to narrow down your site to those minimal features.

Use minimal and clean design. Easier for eyes and you will have better 'Call to Actions'.

#### 02. Hosting your Site.

This can get tricky for many new business owners. The thumb rule is simple, if your target group is from UK, you host your site in the closest vicinity. I personally love <a href="https://m.do.co/c/a10484df87ed">Digital Ocean.</a> for small to medium scale websites and AWS for enterprise solutions.


#### 03. Use a Content Delivery Network
A CDN (Content Delivery Network) will cache your entire site and store it in multiple nodes. Any user accessing the site will get the site's content delivered from the nearest CDN node from their location. Cloudflare is a great option to start with, it not only provides a great set of caching and security tools, but also secures your site for free. For enterprises, I would suggest use of premium services by Cloudflare or Akamai.


#### 04. Page Size

If you page is heavy, it will take more time to load. Simple. Reduce your page size, by optimising all your media assets. You can optimise all your images to be suited for web. Use progressive Jpegs wherever possible and PNGs only when transparent background is needed. Image formats like WebP (from google) and HEIC/HEIF are comparatively new and promising, but will need support from all major browsers and operating systems.

#### 05. Page Requests

There is a limit of concurrent request to a domain which browsers can make. For example if a browser can at max make 8 concurrent request to a domain for files, next set of 8 requests from the same domain will need to wait before the first set gets served (Another reason to use a content delivery network for media assets). Reducing the number of requests per page will significantly improve the site's performance.

#### 06. Lazy Loading Images

Lazy loading is a method where an image loads after we scroll down to a block which has that image. This is a very powerful technique where you only load images which can be seen from the first fold of page load. This significantly reduces your page size as well as number of requests needed to paint the page.

#### 07. Cache everything you can and wherever you can.

All your static assets must be cached. Your browser can also cache all your files. Some modifications in Nginx/Apache (I hope you use Nginx) configuration file can help you attain better caching. Varnish is an amazing service which can help to cache your entire website.

#### 08. Distributed Web Architecture / PWA

Separating your frontend from backend is a great way to build web apps. It will enable you to improve the UI without worrying about fallbacks of the CMS it is built on. I have written a separate post on <a href="https://stories.ahyconsulting.com/heading-for-headless/" >PWA's and Distributed Architecture </a>.


#### 09. Code Wisely

No amount of caching can cover up for bad code. Caching should be used to complement your application layer, and not to cover up for a bad one. Think hard to make algorithms, check online what practices others are following, look for simplicity. If your solution is not simple, it probably is not the right one yet. Test driven development is the right way of development.


#### 10. Data Distribution

Separate your data based on workflows on the site. Shard your database for specific kind of queries. I personally love using ElasticSearch on the frontline for all non transactional data with a fallback mechanism if data is not stored on ElasticSearch cluster and relational databases like MariaDB for transactional data. You will be amazed on how much offloading can happen from one datasource.


#### Results?

Screenshot from Google Page Speed Insights of our blog.

<p class="mb-5"><img class="shadow-lg" src="{{site.baseurl}}/assets/images/psi-mobile.jpg" alt="{{ site.title }}" /></p>

<p class="mb-5"><img class="shadow-lg" src="{{site.baseurl}}/assets/images/psi-desktop.jpg" alt="{{ site.title }}" /></p>


There are some speed optimisation techniques which are specific to applications like Magento, Wordpress etc. which I have not listed down. <a href="mailto:harpreet@ahyconsulting.com">Get in touch with us</a> if you would like us to assist you in speeding up your website.

Happy Coding!

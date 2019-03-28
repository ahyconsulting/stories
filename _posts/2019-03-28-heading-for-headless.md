---
layout: post
title:  "Heading for Headless?"
author: harpreet
categories: [ tech, web ]
image: assets/images/close-up-disjunct-farming-1437587.jpg
featured: false
hidden: false
---

So what is headless exactly? Why is there so much buzz around it in the tech world, specifically pertaining to web technology? Let's find out.

#### My First Encounter, flashback!

Back in 2011, when I was working with an enterprise eCommerce site based on Magento, speed and performance was a HUGE priority and I was exploring a lot of white papers and best practices of fine tuning performance. Huge category, caching, Varnish, hole punching, worker fine tuning, service level optimisations, code optimisation, Redis, everything was done right. Everyone was happy with the performance, as we had reached a new benchmark at organisational level.

I was also exploring ElasticSearch at that time and was pretty much amazed with its capabilities. We had implemented elasticSearch with Magento search but I was sure, ElasticSearch can be used as a very important tool for many other things.

I thought of modifying Magento to render the entire catalog from ElasticSearch as first data source and only to go back to database as fallback.

We implemented this and performance was off the charts. The site was blazing fast. We also significantly reduced the server utilisation.
Our team celebrated and termed this way of design as <b>Giving Wings to Magento!</b>


This led to the foundation of decoupled architecture for me.


#### So what is headless architecture?

<p class="mb-5"><img class="shadow-lg" src="{{site.baseurl}}/assets/images/headless-architecture.jpg" alt="{{site.title}}" /></p>

Browser only understands Javascript, HTML, CSS and static assets like images, videos etc. So in headless architecture, we separate the entire frontend in Javascript application for rendering HTML and the content of the website is accessible via APIs.


#### Why Does it Matter?

Entire focus is now shifted to a frontend driven application. Better user experience and better interaction. It has number of benefits.

+ <b>Speed</b>. By shifting logic of rendering the frontend to the client side, the frontend application has less baggage to carry. Backend is now a true server of content and purely focuses on data delivery.

+ <b>Frontend Developers are Happy.</b> By setting the frontend developers free from overlapping responsibilities of the backend, this architecture gives them the opportunity to take full control of the user experience. Needless to say, roles like frontend architecture and frontend developer has an entirely new meaning today.

+ <b>Breaking Barriers.</b> Remember the times when you choose one CMS, and you were bound by its features? With headless, you can use best tools or CMS for your project, expose the APIs, facilitate the handshake over a unified platform (Hello, GraphQL!) and you are good to go.


#### Demystifying the Jazz

<p class="mb-5"><img class="shadow-lg" src="{{site.baseurl}}/assets/images/abstract-art-background-1037992.jpg" alt="{{page.title}}" /></p>


To sum up, headless website development has the potential to unleash the creative power of front-end developers to deliver faster, more responsive, and richer user experiences. You can see why everyone is so excited.


Need Help with your headless project? <a href="mailto:harpreet@ahyconsulting.com">Contact Us!</a>

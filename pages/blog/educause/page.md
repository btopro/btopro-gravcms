---
title: 'NGDLE is really just Enigma misspelled'
media_order: 'NGDLE-university-uni-side.jpg,NGDLE-university-faculty-side.jpg,2018-01-24_16-39-55.png,2018-01-24_16-40-31.png,lrn-table.jpg,wikipedia-query.jpg,aframe-player.jpg,paper-audio-player.jpg,2018-01-31_10-01-18.png,NGDLE-university.jpg'
published: true
process:
    markdown: true
    twig: false
---


<p>I mean look at it! It's a bunch of random letters that's hard to pronounced or use in a sentence. Years after initial usage, people still have difficulty saying what one is beyond pictures of childhood toys. My poking fun is in gest though, it's a complex idea and it at least evokes an important mental picture of "things beyond the LMS matter... a lot".
At Penn State, I've been fortunate to been building this weird thing called <a href="https://www.elmsln.org/">ELMS: Learning Network</a>
. It's an open source NGDLE and I started development prior to the term (<em>fun fact</em>
). For those on the development team, NGDLE means Next Generation <strong>Distributed</strong>
 Learning <strong>Ecosystem</strong>
.
<a href="https://www.elmsln.org/">ELMS:LN</a>
 and the projects that make it up (it's actually a system of systems) seek to provide those mythical lego-grid-plates in the NGDLE picture. We provide some of the bricks out of the box to give you some ideas, but the real power is in the philosophy of design of the system. No matter what bricks you plug into the grid plate, you'll need a grid to keep it together and this is an attempt to be one of those grid plates.
We've been running courses via <a href="https://www.elmsln.org/">ELMS:LN</a>
 since 2014, so what does our vision of NGDLE look like? What does any of this actually <strong>mean</strong>
 or <strong>look like</strong>
 or <strong>do</strong>
? Hopefully this will help. Let's start at the highest level and drill down from there to real things. (click to expand)
<a href="/educause/NGDLE-university.jpg"><img alt="NGDLE University to Faculty to Student relationships" src="/images/e/4/e/1/7/e4e17905cd786316dd2485bc5e6bc8854f18661b-ngdle-university.jpeg"/></a>
</p>

<h2>Universities, Colleges and NGDLE</h2>

<p><img alt="University with the universe of apps that exist today" src="/images/9/3/5/b/7/935b7d832386eaf3173d063a70fe5000fc03dc1c-ngdle-university-uni-side.jpeg"/>
Universities buy and build solutions but one of the biggest issues no matter what is getting people to know that the thing even exists! There's all kind of things we need in different disciplines too, and that won't change, but how we integrate with them should. Taking a page from <a href="https://developer.byu.edu/docs/design-api/university-api-standard">BYU's University API</a>
, we have one system that we integrate everything with! This is a grid plate for APIs, all plugged in to provide access to data and experience providers. This grid plate we call the "HAX App Exchange".
<img alt="Faculty member and their engagement with the universe" src="/images/5/9/4/5/3/59453a821222752c90fa970c937c2c396bff61f5-ngdle-university-faculty-side.jpeg"/></p>

<h2>Instructors and Instructional Designers</h2>

<p>So we've got our integrations unified but what about where we all consume these things? LMSs, CMSs and portals all integrate with, build and present information differently. One plugs into Box / Google Drive, another doesn't. One talks LTI, the other less fluent. To TRY and simplify things we just said "talk LTI vendors" and many do, but there's way more that don't (and never will). So you go to different places for information (and your students do too) and you get a lot of cognitive load every time you have to learn something new just to put the file into one place vs another. Isn't there a better way to handle the consuming side of systems?
Imagine if we had a remote control for instructional system construction. If we could tell files where and how we want them available to users with minimal cognitive load. If it worked anywhere. In LMSs, CMSs, even desktop and mobile apps! Think of it like the <a href="http://btopro.com/blog/the-lms-is-cable-we-are-roku">Roku remote for education</a>
; stitching together a universe of separate "channels" into one unified interface while providing a standard way of presenting them.</p>

<h2>HAX - Headless Authoring eXperience</h2>

<p>HAX is short for Headless Authoring eXperience; which means that it can be integrated agnostic of any system! Think WYSIWYG editor but on steriods and built future focused (and actually WYSIWYG not Sorta-what-you-wanted-is-what-you-get). We've currently wired HAX into <a href="https://www.elmsln.org/">ELMS:LN</a>
, <a href="https://www.drupal.org/project/hax">Drupal 6, Drupal 7</a>
, <a href="https://github.com/elmsln/grav-plugin-hax">GravCMS</a>
, <a href="https://backdropcms.org/project/hax">BackdropCMS</a>
 and <a href="https://github.com/LRNWebComponents/hax-desktop-app">a desktop app</a>
. The goal isn't to stop there, it's just to illustrate that we can build an identical authoring experience across platforms utilizing the exact same code to do so.
So if we reach out and enhance our platforms that exist currently, but tie them into this "HAX App eXchange" grid plate; what does that look like?</p>

<h2>Visuals</h2>

<p><a href="http://haxtheweb.org">Click here to play with HAX</a>

If I want to edit the way a video looks, I can click and modify it.
<img alt="Placing a video in HAX" src="/images/f/8/6/7/4/f86741992df19f17d8ce4363a54f7b5488a433d9-2018-01-2416-40-31.png"/>
If I want to embed a video from Youtube (or any number of sources, growing quickly), I can search, select, and customize all in one place without ever leaving the app.
<img alt="Search the HAX app exchange" src="/images/1/f/a/0/3/1fa0330c3a59eb0cc283d3c0f50ca6c2f8ea291a-2018-01-3110-01-18.png"/>
If I want to modify an element, HAX presents a consistent form for doing so:
<img alt="Customize how a video is presented" src="/images/6/3/8/e/1/638e1b9aa04f832b94b3990fd81337636577cb0a-2018-01-2416-39-55.png"/>
We've starting to pull media in from NASA, Kaltura, Vimeo, Youtube and internal sources. These are all just the beginning!</p>

<h2>How is this possible?!?</h2>

<p>HAX is built on <a href="https://www.webcomponents.org">Webcomponents</a>
. Webcomponents are changing the way people build things on the web. Imagine HTML but you could define your own tags. If I wanted a branded video player, I could utilize a <code><video-player></code>
 tag and the browser understand the definition and builds it (think HTML that unpacks to other HTML). Here are some more examples we've built for HAX so far:
<img alt="An accessible table of data automatically generated from a CSV file" src="/images/5/d/0/0/1/5d001abe3546a023f3d0a7ad1290c8413119286f-lrn-table.jpeg"/>
<img alt="Embed Audio files in a highly accessible, customizable player" src="/images/7/d/6/3/4/7d6343c00020facd641ecd1827f9d2a3d995b920-paper-audio-player.jpeg"/>
<img alt="Query and embed wikipedia in real time" src="/images/e/0/c/5/2/e0c528920979e1f866a1ef709acea7fbe4e5aeb9-wikipedia-query.jpeg"/>
<img alt="Embed 3D environments directly in the web!" src="/images/9/b/9/1/f/9b91f14f7fc21a27ca87a415945ec7c186ec25e2-aframe-player.jpeg"/></p>

<h2>Future of HAX App eXchange</h2>

<p>Why stop at media? What if we could tell the LMS we have an assignment (so we need a grade book entry) while simultaneously invoking a studio instruction space to be created for students to learn. What if we could <a href="https://www.youtube.com/watch?v=Qn8LjXjtwTg">say the things we wanted it to do</a>
 and bring the technology to us instead of us to it!
</video-player></p>


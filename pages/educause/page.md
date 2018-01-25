---
title: NGDL...Enigma
media_order: 'NGDLE-university.jpg,NGDLE-university-uni-side.jpg,NGDLE-university-faculty-side.jpg,2018-01-24_16-39-09.png,2018-01-24_16-39-55.png,2018-01-24_16-40-31.png,lrn-table.jpg,wikipedia-query.jpg,aframe-player.jpg,paper-audio-player.jpg'
---

NGDLE might as well be Enigma misspelled.
I mean look at it! It's a bunch of letters thrown at the wall. It's hard to pronounced or use in a sentence. Years after usage people still have difficulty saying what one is beyond pictures of legos or other childhood toys. My poking fun is in gest though, it's a complex topic and it at least evokes a certain mental picture.

At Penn State, I've been fortunate to been building this weird thing called ELMS: Learning Network the past few years. It's an open source NGDLE and started development prior to the term existing (fun fact). For those on the development team, comprised of multiple colleges and outside collaborators, NGDLE to us means Next Generation **Distributed** Learning **Ecosystem**.

We feel it is important to emphasize that what we're all building embraces **decentralization** and **ecosystems**. No matter how hard we try, solutions will come from almost anywhere at big universities. Grants, inspired faculty, "rouge faculty", college specific and domain specific tools; solutions can and will come from almost anywhere, both decentralized and centralize.

So how can we best support this mishmash of distributed tools from "those damn rouge faculty"? We embrace them. Explore the problems they are actually solving (and causing) with their solutions. And help give them a framework and methodology for working with the bigger picture.

ELMS:LN and the projects thatm ake it up (it's actually a system of systems) is an attempt at be that mythical a lego-grid of NGDLE. We provide some of the bricks out of the box to give you some ideas, but the real power is in the philosophy of design of the system. No matter what bricks you plug into the grid plate, you'll always have need for the grid to keep it all together and this is an attempt to be one of those grid plates. ([Check us out if you want to learn more about it!](https://www.elmsln.org)).

Anyway, what does this look like though? We've been running courses via ELMS:LN since 2014. What vision of the NGDLE future are we looking for as a result? What does any of this actually **mean** or **look like** or **do**?
[![NGDLE University to Faculty to Student relationships](NGDLE-university.jpg)](NGDLE-university.jpg)
Great question! Hopefully I can help. So let's start with a high level institutional diagram and drill down from there to real things. (click to expand)
![University with the universe of apps that exist today](NGDLE-university-uni-side.jpg)
## Universities, Colleges and NGDLE
Universities buy and build stuff, but one of the most common things after either of these is the old SEO problem: communicating to the people that need a thing that the thing even exists! There's all kind of things we need in different disciplines too, and that won't change, but how we integrate with them will! Taking a page from [BYU's University API](https://developer.byu.edu/docs/design-api/university-api-standard), we have one system that we integrate everything with! No matter what other integrations exist, we MUST integrate with this system so we can **integrate anything with it**. This is one grid plate, as all legos (with studs being APIs) plug into it to provide access to data and experience providers. This grid plate we call the "HAX App Exchange".
![Faculty member and their engagement with the universe](NGDLE-university-faculty-side.jpg)
## Instructors and Instructional Designers
So we've got our integrations unified but what about where we all consume these things? LMSs, CMSs and portals all integrate with, build and present information differently. One plugs into Box / Google Drive, another doesn't. One talks LTI, the other less fluent. To TRY and simplify things we just said "talk LTI vendors" and many do, but there's way more that don't (and never will). So you go to different places for information (and your students do too) and you get a lot of cognitive load every time you have to learn something new just to put the file into one place vs another. Isn't there a better way to handle the consuming side of systems?

Imagine if we had a remote control for instructional system construction. If we could tell files where and how we want them available to users with minimal cognitive load. If it worked anywhere. In LMSs, in CMSs, even in desktop apps. Think of it like the [Roku remote for education](http://btopro.com/blog/the-lms-is-cable-we-are-roku); stitching together a universe of separate "channels" into one unified interface.
## HAX - Headless Authoring eXperience
We call our unified user experience HAX, [which you can play with yourself in a live demo here](http://haxtheweb.org). HAX is short for Headless Authoring eXperience; which means that it can be integrated agnostic of what system it is integrated into. Think of a WYSIWYG editor but on steriods and built with the best of the future of the web. To prove this, we've currently got support for HAX into ELMS:LN, Drupal 6, Drupal 7, GravCMS and Backdrop CMS. The goal isn't to stop there, it's just to illustrate that we can build an identical authoring experience across platforms utilizing the exact same code to do so.

So if we reach out and enhance our platforms that exist currently, but tie them into this "HAX App eXchange" grid plate; what does that look like?
## Examples in practice
If I want to edit the way a video looks in a course, I should be able to reach out and touch the video and modify it.
![Placing a video in HAX](2018-01-24_16-40-31.png)

If I want to embed a video from Youtube, I should be able to search, find, select, and customize all in the same place without ever going to Youtube.
![Search the HAX app exchange](2018-01-24_16-39-09.png)

If I want to modify some additional properties about how that's presented, I should have a clean, consistent interface for doing so no matter what or where it comes from.
![Customize how a video is presented](2018-01-24_16-39-55.png)

This is how you interface with systems and complex media in HAX. And Youtube, is just the beginning. What if we could wire anything up to the HAX app exchange and then create an infinite ways to accessibly present that information? We're starting to pull media in from NASA, Kaltura, Vimeo, Youtube and our own sources.

### How is this possible?!?
HAX is built on a technology called [Webcomponents](https://www.webcomponents.org). Webcomponents are changing the way people build things on the web. Imagine HTML but you could define your own tags. If I wanted a branded video player, I could utilize a `<video-player>` tag and it would render. Here's some examples of other tags we've been working on (of which we currently have 120 + the community)
![An accessible table of data automatically generated from a CSV file](lrn-table.jpg)
![Embed Audio files in a highly accessible, customizable player](paper-audio-player.jpg)
![Query and embed wikipedia in real time](wikipedia-query.jpg)
![Embed 3D environments directly in the web!](aframe-player.jpg)
The ELMS:LN team is over the moon about webcomponents and we hope soon you will be too!

### The future of the app exchange
Why stop at just media? What if we could start setting up courses with our remote? What if we could tell the LMS we have an assignment (so we need a gradebook entry) while simultaneously invoking a studio instruction space to be created for students to learn. What if we could [say the things we wanted it to do](https://www.youtube.com/watch?v=Qn8LjXjtwTg) rather than going anywhere.
---
title: 'Using Webcomponents to unearth the NGDLE'
media_order: file0001000292998.jpg
image: file0001000292998.jpg
taxonomy:
    tag:
        - NGDLE
        - webcomponents
---

I find innovation best comes from the cross-sections. The weave between spaces tends to breed the best ideas of the two fabrics to create something new. It is this mentality that's caused me to look outside the island of edtech first, always asking "What can I bring back to our space to make it better?". 10 years ago, that was Drupal. I evangelized Drupal everywhere I could, wrote hundreds of modules, positively impacted tens of 1000s of sites in and out of education while making it possible for individual developers to leverage open source automation to do awesome things. Today I write to talk about the next thing I want to bring back to our island which I think is *the* technology to bring about an open ecosystem for the Next Generation Digital Learning Environment (NGDLE).
## Webcomponents explained
That technology, is webcomponents. Webcomponents, which you can find out more about on [webcomponents.org](https://www.webcomponents.org/) is a four part browser standard that fundamentally changes what's possible in web based application development. The important thing to know is that webcomponents allows developers to define *custom HTML elements and expresses how the browser handles them*. So, bringing this back to education: *We can use this technology standard in order to build [pedagogically focused, valid, HTML tags](https://github.com/LRNWebComponents/)*.
### Quick note
This is a standard that all major browser vendors have committed to adopting and largely have, though polyfills are required to get full browser support. It also is leaving the IE6/7/8/9/10 world behind (the good news is, [so has Microsoft](http://www.telegraph.co.uk/technology/microsoft/12087103/Microsoft-to-kill-off-Internet-Explorer-8-9-and-10.html)).
## NGDLE backstory
For [four years](http://btopro.wordpress.com) I've been building [ELMS: Learning Network](https://www.elmsln.org/); trying to build a platform that can produce and sustain innovation in educational technology. For about that long, Educause has talked about the concept of NGDLE; what it might look like, what it might do, how to do it. Because it's a big concept to unpack, it's taken a few years to get people all on board with the idea and to agree that it's not an LMS (much like webcomponents was proposed in 2011 yet didn't become a real thing implemented until 2016). Because of the patterns of behaviors and methodology of ELMS:LN I currently consider it the only public NGDLE. For that reason, we're misunderstood but if NGDLE is Lego'ing / app-ifying the LMS; ELMS:LN wants to be the grid-plate. The fundamental base-plate to be plugged into. A routing system to stitch it all together and satisfy the need that no vendor will ever provide: a middleware to pull our ecosystems together.
## So how do we all lego
Ok, so back to webcomponents. If we have a gridplate (you could provide your own, I'm not suggesting ELMS:LN be the only one) then we need lego bricks to plug into the board. But what fits that paradigm? Webcomponents allow you to take simple forms of HTML and build it up into increasingly complex elements. Let's look at a simple concept of a custom tag and how it would start to get towards pedagogically centric HTML.
```
button
- div
- a
- text
- /div
```
Just like HTML, custom tags can go into other custom tags. It can also use and retain semantic meaning just like HTML markup. So let's imagine that we had a semantic, custom element that provides the same thing as above. Now we have a tag called `paper-button` and every time I want to do above, I put that tag. Ok, now let's say I want a comment card. A comment card might be:
```
comment-card
- div
- profile-icon
- text
- paper-button to save
- paper-button to reply
```
Which I can then use in something bigger and now I have a tag called [comment-list](https://lrnwebcomponents.github.io/lrnsys-comment/components/lrnsys-comment/demo/#) or `discussion-board`. A discussion-board could be made out of any number of other smaller lego brick tags. Now I wire it up to a backend to save the data and I've got a fully functional HTML element that can be shared and remixed anywhere and so long as someone provides a backend to store it, it's going to work.
## Critical concepts that webcomponents provide to NGDLE if we do this right
1. Visual consistency - right now when using multiple systems everyone decrys the cognitive load on students. webcomponents can provide a common visual design language and templated approach to help alleviate this. Everything will feel like it's the same (even if it's not)
2. Accessibility - Because most accessibility mistakes happen when HTML is created, this allows us to make elements with high accessibility baked in, eliminating the ability for end-users to make that design element inaccessible.
3. Maintainability - If we were to produce a tag such as `lrn-assignment` that expressed an assignment's properties visually, we can now swap out the guts of that tag and so long as the properties going into it are the same we don't need to update any existing content produced.
4. Interoperability - By design, anything that imports the custom element (which is jsut an HTML file supplying the definition of what to do with that tag) will work. These will work in any system because it's the user's browser that's unpacking what it is and the specification itself gives the element definition and encapsulation.
5. Standards based approach - by using a common methodology for front-end creation, we can standardize the UX and interaction patterns of our users and allow developers to all work together and utilize each other's lego bricks.
6. Schema without Schema - We can start to wire up our custom elements to be schematized for indexing by search engines or our own advanced crawlers, ensuring there is additional semantic meaning to our content no matter where it lives. This has [huge implications for OER](http://oerschema.org) for example.
7. Common Authoring - Because [we just made this](http://haxtheweb.org) and it works anywhere.
## Anywhere?
Yeah, anywhere. HAX is another step towards my vision of NGDLE and the solutions we can craft when we work in this approach. An authoring experience that can pull data from anywhere and assemble it in a standards based format (HTML) which can be deployed anywhere. Imagine having identical authoring and instructional capabilities regardless of where an instructor is assembling a course. Open system? Do it in the open. Closed to the institution? Do it in the LMS. Training exercise or learning module on a random blog? Yeah, with an NGDLE based authoring approach, everything can be a mini-LMS and everything can feed other things to make new Learning experiences.

In the coming months through demonstration, documentation and seemingly impossible levels of progress (webcomponents + elmsln make application development trivial) I'll begin to show the path towards anyone building an NGDLE. What it provides users, How we are sharing things across institutions and systems, and how we can start to dissolve all learning systems into the NGDLE based worldview to provide better solutions for instructors and more engaging learning spaces online for learners.
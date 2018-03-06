---
title: 'HAX apereo piece'
---

Once you see HAX, and realize how it works, you won't be able to unsee it.

What is HAX? HAX is short for Headless Authoring eXperience; meaning that we've decoupled the authoring of content and media from any backend storage system. This frees us to build the best authoring solution for the web. Not specifically for ELMS:LN, or Sakai, or Tsugi but for the web in general. HAX does this through a front-end technology called web components.

Web components have been in the pipeline of the web for many years, but the time is finally right to start jumping on board and planning for how to use them in the future. Web components in short are a four part specification already in most browsers fully (or polyfill-ed in) which allows for the creation of new, custom html tags that the browser recognizes. This nets you modular / component driven development without the need for bloated frameworks like Angular, React, etc.

HAX leverages this technology to build a form of web components authoring web components. This means that we can build new custom elements that any browser understands, and have it fire up a single JSON object and IF hax is around it will understand how to build a UI for it. HAX based content will never appear to have been made with HAX, because it's just writing data into web component properties the same way any developer could.

This means faculty can start authoring advanced HTML without ever looking at it. It also means we as developers can build and expand our systems using open standards without frameworks limiting who can plug and play where. The #usetheplatform movement is lively and is ultimately the replacement for all frameworks or at least huge chunks of them while allowing us to share visual and functional assets.

Interested in helping us #haxtheweb? Check out some links:

* http://haxtheweb.org - this is a demo which is completely headless
* https://github.com/LRNWebComponents - our open element library, currently north of 130 elements that work anywhere
* https://www.youtube.com/playlist?list=PLJQupiji7J5eTqv8JFiW8SZpSeKouZACH - #haxtheweb playlist of tutorials, demonstrations, and ramblings

This is an effort that can benefit any Apereo project and the ELMS:LN core team would happily entertain collaborations to help bring HAX to more than just ELMS:LN's community. Currently there are HAX integrations for Drupal (6,7), BackdropCMS, GravCMS and ELMS:LN. HAX is slated to be the default authoring experience for ELMS:LN by Fall 2018 with pilot to real people happening Summer 2018.

*[this piece was originally written for the Apereo newsletter](https://www.apereo.org/)
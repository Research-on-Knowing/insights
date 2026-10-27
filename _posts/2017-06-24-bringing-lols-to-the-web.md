---
layout: post
title: "Bringing LoLs to the Web: JavaScript, OMetaJS, and the Web Workbench"
author: jamie
date: 2017-06-24 09:00:00 -0700
categories: [Project, Language of Languages]
image: assets/images/language-of-languages-4-workbench-card.png
imagelic: "Pieter Bruegel the Elder, The Tower of Babel (Rotterdam), via Google Art Project and Wikimedia Commons"
imagelicref: "https://commons.wikimedia.org/wiki/File:Pieter_Bruegel_the_Elder_-_The_Tower_of_Babel_(Rotterdam)_-_Google_Art_Project_-_edited.jpg"
excerpt: "Squeak Smalltalk was ideal for prototyping but hard to adopt. We moved the LoLs workbench into the browser with JavaScript and OMetaJS."
series: language-of-languages
series_part: 4
---

<div class="series-note" style="font-style:italic;color:#6c757d;margin-bottom:1.5rem">Part 4 in the Language of Languages series.</div>


While Squeak Smalltalk was instrumental for rapid prototyping, it presented adoption hurdles: Smalltalk was less common in university curricula, and requiring users to download a Squeak image created high friction. To make LoLs broadly accessible, we migrated the core workbench to run natively in web browsers using JavaScript and OMetaJS.

Moving to a browser-native stack eliminated setup barriers, allowing developers to experiment with custom parsers, context checkers, and projectors directly in their browser.

## Try the workbench and explore the code

- **Interactive tool:** [Open the Workbench](https://jamiedouglass.github.io/LanguageWorkbench/) to launch the web environment.
- **OMetaJS engine:** Source code for our OMetaJS adaptation is in the [LoLsOMetaJS repository](https://github.com/jamiedouglass/LoLsOMetaJS) on GitHub.
- **Browser workbench:** The user interface and language environment are in the [LanguageWorkbench repository](https://github.com/jamiedouglass/LanguageWorkbench) on GitHub.

*Next in the series: [Expanding LoLs Capabilities: The JNode Environment and LoLsServer]({{ site.baseurl }}{% post_url 2020-08-07-jnode-environment-and-lols-server %}).*

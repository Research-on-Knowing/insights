---
layout: post
title: "Under the Hood: Building the First LoLs Prototype in Squeak Smalltalk & OMeta"
author: jamie
date: 2010-11-05 09:00:00 -0700
categories: [Project, Language of Languages]
image: assets/images/language-of-languages-2-prototype-card.png
imagelic: "Pieter Bruegel the Elder, The Tower of Babel (Rotterdam), via Google Art Project and Wikimedia Commons"
imagelicref: "https://commons.wikimedia.org/wiki/File:Pieter_Bruegel_the_Elder_-_The_Tower_of_Babel_(Rotterdam)_-_Google_Art_Project_-_edited.jpg"
excerpt: "The first Language of Languages prototype was built in Squeak Smalltalk with OMeta. Here is the minimalist architecture behind it."
series: language-of-languages
series_part: 2
---

<div class="series-note" style="font-style:italic;color:#6c757d;margin-bottom:1.5rem">Part 2 in the Language of Languages series.</div>


To validate the core principles of Language of Languages, we built our initial bootstrap environment inside Squeak Smalltalk using OMeta pattern-matching extensions.

Smalltalk provided an ideal foundation for rapid language experimentation due to its live environment and metacircularity, which allows LoLs to be defined and explored in terms of itself. To support graphical notations alongside textual syntax, we leveraged Squeak’s Morphic graphics system.

## The core architecture

Every notation in LoLs is supported through a minimalist paradigm composed of three primary building blocks:

- **Language Elements and Element Trees:** Structural representations where every token or graphical shape has a corresponding node.
- **Concepts:** Notation-agnostic semantic anchors (for example, an Addition concept) that bind across representations.
- **Language Definitions:** Operational bindings for a Concept that implement three fundamental operations:
    - **Parsing:** Recognizing textual or graphical constructs (using OMeta) to build a Language Element Tree.
    - **Context checking:** Validating whether a definition applies in the current context.
    - **Projecting:** Transforming or interpreting the tree into executable values, alternative text, or Morphic graphical shapes.

This Smalltalk and OMeta prototype proved that complex DSLs, mathematical expressions, and graphical state machines could map back to shared underlying concepts.

*Next in the series: [Language of Languages at SPLASH 2011]({{ site.baseurl }}{% post_url 2011-11-02-language-of-languages-at-splash-2011 %}).*

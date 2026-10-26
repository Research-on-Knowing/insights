---
layout: post
title: "Why We Built Language of Languages: Bridging the Multi-Notation Gap in System Design"
author: jamie
date: 2008-11-20 09:00:00 -0800
categories: [Project, Language of Languages]
image: assets/images/language-of-languages-1-why-lols-card.png
imagelic: "Pieter Bruegel the Elder, The Tower of Babel (Rotterdam), via Google Art Project and Wikimedia Commons"
imagelicref: "https://commons.wikimedia.org/wiki/File:Pieter_Bruegel_the_Elder_-_The_Tower_of_Babel_(Rotterdam)_-_Google_Art_Project_-_edited.jpg"
excerpt: "Large systems are described in many notations at once. Language of Languages began as a way to keep them consistent and understandable."
featured_order: 3
series: language-of-languages
series_part: 1
---

<div class="series-note" style="font-style:italic;color:#6c757d;margin-bottom:1.5rem">Part 1 in the Language of Languages series.</div>


In large-scale system and software engineering, project teams rarely rely on a single notation. Systems architects model structural behaviors in AADL or SysML, software engineers write application code in C++, Java, or VHDL, and domain specialists design state machines and control logic.

While using specialized notations allows developers to choose the most expressive tool for the task, it introduces two major challenges:

- **Communication:** Ensuring different stakeholders understand the intent across distinct notations.
- **Correctness and consistency:** Verifying that disparate representations remain consistent with one another as the system evolves.

The Language of Languages (LoLs) project was conceived to address this fragmentation. Rather than forcing all disciplines into a single monolithic model or writing fragile N x M translators, LoLs adopts a language-agnostic view.

By decoupling underlying domain Concepts (such as State, Action, or Addition) from their concrete Language Definitions (textual, numerical, or graphical), LoLs unifies different representations under a shared Language Element Tree. This concept-centric integration enables early and continuous Virtual Integration, a core principle of initiatives like System Architecture Virtual Integration (SAVI), allowing teams to detect interface mismatches promptly and lower system lifecycle costs.

*Next in the series: [Under the Hood: Building the First LoLs Prototype in Squeak Smalltalk and OMeta]({{ site.baseurl }}{% post_url 2010-11-05-building-first-lols-prototype-squeak-ometa %}).*

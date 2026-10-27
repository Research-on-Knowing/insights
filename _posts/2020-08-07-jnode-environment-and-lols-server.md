---
layout: post
title: "Expanding LoLs Capabilities: The JNode Environment & LoLsServer Architecture"
author: jamie
date: 2020-08-07 09:00:00 -0700
categories: [Project, Language of Languages]
image: assets/images/language-of-languages-5-lols-server-card.png
imagelic: "Pieter Bruegel the Elder, The Tower of Babel (Rotterdam), via Google Art Project and Wikimedia Commons"
imagelicref: "https://commons.wikimedia.org/wiki/File:Pieter_Bruegel_the_Elder_-_The_Tower_of_Babel_(Rotterdam)_-_Google_Art_Project_-_edited.jpg"
excerpt: "To support larger models, LoLs grew into a multi-component architecture with JNode execution and a dedicated server backend."
series: language-of-languages
series_part: 5
---

<div class="series-note" style="font-style:italic;color:#6c757d;margin-bottom:1.5rem">Part 5 in the Language of Languages series.</div>


To support larger models, server-side processing, and decoupled execution environments, the Language of Languages project evolved into a multi-component runtime architecture featuring JNode execution and a dedicated server backend.

This architectural shift decoupled the browser-based editor interface from language processing and concept evaluation services:

- **LoLs Workbench frontend:** Handles projection, user interaction, and layout parsing.
- **LoLs Server backend:** Evaluates server-side projections, manages multi-file concept dependencies, and executes language transformations across distributed nodes.

## Repositories

- **Client and node runtime:** [LoLsWorkbench repository](https://github.com/jamiedouglass/LoLsWorkbench) on GitHub.
- **Backend service:** [LoLsServer repository](https://github.com/jamiedouglass/LoLsServer) on GitHub.

*Next in the series: [Project Retrospective and Archived Resources]({{ site.baseurl }}{% post_url 2024-09-25-lols-retrospective-and-archive %}).*

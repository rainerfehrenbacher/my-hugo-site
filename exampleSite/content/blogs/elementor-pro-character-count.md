---
title: "Dynamic Character Counts on Elementor Forms"
date: 2023-07-18T12:53:58+05:30
draft: true
author: "Rainer Fehrenbacher"
tags:
  - Elementor
  - Forms
  - JavaScript
  - WordPress
image: /images/mastodon.png
description: "A quick explanation of how to add max character limits and dynamic character counts for a textarea field on Elementor Pro"
---
# Background
I recently came across an issue with a client site where it became necessary to migrate one of their forms from NinjaForms to an Elementor Pro Form. Take this with a grain of salt because it came from a NF support tech who provided very sub-par service, but NinjaForms has a lot of trouble implementing reCaptcha v3 on sites that also run Elementor Pro. Apparently the Elementor Pro plugin runs the code for the v3 reCaptcha on every page (even when reCaptcha has not been set up in the Elementor settings). This creates a conflict with any other plugin that wants to add a reCaptcha v3 field (in this case, NinjaForms).

Long story short - I tried to add reCaptcha v2 to our site with the assistance of NF support and we ended up just switching our site over to Elementor Pro Forms. It was a frustrating experience, but I think it is going to save us a lot of headache down the road.
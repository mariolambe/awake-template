---
title: Getting Started
subtitle: Get Up and Running with Awake
category:
  - category-1
  - category-3
author: Daniel Kelly
date: 2019-07-23T19:59:59.000Z
featureImage: /uploads/getting-started-hero.jpg
---
Awake is a Nuxt.js template for generating a beautifully robust static site with blog in as few steps as possible. 

# Features

* Simple modern design based on the Bulma css framework (with unused css purged via [purgecss](https://www.purgecss.com/))
* Site search
* Statically generated API for posts and categories
* Disqus powered comments
* Mailchimp powered newsletter
* Highly customizable with out of the box configurations
* Built with performance in mind
* Isolated Netlify CMS driver (with more CMS drivers planned for future) for easily migrating between various headless cms'
* Feature images automatically given srcsets and resized

Deploy to Netlify Button Here

# Configuration

Site configuration is found in `/config/_siteConfig.js`. Here you can customize site settings such as the site name, layout, disqus and mailchimp setup, image sizes and more. 

# Editing Content

Posts and categories can be edited in Netlify CMS at \[your-site-url]/admin. At this time any new pages must be created in the code itself and committed to the repo

# Local Development

Since all content is store in the git repo with Netlify CMS, local development is a breeze. Simply install node, pull down the repo, and run `npm run dev`.
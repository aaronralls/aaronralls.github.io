---
layout: post
title: How to start a blog for free
summary: "Learn how you can get a hosted blog for free"
image: /assets/images/20190110/header.jpg
twitter_image: /assets/images/20190110/twitter-image.jpg
facebook_link_image: /assets/images/20190110/facebook-link-image.jpg
date: 2019-01-10 02:34:24.000000000 -05:00
type: post
parent_id: '0'
published: true
password: ''
status: publish
categories:
- GitHub
- Blog
tags:
- GitHub
- Blog
image_sliders:
  - sliderCreateGitHubAccount
excerpt: |-
  Start a free blog to share your experiences with the world.

  You can do this for free thanks to GitHub!
permalink: '/:year/:month/:day/:title'
---

## How do I get my Free Blog

There are a couple of options for getting your own hosted blog site up and running.

- [WordPress.com][WordPressPlansLink] Free plan
- [GitHub Pages][GitHubPAgesLink]

If you are still not sure why you should start blogging see my [5 reasons post][5ReasonsPost].

Wait! Is this going to be all technical?

Yes this will get technical and if this is not comfortable for you then I would recommend going with the WordPress.com free site.

You can always move from the WordPress site to the GitHub Page blog as I did.

Before you ultimately decide, let me ask you a couple of questions.

Are you working as a developer or aspire to become one?

Or are you working in any technical computer job or even with a technical team?

If yes then I highly recommend the GitHub Pages option as it will expose you to some tools and process you should start to get familiar with.

In this post I will cover how to start a blog for free using GitHub Pages. Before I jump into that I will provide you with some basic information on the WordPress option I mentioned.

## WordPress

To be clear there are two distinct WordPress sites, [WordPress.com][WordPressCOMLink] and [WordPress.org][WordPressOrgLink] site. The latter is home of the open source software and would require you to find a place to host the site like [GoDaddy.com][GoDaddyLink]

On the [WordPress.com][WordPressCOMLink] you may create a free blog that you can later upgrade to paid versions with more functionality. This is where I originally started.

If you want to learn more about the differences between the WordPress sites [here][WordPressComparisonLink] is a good article.

So if you don't want to deal with anything more technical than absolutely necessary than this will work just fine.

## GitHub Pages

[GitHub Pages][GitHubPAgesLink] are a free hosting service that is provided by [GitHub][GitHubLink] for Git repositories hosted on their site.

This has a little more complexity to setup and will be worth the time.

Great, but what is GitHub, and what is a Git repository?

These are great questions! Lets go over some basics.

If you already are familiar with these then [jump](#create-github-account) to were all the action starts!

## What is Git

So lets start with Git, which is a tool to version control files. These can be any type of files. The great thing about this tool is the ability to work in a distributed fashion. What this means is that you can work on your project and keep track of all changes on your own computer and synch them back to a remote location, like the GitHub website.

When you work with your files you keep them in a repository for safe keeping.

There is a lot you can dive into with Git and you only need the basics to use GitHub Pages. If you want to learn more check out Git and version control check out this [site][GitTrainingLink].

## What is GitHub

GitHub is a company that provides services for managing Git repositories. The features that you will need are all free.

You can read this older [article][GitHubMakeMoneyLink] on how they make their money and are able to offer these free services.

Many IT Professionals and Open Source Projects use GitHub free repositories to share their work.

## Tell me about these GitHub Pages

[GitHub Pages][WhatIsGitHubPages] is a website hosting service that you can use for an individual, organization, or project where the content is maintained in a public Git repository on the GitHub site.

The only limitation is that the site is a static site which means there will be no code running on the web server. The only code that can work is what the web browser would be able to run.

Great so what type of code can it work with? Wait do I have to know how to write code too??

Ah don't worry you will not have to learn how to code to get your site up and running. You can copy what I have or another theme and just update some settings like your name and start blogging!

## Let's do this

Great you have made it this far and decided to go with the GitHub pages!

Here is what we will cover to get your blog up and running.

- Create a GitHub Account
- Setup the GitHub repository
- Verify the Blog is up and running
- Update Blog settings

### Create GitHub account

Follow the steps in the images below to create your GitHub account.

{% include slider.html selector="sliderCreateGitHubAccount" %}

### Setup the GitHub repository

In this step you will copy a repository with the blog site code. This will allow you to change the settings and start your blog quickly.

To get a working copy we are going to fork a repository I created that has the [blog][BlogRepository] code ready to go.

### Verify the Blog is up and running

Now that we have copied the repository lets make sure it works from the get go.

### Update Blog settings

These are the things you will need to change to complete the minimal setup.

For simplicity we will make these changes from the GitHub web page vs a code editor.

I will cover how you can work with your blog on your local computer in another post.

- Name and Website in Policy Page
- Favorite icon
- About Page
- First Post
- Main config file _config.yml
  - Title
  - Name
  - Repository
  - URL
  - Production URL
  - GitHub Username

## Parting Thoughts - Blog Away

Great now you have a cool and free blog!

Your next step is to plan your next blog post. Set a deadline and time to work on it!

Stay tuned for the next step on how you can add a custom domain name.

[5ReasonsPost]: {% post_url 2019-01-07-5-reasons-to-start-blogging %}  "5 Reasons you should Blog!"
[GitHubLink]: https://Github.com "GitHub site"
[GitHubPAgesLink]: https://pages.Github.com "GitHub Pages site"
[WhatIsGitHubPages]: https://help.github.com/articles/what-is-github-pages/ "What is GitHub Pages?"
[GitTrainingLink]: https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control "Git Training"
[101Start]: #Create-GitHub-account "Create GitHub account internal link"
[101NoDomainStart]: #GitHub-Setup "GitHub Setup internal link"
[GitHubMakeMoneyLink]: https://www.cnbc.com/2017/10/11/github-has-a-110-million-run-rate-from-business-products.html "How Does GitHub make money?"
[WordPressOrgLink]: https://wordpress.org "WordPress.org site"
[WordPressPlansLink]: https://wordpress.com/pricing/ "WordPress.com plans and pricing link"
[GitHubPageDependencies]: https://pages.github.com/versions/ "GitHub Page Dependencies"
[RubyWinInstaller]: https://rubyinstaller.org/downloads "Ruby Windows Installer"
[Jekyll374Dependencies]: https://rubygems.org/gems/jekyll/versions/3.7.4 "Jekyll 3.7.4 Dependencies"
[GitHubPagesJekyll38Issue]:https://github.com/github/pages-gem/issues/555 "GitHub Pages Jekyll 3.8 Issue"
[VerifyDNS]: https://centralops.net/co/ "Verify DNS Tool"
[GitHubLocalSetup]: https://help.github.com/articles/setting-up-your-github-pages-site-locally-with-jekyll/ "GitHub Pages locally with Jekyll"
[GitHubFlavoredMarkdownRef]: https://github.com/adam-p/markdown-here/wiki/Markdown-Here-Cheatsheet "GitHub Flavored Markdown (GFD) Cheat sheet"
[KramdownRef]: https://kramdown.gettalong.org/syntax.html "Kramdown Reference"
[OverrideThemeDefaults]: https://jekyllrb.com/docs/themes/#overriding-theme-defaults "Override Theme Defaults"
[GoDaddyLink]: https://www.godaddy.com/hosting/wordpress-hosting "GoDaddy WordPress Hosting"
[WordPressCOMLink]: https://wordpress.com/ "WordPress main site"
[WordPressComparisonLink]:https://www.wpbeginner.com/beginners-guide/why-is-wordpress-free-what-are-the-costs-what-is-the-catch/ "WordPress.org vs. WordPress.com"
[BlogRepository]: https://github.com/aaronralls/Blog "Blog Repository"

---
layout: post
redirect_from:
   - /2019/01/13/how-to-add-custom-domain-github-pages-blog/
title: How to add Custom Domain to GitHub Pages Blog
slug: how-to-add-custom-domain
summary: "How to add Custom Domain to GitHub Pages Blog"
image: /assets/images/20190113/header.jpg
twitter_image: /assets/images/20190113/twitter-image.jpg
facebook_link_image: /assets/images/20190113/facebook-link-image.jpg
date: 2019-01-13 02:34:24.000000000 -05:00
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
  - sliderVerifyGitHubBlog
excerpt: |-
  We will add a custom domain to your GitHub Pages blog.

permalink: '/github-pages/:slug'
---

# How to add Custom Domain to GitHub Pages Blog

You decided to go with the [GitHub pages][GitHubPagesLink] for your blog and now you want to start writing your first post about some cool new technology you just learned about.

You can't wait to share it with your friends and followers on Twitter, LinkedIn, Medium, and Facebook.

Then it hits you, the current domain name you have is underwhelming. In the [previous post][HowToStartBlogForFree], we set up the site with the default repository name.

{% include note.html content="The default domain name will be <b><i>GitHubUserName</i>.github.io</b>." %}

You think to yourself I'm a professional I don't want to share it like that!

So you run out and get your super awesome domain name from [GoDaddy][GoDaddyLink] for .99¢ and are stumped as to how you get it working with your new blog.

You have come to the right spot because I will walk you through the steps to add your custom domain to your GitHub Pages Blog site.

## Let's do this

Now it's time to give your site that professional look.

This will be a quick process to complete!

- Configure DNS settings for a custom domain
- Update the Blog settings
- Update the _config.yml file
- Verify the Blog is using the custom domain

### Configure DNS settings

You need to go to the company that you bought the domain name from and change the DNS settings.

Since the admin pages will look different from other providers you may need to find the help documentation on their site.

This is what the GoDaddy DNS Management page looks like when it is all configured.

![DNS Settings][DNSSettings]

Here is how you will create each of the A records. When making DNS changes it could take as long as 24 hours for them to be established.

{% include important.html content="Set the TTL time value to 300 seconds." %}

{% include note.html content="Notice how the <b><i>Host</i></b> value will be the <b><i>Name</i></b> value once it is saved." %}

![DNS Record][DNSRecord]

Make sure there is the CNAME record to allow users to reach your site when they use the **_www_** domain prefix.

![DNS CNAME Record][DNSCNAMERecord]

### Update Blog settings

This step is crazy simple!

Go to the settings tab for the repository and enter in your Custom domain name.

Then click the Save button.

{% include note.html content="When you save the settings the site will run the build process." %}

![Repository Settings Tab][RepoSettingsTab]

### Update the _config.yml

In the main configuration file, __config.yml_, you have to update the *url* and *prod_url* values.

![_config.yml changes][configYML]

### Verify the Blog

You will want to make sure the blog built successfully before trying to load it in a browser.

{% include slider.html selector="sliderVerifyGitHubBlog" %}

## Parting Thoughts - Commit to Content

Now that you have the custom domain added to your GitHub pages blog you are ready to confidently share your site with everyone you know!

Sharing your goals with others is a great way to help hold yourself accountable. The fact that you told your friends and family what you plan on doing you will be more likely to follow through.

Set a day each week to write one blog post. Get in a routine for a couple of months, then try to increase how many you are writing a week.

[HowToStartBlogForFree]: {% post_url 2019-01-10-how-to-start-a-blog-for-free %}  "How to start a blog for free"
[5ReasonsPost]: {% post_url 2019-01-07-5-reasons-to-start-blogging %}  "5 Reasons you should Blog!"
[GitHubPagesLink]: https://pages.Github.com "GitHub Pages site"
[VerifyDNS]: https://centralops.net/co/ "Verify DNS Tool"
[GoDaddyLink]: https://www.godaddy.com/hosting/wordpress-hosting "GoDaddy WordPress Hosting"
[RepoSettingsTab]: /assets/images/20190113/reposettingstab.PNG "GitHub Repository Settings Tab"
[DNSSettings]: /assets/images/20190113/DNSSettings.PNG "DNS Settings"
[DNSRecord]: /assets/images/20190113/DNSRecord.PNG "DNS Record"
[DNSCNAMERecord]: /assets/images/20190113/DNSCNAMERecord.PNG "DNS CNAME Record"
[configYML]: /assets/images/20190113/configYML.PNG "_config.yml changes"
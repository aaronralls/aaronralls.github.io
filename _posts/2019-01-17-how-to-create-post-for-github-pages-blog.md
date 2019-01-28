---
layout: post
title: "How do I work this Github blog?"
slug: 5-steps-to-publish-blog-post
summary: "5 Steps to Publish Github Blog Post"
excerpt: 
  You have your Github Pages blog post content ready to go, but aren't sure how to put that in your site. Follow these steps to get your post live!
image: /assets/images/20190117/header.jpg
twitter_image: /assets/images/20190117/twitter-image.jpg
facebook_link_image: /assets/images/20190117/facebook-link-image.jpg
date: 2019-01-17 02:34:24.000000000 -05:00
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
related_posts:
- how-to-start-a-blog-for-free
- 5-reasons-to-start-blogging
#image_sliders:
#  - sliderVerifyGitHubBlog
permalink: '/github-pages/:slug'
---

# 5 Steps to Publish a GitHub Pages Blog Post

You have your post content written and reviewed by a friend.

Now you are thinking "Great, where do I put this information?".

That is understandable!

You put all that time into your post and you want to make sure you're doing it the correct way.

In this post I will show you where everything goes that you created.

Be sure that you read my [previous][StepsCreateBlogPost] post on what you needed to create.

## Let's do this

Here are the items you will be updating.

- [Save Artwork](#artwork)
    - Original
    - Optimized
- [Front Matter Variables](#front-matter-variables)
    - Categories and Tags
    - URL and Slug
    - Blog Excerpt
    - Related Posts
    - Title
    - Image Locations
- [Markdown Content](#markdown-content)
    - Main Heading
    - Introduction
    - Body
    - Call to Action

Then we will wrap up by validating the new post by checking for the following:

- [Readability and Spelling](#check-readability-and-spelling-again)
- [Page Loading Speed](#page-loading-speed)

## Artwork

Create new folders, one for the originals and one for the optimized content.

In my template I use the following folders.

- assets/images/20190117
- assets_original/images/20190117

Where the date is the date of the post publish date. This works for me since I have yet to have more than one post on a given date.

All files under the *__assets__* folder are part of the website.

Any files in the *__assets_original__* folder will not get published to the website. You want to keep them separate to preserve the original size and content.

## Front Matter Variables

Start with a new post template file to create new post markdown file. In this post we will use one that is dependent on the theme I previewed in a previous post.

What are font matter variables?

Here is the front matter from my template.

{% highlight markdown %}
{% raw %}
---
layout: post
title: "How do I work this Github blog?"
slug: 10-steps-to-publish-blog-post
summary: "10 Steps to Publish Github Blog Post"
excerpt:
  You have your Github Pages blog post content ready to go, what's next?
image: /assets/images/20190117/header.jpg
twitter_image: /assets/images/20190117/twitter-image.jpg
facebook_link_image: /assets/images/20190117/facebook-link-image.jpg
date: 2019-01-17 02:34:24.000000000 -05:00
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
related_posts:
- how-to-start-a-blog-for-free
- 5-reasons-to-start-blogging
permalink: '/github-pages/:slug'
---
{% endraw %}
{% endhighlight %}

The front matter variables that are specific to this theme.

- related_posts
- twitter_image
- facebook_link_image
- slug

### Categories and Tags

The Categories and Tags will go into their own collection list.

{% highlight markdown %}
{% raw %}
categories:
- GitHub
- Blog
tags:
- GitHub
- Blog
{% endraw %}
{% endhighlight %}

### Slug

The Slug will be assigned to the matching *__slug__* variable.

{% highlight markdown %}
{% raw %}
slug: 10-steps-to-publish-blog-post
{% endraw %}
{% endhighlight %}

The URL that you planned out should include the full path including the slug. 

For this blog post the URL is *__websitename/github-pages/10-steps-to-publish-blog-post__*.

Here are some examples:

*websitename/category1/slug*

*websitename/category1/category2/slug*

*websitename/slug*

I chose to only use one category when deciding on my final URL. There is a strategy to creating the URL that impacts the SEO of the post. I like to make sure my URL does not double up on keywords.

You will update the *__permalink__* variable to include the category list you want.

{% highlight markdown %}
{% raw %}
permalink: '/github-pages/:slug'
{% endraw %}
{% endhighlight %}

### Blog Excerpt

The excerpt that you would like to show on this site and externally will go with the *__excerpt__* variable.

{% highlight markdown %}
{% raw %}
excerpt: You have your Github Pages blog post content ready to go, what's next?
{% endraw %}
{% endhighlight %}

### Related Posts

The featured.html template will show related posts below the main post content. List out the slug(s) from the posts that you want shown with the *__related_posts__* variable.

{% highlight markdown %}
{% raw %}
related_posts:
- how-to-start-a-blog-for-free #This is the slug of the post that will be linked
- 5-reasons-to-start-blogging
{% endraw %}
{% endhighlight %}

### Title

The title of the blog will be assigned to the matching *__title__* variable. Be sure to put your title in double quotes.

{% highlight markdown %}
{% raw %}
title: "How do I work this Github blog?"
{% endraw %}
{% endhighlight %}

### Image Locations

The following variables will state the location of the optimized images.

*__image:__*

This is the main image that will be used at the top of the post.

{% highlight markdown %}
{% raw %}
image: /assets/images/20190117/header.jpg
{% endraw %}
{% endhighlight %}

*__twitter_image:__*

This is used by the twitter_card.html template to have information in the required Twitter format.

{% highlight markdown %}
{% raw %}
twitter_image: /assets/images/20190117/twitter-image.jpg
{% endraw %}
{% endhighlight %}

*__facebook_link_image:__*

This is used by the open-graph.html template to populate content used by Facebook.

{% highlight markdown %}
{% raw %}
facebook_link_image: /assets/images/20190117/facebook-link-image.jpg
{% endraw %}
{% endhighlight %}

## Markdown Content

In this step you will put the blog post material in the area below the front matter variables.

This where you put the introduction, body and the call to action.

I prefer to keep all images and links that I use in a post at the bottom and use markdown references in the main content.

### Insert Images

Image defined at the bottom.

{% highlight markdown %}
{% raw %}
[SampleSearchEngineResults]: /assets/images/20190115/search-results.JPG "sample search engine result"
{% endraw %}
{% endhighlight %}

{% highlight markdown %}
{% raw %}
![][SampleSearchEngineResults]

Some text related to the Image used in the main content.
{% endraw %}
{% endhighlight %}

### Insert External Links

External Link defined at the bottom.

{% highlight markdown %}
{% raw %}
[BlogPostInspiration]: https://somelink.com "something"
{% endraw %}
{% endhighlight %}

External Link used in the main content.

{% highlight markdown %}
{% raw %}
Some external [link][BlogPostInspiration] related to the Image used in the main content.
{% endraw %}
{% endhighlight %}

### Insert Internal Links

Internal Link defined at the bottom.

{% highlight markdown %}
{% raw %}
[BlogOtherSites]: {% post_url 2019-01-08-how-to-blog-without-a-blog %} "How to blog without a blog"
{% endraw %}
{% endhighlight %}

{% highlight markdown %}
{% raw %}
Some internal [post link][BlogOtherSites] related to the Image used in the main content.
{% endraw %}
{% endhighlight %}

{% include important.html content="Save and check each image and link in the post." %}

## Check Readability and Spelling AGAIN

Now that you have published the new post to your site, open it up in a browser to make sure it looks good.

The easiest way to do this is to use the [Hemingway][Hemingwayapp] website. Copy the post content from your web browser screen and paste it in the Hemingway website. It will show you misspelled words and sentences that are too complex.

## Page Loading Speed

Use the Google [PageSpeed Insights][PageSpeedTool] tool to make sure there are no issues.

Since you are using a static website the score should be close to 90 or above.

## Parting Thoughts - Share Your Work

In a future post I will show you how to set up your computer to test new posts locally.

Now that you have a good format and process for publishing your posts, go out and share them!

Share them on Twitter, Facebook. Email it out to friends. Ask for feedback and continue to improve!

Be sure you read my [post][AddCustomDomainGitHubPages] on how to add a custom domain to your Github pages blog!

[HowToStartBlogForFree]: {% post_url 2019-01-10-how-to-start-a-blog-for-free %}  "How to start a blog for free"
[AddCustomDomainGitHubPages]: {% post_url 2019-01-13-how-to-add-custom-domain-github-pages-blog %} "How to add Custom Domain to GitHub Pages Blog"
[5ReasonsPost]: {% post_url 2019-01-07-5-reasons-to-start-blogging %}  "5 Reasons you should Blog!"
[FreeBlog]: {% post_url 2019-01-10-how-to-start-a-blog-for-free %} "Free Blog"
[BlogOtherSites]: {% post_url 2019-01-08-how-to-blog-without-a-blog %} "How to blog without a blog"
[StepsCreateBlogPost]: {% post_url 2019-01-15-10-steps-to-create-blog-post %} "10 Steps to Create a Successful Blog Post"
[CreatePostForGithubPages]: {% post_url 2019-01-17-how-to-create-post-for-github-pages-blog %} "10 Steps to Publish Github Blog Post"

[Hemingwayapp]: http://www.hemingwayapp.com/ "Hemingwayapp site to check readability"
[CharacterCountTool]: https://www.lettercount.com/ "Website tool to count character"
[PageSpeedTool]: https://developers.google.com/speed/pagespeed/insights/ "Google PageSpeed Insights tool"
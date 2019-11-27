---
layout: post
title: "What is new in Azure: Episode 3"
slug: what-is-new-in-azure-episode-3
summary: "What is new in Azure: Episode 3"
excerpt: 
  Stay up to date with Azure and see what's new for the week of 12/04/2019!
image: /assets/images/20191204/header.jpg
twitter_image: /assets/images/20191204/twitter-image.jpg
facebook_link_image: /assets/images/20191204/facebook-link-image.jpg
date: 2019-12-04 02:34:24.000000000 -05:00
type: post
parent_id: '0'
published: true
password: ''
status: publish
categories:
- Azure
tags:
- Azure
related_posts:
- what-is-new-in-azure-episode-1
- what-is-new-in-azure-episode-2
#image_sliders:
#  - sliderVerifyGitHubBlog
permalink: '/azure/updates/:slug'
---

# What is new in Azure: Episode 3

Welcome to my second post in this new weekly blog series to help you stay up to date with Azure!

If you want to get the background on my rating system please read the intro in [Episode1][AzureUpdatesEpisode1Post]

I won't cover every single update, just those I feel will benefit the largest possible audience.

This Episode will cover changes going back to 11-27-2019.

To learn more about me, be sure that you read my [post][StepsCreateBlogPost] on why I started blogging.

## Let's do this

Here are the updates I will cover.

- [Live transcription with Azure Media Services](#live-transcription-with-azure-media-services)

## Live transcription with Azure Media Services

[announcement][AzureMediaServicesLiveTranscriptionAnnouncement]

The new [Change feed][ChangeFeedAnnouncement] feature is in preview and will provide a read-only log that will allow you to see all the actions that have taken place to the blobs.

If you are new to [Azure Blob Storage][AzureBlobStorage] be sure to read up on how versatile they can be.

*__Why is this a big deal?__*

![Rating 7 of 10][Rating7of10]

I give this update 7/10 Astronauts because Azure Blob storage is a commonly used asset and by allowing you to tie the log changes to event-driven applications can be a game changer compared to what is available today.

Previously I built an [Azure Logic App][AzureLogicApps] that would run every 10 minutes to see if a new blob was saved to a container using the [Azure Blob Storage Connector][AzureBlobStorageConnectorDocs]. An alternative would be to have the [blob storage events][BlobStorageEventsDocs] pass through [Azure Event Grid][AzureEventGridDocs] and then consume them via an [Azure Function][MicrosoftDocsAzureFunctions].

With this new feature you can update this process to audit all of the changes and/or to process the changes in the order.

## Parting Thoughts - Read, Read, Read

![Reading Image][ReadingImage]
*Photo by [Peter Lawrence][ReadingPhotoCredit] on [Unsplash][UnsplashLink]*

I used to hate to read.

In high school we had books we had to read, well I was supposed to read them.

They were dreadful titles like ["Wuthering Heights"][WutheringHeightsWiki].

That turned me off on reading until I was in the US NAVY, stuck on an air craft carrier in the middle of the ocean with nothing to do.

I picked up a friends book and found I liked to read.

Fast forward to the start of my IT career...I realized I enjoyed to read because I liked to learn more and reading was an efficient way for me to do so.

I would read books on COM like the ["Essential COM"][EssentialCOMbook] book by [Don Box][DonBoxWiki] and try to understand every detail like I was staring at a beautiful painting trying to take in all its meaning.

My eagerness to read has helped me keep up with the never ending changes in IT.

So find some time each day to read something.

A blog post *wink wink*, software documentation, learning material like [Microsoft Learn][MicrosoftLearnSite], a fictional novel.

Just be sure to Read, Read, Read!

Be sure you read my [Episode #1][AzureUpdatesEpisode1Post] post on previous Azure updates!

[HowToStartBlogForFree]: {% post_url 2019-01-10-how-to-start-a-blog-for-free %}  "How to start a blog for free"
[AddCustomDomainGitHubPages]: {% post_url 2019-01-13-how-to-add-custom-domain-github-pages-blog %} "How to add Custom Domain to GitHub Pages Blog"
[5ReasonsPost]: {% post_url 2019-01-07-5-reasons-to-start-blogging %}  "5 Reasons you should Blog!"
[FreeBlog]: {% post_url 2019-01-10-how-to-start-a-blog-for-free %} "Free Blog"
[BlogOtherSites]: {% post_url 2019-01-08-how-to-blog-without-a-blog %} "How to blog without a blog"
[StepsCreateBlogPost]: {% post_url 2019-01-15-10-steps-to-create-blog-post %} "10 Steps to Create a Successful Blog Post"
[CreatePostForGithubPages]: {% post_url 2019-01-17-how-to-create-post-for-github-pages-blog %} "10 Steps to Publish Github Blog Post"
[AzureUpdatesEpisode1Post]: {% post_url 2019-11-21-What-is-new-in-Azure-this-week %} "Azure Updates: Episode 1"
[AzureUpdatesEpisode2Post]: {% post_url 2019-11-27-What-is-new-in-Azure-this-week %} "Azure Updates: Episode 2"

[Rating1of10]: /assets/images/templates/astronaut-rating-1-of-10.png "Rating 1 of 10 Astronauts"
[Rating2of10]: /assets/images/templates/astronaut-rating-2-of-10.png "Rating 2 of 10 Astronauts"
[Rating3of10]: /assets/images/templates/astronaut-rating-3-of-10.png "Rating 3 of 10 Astronauts"
[Rating4of10]: /assets/images/templates/astronaut-rating-4-of-10.png "Rating 4 of 10 Astronauts"
[Rating5of10]: /assets/images/templates/astronaut-rating-5-of-10.png "Rating 5 of 10 Astronauts"
[Rating6of10]: /assets/images/templates/astronaut-rating-6-of-10.png "Rating 6 of 10 Astronauts"
[Rating7of10]: /assets/images/templates/astronaut-rating-7-of-10.png "Rating 7 of 10 Astronauts"
[Rating8of10]: /assets/images/templates/astronaut-rating-8-of-10.png "Rating 8 of 10 Astronauts"
[Rating9of10]: /assets/images/templates/astronaut-rating-9-of-10.png "Rating 9 of 10 Astronauts"
[Rating10of10]: /assets/images/templates/astronaut-rating-10-of-10.png "Rating 10 of 10 Astronauts"

[UnsplashLink]: https://unsplash.com/ "Unsplash"
[ReadingPhotoCredit]: https://unsplash.com/@chesterfordhouse "Peter Lawrence Photo Credit"
[ReadingImage]: /assets/images/20191127/peter-lawrence-people-reading-on-subway-unsplash.jpg "People Reading on subway Photo by Peter Lawrence"

[AzureMediaServicesLiveTranscriptionAnnouncement]: https://azure.microsoft.com/en-us/blog/preview-live-transcription-with-azure-media-services/ "AzureMedia ServicesLive Transcription"

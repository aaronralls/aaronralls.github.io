---
layout: post
title: "What is new in Azure: Episode 2"
slug: what-is-new-in-azure-episode-2
summary: "What is new in Azure: Episode 2"
excerpt: 
  Stay up to date with Azure and see what's new for the week of 11/27/2019!
image: /assets/images/20191127/header.jpg
twitter_image: /assets/images/20191127/twitter-image.jpg
facebook_link_image: /assets/images/20191127/facebook-link-image.jpg
date: 2019-11-27 02:34:24.000000000 -05:00
type: post
parent_id: '0'
published: true
password: ''
status: publish
categories:
- Azure
- DevOps
- Azure Blob Storage
- Blob Storage Events
- Azure Functions
- Azure Event Grid
- Azure Logic Apps
- Azure Dedicated Host
- Azure Service Tags
- Network security group
- Azure HDInsight
- Azure Service Health
- Azure Migrate
- Azure SQL Database Metrics
- Azure Monitor
- Azure Metrics Explorer
tags:
- Azure
- DevOps
- Azure Blob Storage
- Blob Storage Events
- Azure Functions
- Azure Event Grid
- Azure Logic Apps
- Azure Dedicated Host
- Azure Service Tags
- Network security group
- Azure HDInsight
- Azure Service Health
- Azure Migrate
- Azure SQL Database Metrics
- Azure Monitor
- Azure Metrics Explorer
related_posts:
- how-to-start-a-blog-for-free
- what-is-new-in-azure-episode-1
#image_sliders:
#  - sliderVerifyGitHubBlog
permalink: '/azure/updates/:slug'
---

# What is new in Azure: Episode 2

Welcome to my second post in this new weekly blog series to help you stay up to date with Azure!

If you want to get the background on my rating system please read the intro in [Episode 1][AzureUpdatesEpisode1Post]

I won't cover every single update, just those I feel will benefit the largest possible audience.

This Episode will cover changes going back to 11-21-2019.

To learn more about me, be sure that you read my [post][StepsCreateBlogPost] on why I started blogging.

## Let's do this

Here are the updates I will cover.

- [Change feed for Azure Blob Storage](#change-feed-for-azure-blob-storage)
- [Azure Virtual Machines Isolation Changes D15 and DS15 v2](#azure-virtual-machines-isolation-changes-d15-and-ds15-v2)
- [Azure HDInsight Create NSG rules with service tags](#azure-hdinsight-create-nsg-rules-with-service-tags)
- [AzureDB Service Health Notifications](#azure-db-service-health-notifications)
- [Azure Migrate Assess Servers from CSV file](#azure-migrate-assess-servers-from-csv-file)
- [Azure Backup extended support](#azure-backup-extended-support)
- [Azure Data Lake Updates](#azure-data-lake-updates)

## Change feed for Azure Blob Storage

The new [Change feed][ChangeFeedAnnouncement] feature is in preview and will provide a read-only log that will allow you to see all the actions that have taken place to the blobs.

If you are new to [Azure Blob Storage][AzureBlobStorage] be sure to read up on how versatile they can be.

*__Why is this a big deal?__*

![Rating 7 of 10][Rating7of10]

I give this update 7/10 Astronauts because Azure Blob storage is a commonly used asset and by allowing you to tie the log changes to event-driven applications can be a game-changer compared to what is available today.

Previously I built an [Azure Logic App][AzureLogicApps] that would run every 10 minutes to see if a new blob was saved to a container using the [Azure Blob Storage Connector][AzureBlobStorageConnectorDocs]. An alternative would be to have the [blob storage events][BlobStorageEventsDocs] pass through [Azure Event Grid][AzureEventGridDocs] and then consume them via an [Azure Function][MicrosoftDocsAzureFunctions].

With this new feature, you can update this process to audit all of the changes and/or to process the changes in the order.

## Azure Virtual Machines Isolation Changes D15 and DS15 v2

As of Feb 15, 2020, the D15_v2 and DS15_v2 Linux Virtual Machines may no longer be isolated. Read the [Announcement][AzureD15DS15NoLongerIsolatedAnnouncement] specific details.

*__Why is this a big deal?__*

![Rating 4 of 10][Rating4of10]

I give this update 4/10 Astronauts because the isolated instances are being replaced with a new service [Azure Dedicated Host][AzureDedicatedHostPreviewAnnouncement]. All of the details on this service can be [read here][AzureD15IsolationQandA].

## Azure HDInsight Create NSG rules with service tags

You can now use [Azure Service Tags][AzureServiceTags] to manage inbound [network security group (NSG)][AzureNSGDocs] rules for [Azure HDInsight][AzureHDInsightDocs].

Here is the official [announcement][AzureHDInsighServiceTagAnnouncement].

*__Why is this a big deal?__*

![Rating 8 of 10][Rating8of10]

I give this update 8/10 Astronauts because improving the usability of implementing and managing security if important.

Second, [Azure HDInsight][AzureHDInsightDocs] is where you would be running data processes like extracts, transformations, and a data warehouse.

Protecting your data and your customers is critical.

So go learn the nitty-gritty on [Service Tags][AzureServiceTags] and [Azure Service Tags For HDInsight][AzureServiceTagsForHDInsightDocumentation]!

## Azure DB Service Health Notifications

The major update here is that the following database offerings now support [Azure Service Health][AzureServiceHealthDocs] notifications for planned maintenance.

- [MariaDB Announcement][AzureDBforMariaDBServiceHealthAnnouncement]
- [MySQL Announcement][AzureDBforMySQLServiceHealthAnnouncement]
- [PostgreSQL Announcement][AzureDBforPostgreSQLServiceHealthAnnouncement]

*__Why is this a big deal?__*

![Rating 7 of 10][Rating7of10]

I give this update 7/10 Astronauts because monitoring your databases is critical and easily the one component that can take your product offline and cause you to miss some SLA's.

## Azure Migrate Assess Servers from CSV file

It was [announced][AzureMigrateAssessCSVAnnouncement] that [Azure Migrate][AzureMigrateDocs] will allow you to start and migration assessment with a CSV file of servers.

*__Why is this a big deal?__*

![Rating 8 of 10][Rating8of10]

I give this update 8/10 Astronauts because many companies don't want to install an agent on production servers to evaluate an Azure Migration.

They already have inventories in spreadsheets or in a [Configuration Management Database][CMDBWiki] so this makes it a no-brainer first step to evaluate moving to Azure.

Here are the [steps][AzureMigrateAssessDocumentation] to use a CSV file.

## Azure Backup extended support

We have two announcements for new features related to Azure backups!

First, we have new [backup metrics][AzureBackupSupportSQLServer2019AVM] for Azure SQL Database.

With [Azure Metrics Explorer][AzureMetricsExplorerDocs] you can now see events related to Full, Differential, and Log backups.

Second, and the more important [announcement][AzureBackupSQLAsFiles], is support for Azure Backup for more versions of SQL and Windows Server in Virtual Machines

- SQL Server 2008 & 2008 R2
- SQL Server 2019
- Windows Server 2019

Along with....

"INSERT DRUM ROLL"

The ability to restore SQL databases as files to on-premises or other Azure subscriptions!

Restore as files anywhere!!

*__Why is this a big deal?__*

![Rating 9 of 10][Rating9of10]

I give this update 9/10 Astronauts because these changes are HUGE!

Monitoring database backups are important and most people don't think to look at them or their status until a production issue comes up. This will help you keep a tab on them proactively.

See the documentation for a complete list of [Azure SQL Database Metrics][AzureSQLDBMetricsDocs] you may monitor with [Azure Metrics Explorer][AzureMetricsExplorerDocs].

The second part I mentioned about adding more SQL and Windows versions to [Azure backup][SQLServerBackupInVMDocumentation] is nice, the real beauty is the ability to restore as files!

This will give you more flexibility to manage your database recovery processes.

I know this is really three announcements, but they made sense to cover as one topic.

## Azure Data Lake updates

Azure Data Lake Storage [announced][AzureDataLakeUpdatesAnnouncement] the ability of multi-protocol access, allowing the access of data on Azure Blobs via the Azure Blob Storage API.

This allows for new Azure Service Integrations with Data Lake

- Azure Stream Analytics
- IoT Hub
- Azure Event Hubs Capture
- Azure Data Box
- Azure Logic Apps

*__Why is this a big deal?__*

![Rating 7 of 10][Rating7of10]

I give this update 7/10 Astronauts because of the added capability of using other Azure services to take real-time action.

A bonus addition is that they are now allowing customers to have data on different tiers, hot and cool, to reduce costs.

You should read up on the [Data Lake Multi Protocol Access Docs][DataLakeMultiProtocolAccessDocs].

## Parting Thoughts - Read, Read, Read

![Reading Image][ReadingImage]
*Photo by [Peter Lawrence][ReadingPhotoCredit] on [Unsplash][UnsplashLink]*

I used to hate to read.

In high school, we had books we had to read, well I was supposed to read them.

They were dreadful titles like ["Wuthering Heights"][WutheringHeightsWiki].

That turned me off on reading until I was in the US NAVY, stuck on an aircraft carrier in the middle of the ocean with nothing to do.

I picked up a friend's book and found I liked to read.

Fast forward to the start of my IT career...I realized I enjoyed to read because I liked to learn more and reading was an efficient way for me to do so.

I would read books on COM like the ["Essential COM"][EssentialCOMbook] book by [Don Box][DonBoxWiki] and try to understand every detail like I was staring at a beautiful painting trying to take in all its meaning.

My eagerness to read has helped me keep up with the never-ending changes in IT.

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

[AzureBlobStorage]: https://docs.microsoft.com/en-us/azure/storage/blobs/storage-blobs-introduction "Azure Blob Storage documentation"
[ChangeFeedAnnouncement]: https://azure.microsoft.com/en-us/blog/change-feed-support-now-available-in-preview-for-azure-blob-storage/ "Change feed for Azure Blob Storage Announcement"
[AzureBlobStorageConnectorDocs]: https://docs.microsoft.com/en-us/connectors/azureblob/ "Azure Blob Storage Connector Docs"
[AzureLogicApps]: https://azure.microsoft.com/en-us/services/logic-apps/ "Azure Logic Apps"
[AzureEventGridDocs]: https://docs.microsoft.com/en-us/azure/event-grid/overview "Azure Event Grid Docs"
[MicrosoftDocsAzureFunctions]: https://docs.microsoft.com/en-us/azure/azure-functions/ "Microsoft Docs Azure Functions"
[BlobStorageEventsDocs]: https://docs.microsoft.com/en-us/azure/storage/blobs/storage-blob-event-overview "[Blob Storage Events Docs]"

[AzureD15DS15NoLongerIsolatedAnnouncement]: https://azure.microsoft.com/en-us/updates/the-d15-v2-ds15-v2-azure-virtual-machines-may-no-longer-be-isolated-starting-february-15-2020/ "Azure VM D15 and DS15 no longer isolated"
[AzureDedicatedHostPreviewAnnouncement]: https://azure.microsoft.com/en-us/blog/introducing-azure-dedicated-host/ "Azure Dedicated Host"
[AzureD15IsolationQandA]: https://docs.microsoft.com/en-us/azure/virtual-machines/linux/isolation#retiring-d15_v2ds15_v2-isolation-on-february-15-2020

[AzureHDInsighServiceTagAnnouncement]: https://azure.microsoft.com/en-us/updates/simplify-nsg-rules-management-for-azure-hdinsight-using-service-tags/ "Azure HDInsight Create NSG rules with service tags"
[AzureServiceTags]: https://docs.microsoft.com/en-us/azure/virtual-network/security-overview#service-tags "Azure Service Tags"
[AzureServiceTagsForHDInsightDocumentation]: https://docs.microsoft.com/en-us/azure/hdinsight/hdinsight-service-tags "Azure Service Tags For HDInsight Documentation"
[AzureHDInsightDocs]: https://docs.microsoft.com/en-us/azure/hdinsight/hdinsight-overview "Azure HDInsight Docs"
[AzureNSGDocs]: https://docs.microsoft.com/en-us/azure/virtual-network/security-overview "AZure Network Security Group Docs"

[AzureDBForMariaDBDocumentation]: https://docs.microsoft.com/en-us/azure/mariadb/ "Azure Database for MariaDB documentation"
[AzureServiceHealthDocumentation]: https://docs.microsoft.com/en-us/azure/service-health/overview "Azure Service Health documentation"
[MonitorMariaDBServiceHealthDocs]: https://docs.microsoft.com/en-us/azure/mariadb/concepts-monitoring#service-health "Monitor MariaDB Service Health"
[AzureDBforMariaDBServiceHealthAnnouncement]: https://azure.microsoft.com/en-us/updates/azure-database-for-mariadb-support-for-service-health-notifications-for-planned-maintenance-is-now-in-preview-in-east-us-and/ "Azure DB for MariaDB Service Health Announcement"
[MariaDBSite]: https://mariadb.org/about/ "MariaDB website"
[AzureDBforMySQLServiceHealthAnnouncement]: https://azure.microsoft.com/en-us/updates/azure-database-for-mysql-support-for-creating-activity-log-alerts-for-service-health-notification-is-now-in-preview/ "AzureDB for MySQL Service Health Announcement"
[AzureDBforPostgreSQLServiceHealthAnnouncement]: https://azure.microsoft.com/en-us/updates/azure-database-for-postgresql-single-server-support-for-service-health-notifications-for-planned-maintenance-is-now-in-previe/ "AzureDB for PostgreSQL Service Health Announcement"
[AzureServiceHealthDocs]: https://docs.microsoft.com/en-us/azure/service-health/overview "Azure Service Health Docs"

[AzureMigrateAssessCSVAnnouncement]: https://azure.microsoft.com/en-us/updates/assessment-of-imported-servers-now-supported-in-preview/ "Azure Migrate Assess CSV Announcement"
[AzureMigrateAssessDocumentation]: https://docs.microsoft.com/en-us/azure/migrate/tutorial-assess-import "Azure Migrate Assess Documentation"
[CMDBWiki]: https://en.wikipedia.org/wiki/Configuration_management_database "Configuration management database wiki"
[AzureMigrateDocs]: https://docs.microsoft.com/en-us/azure/migrate/migrate-services-overview "Azure Migrate Docs"

[AzureSQLDBBackupMetricsAnnouncement]: https://azure.microsoft.com/en-us/updates/new-azure-sql-database-backup-storage-metrics-are-now-generally-available/ "Azure SQL DB Backup Metrics Announcement"
[AzureMetricsExplorerDocs]: https://docs.microsoft.com/en-us/azure/azure-monitor/platform/metrics-charts "Azure Metrics Explorer Documentation"
[AzureSQLDBMetrics]: https://docs.microsoft.com/en-us/azure/azure-monitor/platform/metrics-supported#microsoftsqlserversdatabases "Azure SQL DB Metrics"
[AzureSQLDBMetricsDocs]: https://docs.microsoft.com/en-us/azure/azure-monitor/platform/metrics-supported#microsoftsqlserversdatabases "Azure SQL DB Metrics Docs"
[AzureBackupSQLAsFiles]: https://azure.microsoft.com/en-us/blog/azure-backup-support-for-sql-server-2019-and-restore-as-files/ "Azure Backup SQL as Files"

[AzureBackupSupportSQLServer2019AVM]:https://azure.microsoft.com/en-us/blog/azure-backup-support-for-sql-server-2019-and-restore-as-files/ "Azure Backup Support SQL Server 2019 AVM"
[SQLServerBackupInVMDocumentation]: https://docs.microsoft.com/en-us/azure/backup/backup-azure-sql-database "SQL Server Backup In VM Documentation"

[VideoIndexerMultiLanguageSupportAnnouncement]: https://azure.microsoft.com/en-us/blog/multi-language-identification-and-transcription-in-video-indexer/ "Video Indexer Multi-Language Support Announcement"
[VideoIndexerWebsite]: https://vi.microsoft.com/ "Video Indexer website"
[VideoIndexerDocumentation]: https://docs.microsoft.com/en-us/azure/media-services/video-indexer/video-indexer-overview "Video Indexer Documentation"
[VideoIndexerOverview]: https://azure.microsoft.com/en-us/services/media-services/video-indexer/ "Video Indexer Overview"

[AzureDataLakeUpdatesAnnouncement]: https://azure.microsoft.com/en-us/blog/multi-protocol-access-on-data-lake-storage-now-generally-available/ "AzureDataLakeUpdatesAnnouncement"
[DataLakeMultiProtocolAccessDocs]: https://docs.microsoft.com/en-us/azure/storage/blobs/data-lake-storage-multi-protocol-access "Data Lake Multi Protocol Access Docs"

[WutheringHeightsWiki]: https://en.wikipedia.org/wiki/Wuthering_Heights "Wuthering Heights Wiki"
[DonBoxWiki]: https://en.wikipedia.org/wiki/Don_Box "Don Box Wiki"
[EssentialCOMbook]: https://www.goodreads.com/book/show/919597.Essential_Com "Essential COM book by Don Box"
[MicrosoftLearnSite]: https://docs.microsoft.com/en-us/learn/ "Microsoft Learn website"

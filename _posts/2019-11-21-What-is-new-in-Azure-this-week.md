---
layout: post
title: "What is new in Azure: Episode 1"
slug: What-is-new-in-Azure-episode-1
summary: "What is new in Azure: Episode 1"
excerpt: 
  You have your Github Pages blog post content ready to go, but aren't sure how to put that in your site. Follow these steps to get your post live!
image: /assets/images/20191121/header.jpg
twitter_image: /assets/images/20191121/twitter-image.jpg
facebook_link_image: /assets/images/20191121/facebook-link-image.jpg
date: 2019-11-21 02:34:24.000000000 -05:00
type: post
parent_id: '0'
published: true
password: ''
status: publish
categories:
- Azure
- DevOps
- Kubernetes
- Azure Functions
- Azure Cognitive Services
- Spring Cloud
tags:
- Azure
- DevOps
- Kubernetes
- Azure Functions
- Azure Cognitive Services
- Spring Cloud
related_posts:
- how-to-start-a-blog-for-free
- 5-reasons-to-start-blogging
#image_sliders:
#  - sliderVerifyGitHubBlog
permalink: '/azure/updates/:slug'
---

# What is new in Azure: Episode 1

Welcome to my new weekly blog series to help you stay up to date with Azure!

I will scour the "interwebs" for the best updates and changes related to Azure.

I won't cover every single update, just those I feel will benefit the largest possible audience.

For the first Episode I will cover changes going back to Microsoft Ignite 2019.

To learn more about me be sure that you read my [previous][StepsCreateBlogPost] post on why I started blogging.

## Let's do this

Here are the updates I will cover.

- [Microsoft Secure Code Analysis toolkit](#microsoft-secure-code-analysis-toolkit)
- [Training for Azure DevOps Engineer Expert (Exam AZ-400)](#training-for-azure-devops-engineer-expert-exam-az-400)
- [Training for Azure Functions](#training-for-azure-functions)
- [Cognitive Services Updates](#cognitive-services-updates)
- [Kubernetes based event-driven auto scaling (KEDA) 1.0 release](#kubernetes-based-event-driven-auto-scaling-keda-1-release)
- [Azure Arc](#azure-arc)
- [Azure Firewall Manager](#azure-firewall-manager)
- [Azure Bastion](#azure-bastion)
- [Azure Security Center Updates](#azure-security-center-updates)
- [Azure Spring Cloud](#azure-spring-cloud)

## Microsoft Secure Code Analysis toolkit

While the [Secure Code Analysis toolkit][MicrosoftSecurityCodeAnalysis] is not new, it was just added to [Microsoft Unified Support][MicrosoftUnifiedSupport].

The toolkit is an extension that can be added to Azure DevOps CI/CD pipelines that consists of Microsoft-managed tools and open-source tools.

With this extension you can run Anti-Malware scanner, credential scanner, and other static code analyzers.

*__Why is this a big deal?__*

![Rating 5 of 10][Rating5of10]

I give this update 5/10 Astronauts because it's an existing tool that has been brought into the Microsoft Unified Support model.

Microsoft Unified Support is the new support model that is replacing the Microsoft Premier Support program that was [announced in 2017][MicrosoftUnifiedSupportAnnouncement].

By adding the Secure Code Analysis toolkit to the support program you should be able to get better help from Microsoft resources.

## Training for Azure DevOps Engineer Expert Exam AZ-400

Microsoft added content on their learning site for [Azure DevOps Training][AzureDevOpsLearningPath] for the [AZ-400 exam][ExamAZ-400] that you may use to achieve the [Microsoft Certified: Azure DevOps Engineer Expert][AzureDevOpsEngineerExpertCertification] title.

*__Why is this a big deal?__*

![Rating 6 of 10][Rating6of10]

I give this update 6/10 Astronauts because free training is awesome! I can't give it any more Astronauts because there are no sample exam questions and it's not one of the more marketable exams like the AZ-300, AZ-301 or other Azure exams. Additionally, there is other free training that is out on [OpenEDX.com][OpenEDXAZ-400] and [Azure DevOps Labs website][AzureDevOpsLabsSite].

[Azure DevOps][AzureDevOps] is great product that allows you to manage you code with repositories, your projects with agile tools like Azure Boards, CI/CD pipelines, and so many more features. This training allows you to get up to speed and aware of what the product can do for you, without having to do any setup.

Lastly, my good friend [Gregor Suttie][GregorSuttieTwitter] has a good [blog post][GregorSuttieAZ-400StudyNotesPost] of study material for this exam.

## Training for Azure Functions

[Azure Functions][MicrosoftLearnAzureFunctions] are a great tool that has grown in popularity. Microsoft has released a new Learning module on Azure Functions to help you get up to speed on them.

*__Why is this a big deal?__*

![Rating 5 of 10][Rating5of10]

I give this update a 5/10 Astronauts because the material is free, but it's not a comprehensive course.

Once again free training is a plus. If you are just learning about Azure or have applications running in Azure you need to have Azure Functions on your learning radar. Additionally, if you are preparing for the Azure certifications you will need to review Azure Functions.

For more free training resources on Azure Functions see the Microsoft Docs [website][MicrosoftDocsAzureFunctions].

Another way you may be able to learn more about [Azure Functions][AzureFunctionsTwitter] is the upcoming 25 days of [serverless challenges][AzureFunctions25DaysOfServerless] in December! #25DaysOFServerless

## Cognitive Services Updates

[Azure Cognitive Services][AzureCognitiveServices] allows you to utilize Artificial Intellegence (AI) in your applications with ease.

Some of the services allow you to analyze language, speech, vision, and decision making API's such as the [Content Moderator][AzureCognitiveServicesContentModerator].

Azure Cognitive Search has new data connectors for other services like Azure Logic Apps, new AI skills, and available in more regions.

[Personalizer][AzureCognitiveServicesPersonalizer] is a new service that will allow you to prioritize relevant content with customer interactions to create customized interactions.

Speech services has, in preview, the ability to use custom voices with humanlike voices.

[Text Analytics][CognitiveServicesTextAnalytics] are now able to identify personally identifiable information in documents.

There is a new [Bot Framework Composer][CognitiveServicesBotFrameworkComposer] to make it easier to create bots without having to use raw code. The user interface reminds me of the Azure [Log Apps tools][AzureLogicApps].

*__Why is this a big deal?__*

![Rating 8 of 10][Rating8of10]

I have to give this 8/10 Astronauts due to the expansion of the Text Analytics to recognize personally identifiable information. Data security is critical and have another tool to help manage that data is critical. Then the addition of the Bot Framework Composer will allow people to start tinkering with bots and leveraging them in more of their products.

## Kubernetes based event-driven auto scaling KEDA 1 release

What is KEDA? Well here is an excerpt from their [documentation][KEDAGitHub].

"KEDA allows for fine grained auto scaling (including to/from zero) for event driven Kubernetes workloads. KEDA serves as a Kubernetes Metrics Server and allows users to define auto scaling rules using a dedicated Kubernetes custom resource definition."

*__Why is this a big deal?__*

![Rating 8 of 10][Rating8of10]

I give this 8/10 Astronauts since it adds a new ways to allow you to scale your Kubernetes containers beyond the CPU and memory metrics.

To learn more check out the [announcement][KEDAAnnouncement].

## Azure Arc

Microsoft [announced][AzureArcAnnouncement] Azure Arc at Ignite 2019 and described it as:

"a set of technologies that unlocks new hybrid scenarios for customers by bringing Azure services and management to any infrastructure."

This will allow customers to manage the portfolio of cloud assets with a common tool set, Azure Resource Manager, Microsoft Azure Cloud Shell, Azure portal, and Microsoft Azure Policy.

*__Why is this a big deal?__*

![Rating 10 of 10][Rating10of10]

This is a game changer and is 10/10 Astronauts! This will allow you to create an Azure SQL Database in your data center using the Microsoft Azure Cloud Shell and manage it via the Azure Portal.

Another scenario is that you will be able to manage your Amazon EC2 and VMware vSphere VM's via the [Azure Resource Manager][AzureResourceManager] (ARM).

Azure Arc will allow you to manage [Azure Stack Hub][AzureStack], formally Azure Stack, and the new [Azure Stack Edge][AzureStackEdge] as well.

More services will be added so stay tuned!

## Azure Firewall Manager

The new [Azure Firewall Manger][AzureFirewallManager] is in public preview and will allow you to mange all of your [Azure Fire Walls][AzureFireWall] in one place.

*__Why is this a big deal?__*

![Rating 4 of 10][Rating4of10]

I will give this 4/10 Astronauts because while being a good new offering it has some issues and is just in public preview, meaning it's not ready for production.

I will revisit this as the product matures.

## Azure Bastion

[Azure Bastion][AzureBastion] is a new PaaS offering that allows you to RDP and SSH to VM via the Azure Portal.

*__Why is this a big deal?__*

![Rating 8 of 10][Rating8of10]

I will give this 8/10 Astronauts because improving your security is important and this product allows you to do away with jump boxes.

## Azure Security Center Updates

[Azure Security Center][AzureSecurityCenter] provides you a way to better manage your infrastructure, regardless of location.

At Ignite 2019 they rolled out some new features.

*__Why is this a big deal?__*

![Rating 6 of 10][Rating6of10]

I will give this 6/10 Astronauts because they added the ability to created automated configurations using [Azure Logic Apps][AzureLogicApps].

Another great addition is the ability to perform an action on a large set of resources using the [Quick Fix][AzureSecurityCenterQuickFix] action.

Other updates included:

- [Regulatory Compliance dashboard][AzureSecurityCenterRegulatoryComplianceDashboard] 
- [Scanning of container Images][AzureSecurityCenterScanContainers]
- [Threat protection for Azure Kubernetes Service][AzureSecurityCenterThreatProtectionAKS]
- [Custom Policies][AzureSecurityCenterCustomPolicies]
- [Advanced Integrations][AzureSecurityCenterAdvancedIntegrations]

## Azure Spring Cloud

[Azure Spring Cloud][AzureSpringCloud] provides a quick way for Spring developers to launch applications that rely on [Spring Cloud][SpringCloud] in a fully managed environment.

*__Why is this a big deal?__*

![Rating 6 of 10][Rating6of10]

I have to give this 6/10 Astronauts since Azure is the only public cloud provider that offers this fully managed environment for Spring Cloud.

## Parting Thoughts - Let me be your branch

![Tree Image][TreeImage]
*Photo by [Faye Cornish][FayeCornsihPhotoCredit] on [Unsplash][UnsplashLink]*

There will always be a constant fire hose of new information in the IT industry.

I like to pride myself on knowing where to go to get the details I need when I need them.

I think about it like a tree, you only have to worry about the big branches and not all of the leaves.

This way I don't have to worry about keeping all of the small details in my brain.

Most people can't memorize everything they read. So try to work smarter!

I hope I can become a branch on your tree of knowledge to help you in your career!

Be sure you read my [post][FreeBlog] on how you can get a free blog!

[HowToStartBlogForFree]: {% post_url 2019-01-10-how-to-start-a-blog-for-free %}  "How to start a blog for free"
[AddCustomDomainGitHubPages]: {% post_url 2019-01-13-how-to-add-custom-domain-github-pages-blog %} "How to add Custom Domain to GitHub Pages Blog"
[5ReasonsPost]: {% post_url 2019-01-07-5-reasons-to-start-blogging %}  "5 Reasons you should Blog!"
[FreeBlog]: {% post_url 2019-01-10-how-to-start-a-blog-for-free %} "Free Blog"
[BlogOtherSites]: {% post_url 2019-01-08-how-to-blog-without-a-blog %} "How to blog without a blog"
[StepsCreateBlogPost]: {% post_url 2019-01-15-10-steps-to-create-blog-post %} "10 Steps to Create a Successful Blog Post"
[CreatePostForGithubPages]: {% post_url 2019-01-17-how-to-create-post-for-github-pages-blog %} "10 Steps to Publish Github Blog Post"

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
[FayeCornsihPhotoCredit]: https://unsplash.com/@fcornish "Faye Cornsih Photo Credit"
[TreeImage]: /assets/images/20191121/faye-cornish-tree-unsplash.jpg "Tree Photo by Faye Cornish"

[MicrosoftSecurityCodeAnalysis]: https://docs.microsoft.com/en-us/azure/security/develop/security-code-analysis-overview "About Microsoft Security Code Analysis"
[MicrosoftUnifiedSupport]: https://www.microsoft.com/en-us/enterprise/services/unified-support-solutions "Microsoft Unified Support"
[MicrosoftUnifiedSupportAnnouncement]: https://redmondmag.com/articles/2017/08/25/microsoft-unified-support-program.aspx "Microsoft Unified Support Announcement"
[AzureDevOpsLearningPath]: https://docs.microsoft.com/en-us/learn/paths/evolve-your-devops-practices/ "Azure DevOps Learning Path for Exam AZ-400"
[AzureDevOpsEngineerExpertCertification]: https://docs.microsoft.com/en-us/learn/certifications/azure-devops "Microsoft Certified: Azure DevOps Engineer Expert AZ-400"
[ExamAZ-400]: https://docs.microsoft.com/en-us/learn/certifications/exams/az-400 "Exam AZ-400: Microsoft Azure DevOps Solutions"
[AzureDevOpsLabsSite]: https://azuredevopslabs.com/ "Azure DevOps Labs website"
[OpenEDXAZ-400]: https://openedx.microsoft.com/courses/course-v1:Microsoft+AZ-400.1+2019_T1/about "Azure DevOps Training on OpenEDX website"
[GregorSuttieAZ-400StudyNotesPost]: https://gregorsuttie.com/2018/10/27/azure-devops-az-400-exam-study-notes/ "Gregor Suitte AZ-400 Study Notes"
[GregorSuttieTwitter]: https://twitter.com/gregor_suttie "Gregor Suttie Twitter"
[AzureDevOps]: https://azure.microsoft.com/en-us/services/devops/ "Azure DevOps"
[MicrosoftLearnAzureFunctions]: https://docs.microsoft.com/en-us/learn/modules/develop-test-deploy-azure-functions-with-core-tools/ "Microsoft Learn Azure Functions"
[MicrosoftDocsAzureFunctions]: https://docs.microsoft.com/en-us/azure/azure-functions/ "Microsoft Docs Azure Functions"
[AzureFunctions25DaysOfServerless]: https://dev.to/azure/merry-and-bright-with-azure-advocates-25-days-of-serverless-1hi0 "Azure Functions 25 days of serverless"
[AzureFunctionsTwitter]: https://twitter.com/AzureFunctions "Azure Functions Twitter"
[AzureCognitiveServicesUpdates]: https://venturebeat.com/2019/11/04/azure-cognitive-services-gets-speech-search-language-and-security-updates-at-ignite-2019/ "Azure Cognitive Services Updates"
[AzureCognitiveServices]: https://azure.microsoft.com/en-us/services/cognitive-services/ "Azure Cognitive Services"
[AzureCognitiveServicesContentModerator]: https://azure.microsoft.com/en-us/services/cognitive-services/content-moderator/ "Azure Cognitive Services Content Moderator"
[AzureCognitiveServicesPersonalizer]: https://azure.microsoft.com/en-us/services/cognitive-services/personalizer/ "Azure Cognitive Services Personalizer"
[CognitiveServicesTextAnalytics]: https://azure.microsoft.com/en-us/services/cognitive-services/text-analytics/ "Azure Cognitive Services Text Analytics"
[CognitiveServicesBotFrameworkComposer]: https://github.com/microsoft/BotFramework-Composer/blob/stable/README.md "Azure Bot Framework Composer"
[CognitiveServicesBotFramework]:https://azure.microsoft.com/en-us/services/bot-service/ "Cognitive Services Bot Framework"
[AzureLogicApps]: https://azure.microsoft.com/en-us/services/logic-apps/ "Azure Logic Apps"
[KEDAAnnouncement]: https://cloudblogs.microsoft.com/opensource/2019/11/19/keda-1-0-release-kubernetes-based-event-driven-autoscaling/ "Kubernetes-based event-driven auto scaling (KEDA) 1.0 release"
[KEDAGitHub]: https://github.com/kedacore/keda "KEDA Github location"
[AzureArcAnnouncement]: https://azure.microsoft.com/en-us/blog/azure-services-now-run-anywhere-with-new-hybrid-capabilities-announcing-azure-arc/ "Azure Arc Announcement"
[AzureStack]: https://azure.microsoft.com/en-us/overview/azure-stack/ "Azure Stack"
[AzureStackEdge]: https://azure.microsoft.com/en-us/overview/azure-stack/ "Azure Stack Edge"
[AzureResourceManager]: https://docs.microsoft.com/en-us/azure/azure-resource-manager/resource-group-overview "Azure Resource Manager"
[AzureFirewallManager]: https://azure.microsoft.com/en-us/services/firewall-manager/ "Azure Firewall Manager"
[AzureFireWall]: https://azure.microsoft.com/en-us/services/azure-firewall/ "Azure Fire Wall"
[AzureBastion]: https://azure.microsoft.com/en-us/services/azure-bastion/ "Azure Bastion"
[AzureSecurityCenter]: https://azure.microsoft.com/en-us/services/security-center/ "Azure Security Center"
[AzureSecurityCenterQuickFix]: https://azure.microsoft.com/en-us/updates/azure-security-center-quick-fix-for-bulk-resources-generally-available/ "Azure Security Center Quick Fix"
[AzureSecurityCenterRegulatoryComplianceDashboard]: https://azure.microsoft.com/en-us/updates/additional-regulatory-compliance-standards-in-azure-security-center/ "Azure Security Center Regulatory Compliance dashboard"
[AzureSecurityCenterScanContainers]: https://azure.microsoft.com/en-us/updates/scan-container-images-for-vulnerabilities-in-azure-security-center/ "Azure Security Center Scan Container Images"
[AzureSecurityCenterThreatProtectionAKS]: https://azure.microsoft.com/en-us/updates/threat-protection-for-azure-kubernetes-service-aks-support-in-security-center/ "AzureSecurity Center Threat Protection AKS"
[AzureSecurityCenterCustomPolicies]: https://azure.microsoft.com/en-us/updates/azure-security-center-support-for-custom-policies/ "Azure Security Center Custom Policies"
[AzureSecurityCenterAdvancedIntegrations]: https://azure.microsoft.com/en-us/updates/azure-security-center-advanced-integrations-with-export-of-recommendations-and-alerts/ "Azure Security Center Advanced Integrations"
[AzureSpringCloud]: https://azure.microsoft.com/en-us/services/spring-cloud/ "Azure Spring Cloud"
[SpringCloud]: https://spring.io/projects/spring-cloud "Spring Cloud"

# Plot

To provide a lifecycle of the solution it is required to have certain tools which are responsible for different areas.  
In general there are 2 options of getting this tools:

*   Option A - to assemble from different tools from different vendors.
*   Option M - to get a pack, so called Solution Lifecycle Management package from one vendor.

It’s like you need a car to ride and you can go to Mercedes store and buy one or you can get to a market buy separate parts and assemble one.

Following document tries to describe in detail pros and cons of both approaches.

First of all let's take a look at possible options:

*   Option **A - A**tlassian based, because it is takes **at least 3 different products** from Atlassian.
*   Option **M - M**S VSTS because it is just **only 1 product** from Microsoft named Visual Studio Team Services.

## Compare by aspects

Following table compares options by different aspects

| | Area | Option A | | Option M | |
|:---|:---|:---|:---|:---|:---|
| 1 | Payment and Cost |- Purchases from each vendor of each service are separate.<br/>- **Separate invoices** at the end of the month.<br/>- Total **cost** of ownership is **greater** than all-in-one solutions.| - |All services are purchased from one vendor as pack.<br/>- **One invoice** at the end of the month.<br/>- Total **cost** of ownership is **less** than separate systems.| + |
| 2 | Legal | It is required to accept **different policies** from **each vendor**. | - | It is required to accept **one policy** from **only one vendor**. | + |
| 3 | Security & Compliance | [Atlassian has achieved following certificates for some cloud services:](https://www.atlassian.com/trust/compliance)<br/>- **[GDPR (on May 25 2018)](https://www.atlassian.com/blog/announcements/atlassian-and-gdpr-our-commitment-to-data-privacy)**<br/>- ISO 27001<br/>- SOC 2 Type 1<br/>- CSA STAR Level 1|-| [Microsoft has achieved following list of certificates for VSTS:](https://docs.microsoft.com/en-us/vsts/articles/team-services-security-whitepaper)<br/>- **GDPR (on May 25 2018) **<br/>-  ISO 27001:2013<br/>-  HIPAA (Health Insurance Portability and Accountability Act)<br/>-  BAA (Business Associate Agreement)<br/>-  EU Model Clauses<br/>-  SOC 1 Type 2 and SOC 2 Type 2| + |
| 4 | Identity & Access Management | Requires **separate** management of each user for each system.  Integration of some products with Identity Service is available for **additional cost.** | - | VSTS **out of the box** provide integration with the Azure Active Directory which can be connected with on-premises Active Directory. | + |
| 5 | Service Management | While most of the services are managed (hosted in the cloud) some services like Jenkins **requires additional infrastructure**, setup and provision. | - | VSTS is **completely managed** service. | + |
| 6 | [Requirements Traceability](https://en.wikipedia.org/wiki/Requirements_traceability) | **Requires purchase** of additional plugins. | - | Provided **out of the box.** | + |
| 7 | IDE | **Requires additional** plugins. | - | Provides **out of the box** integration within the Visual Studio IDE. | + |
| 8 | Adoption | **Some products** are used already. | + | It may require to educate **some people.** | - |
| **Total** | | | **1** | | **7** |

## Compare by price

Following table compares options by price

| | Option A | | Option M | |
|:---|:---|:---|:---|:---|
| Area | Product | Price | Tool | Price |
| Knowledge Sharing | [Atlassian Confluence](https://www.atlassian.com/software/confluence) |\< 10 users - $10/month<br/>\> 10 users - [$5/user/month](https://www.atlassian.com/software/confluence/pricing) | [Wiki](https://www.visualstudio.com/team-services/wiki/) |free - 5 users<br/>extra - [$3/user/month](https://marketplace.visualstudio.com/items?itemName=ms.vss-vstsuser#pricing)|
| Requirements Management | [Atlassian Jira](https://jira.atlassian.com/) |\< 10 users - [$10/month](https://www.atlassian.com/software/jira/pricing)<br/>\> 10 users - $7/user/month | [Agile Tools](https://www.visualstudio.com/team-services/agile-tools/) | Included |
| Source Control | [Atlassian Bitbucket](https://www.atlassian.com/software/bitbucket) | free - 5 users<br/>[extra - $5/user/month](https://www.atlassian.com/software/bitbucket/pricing?tab=cloud)| [Git](https://www.visualstudio.com/team-services/git/) | Included |
| Build & Release | [Jenkins](https://jenkins.io/) | *1 | [Continous Integration and Delivery](https://www.visualstudio.com/team-services/continuous-integration/) | free - [240 mins]/month<br/>extra - [$40/pipeline/month](https://marketplace.visualstudio.com/items?itemName=ms.build-release-hosted-pipelines#pricing) |
| Tests / Management | [Gurock TestRail](http://www.gurock.com/testrail/) | [$25/user/month](http://www.gurock.com/testrail/pricing/cloud/) | [Test Manager](https://www.visualstudio.com/team-services/testing-tools/) | [$52/user/month](https://marketplace.visualstudio.com/items?itemName=ms.vss-testmanager-web#pricing) |
| Tests / Performance | [Load Impact](https://loadimpact.com/) | [$300/month](https://loadimpact.com/pricing) | [Cloud Based Load Tests](https://www.visualstudio.com/team-services/cloud-load-testing/) | free - [20k VUMS]/month<br/>extra - [$36/[100k VUMS]](https://docs.microsoft.com/en-us/vsts/billing/buy-load-testing-vs#_buy-load-testing) |
| Package Management | [NuGet Server](https://docs.microsoft.com/en-us/nuget/hosting-packages/nuget-server) | *1 |[Package Manager](https://www.visualstudio.com/team-services/reporting/) | free - 5 users/month<br/>extra - [$4/user/month](https://marketplace.visualstudio.com/items?itemName=ms.feed#pricing) |
| Symbols Server |  | *1 | [Package Manager](https://www.visualstudio.com/team-services/reporting/) | Included |

*1 Are free, but requires additional infrastructure, setup, provision and management.
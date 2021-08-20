---
title: What's new in Microsoft Graph
description: What's currently new in Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 5926d13f8971d891d48eb09205162f502999faed
ms.sourcegitcommit: 22bd45d272681658d46a8b99af3c3eabc7b05cb1
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2021
ms.locfileid: "58384468"
---
# <a name="whats-new-in-microsoft-graph"></a>What's new in Microsoft Graph

See highlights of what's new in the recent two months in Microsoft Graph, [what's added earlier](whats-new-earlier.md), and how you can [share your ideas](#want-to-stay-in-the-loop). For a detailed list of API-level updates, see the [API changelog](https://developer.microsoft.com/graph/changelog/). 

> [!IMPORTANT]
> Features, including APIs and tools, in _preview_ status may change without notice, and some may never be promoted to generally available (GA) status. Do not use preview features in production apps.

## <a name="august-2021-new-and-generally-available"></a>August 2021: New and generally available

### <a name="devices-and-apps--corporate-management"></a>Devices and apps | Corporate management
Intune monthly updates for the v1.0 version. Set the **Date** filter for August, 2021, and look for a section with this same heading.

### <a name="devices-and-apps--service-health-and-communications"></a>Devices and apps | Service health and communications
GA of the [service communications API](service-communications-concept-overview.md) in Microsoft Graph to access the health status and message center posts about Microsoft cloud services.

### <a name="identity-and-access--governance"></a>Identity and access | Governance
Get a collection of access review scopes that is used to define reviewers and fallback reviewers for an [instance of access reviews](/graph/api/resources/accessReviewInstance).

## <a name="august-2021-new-in-preview-only"></a>August 2021: New in preview only

### <a name="devices-and-apps--corporate-management"></a>Devices and apps | Corporate management
Intune monthly updates for the beta version. Set the **Date** filter for August, 2021, and look for a section with this same heading.

### <a name="identity-and-access--governance"></a>Identity and access | Governance
- [Reprocess](/graph/api/accesspackageassignmentrequest-reprocess?view=graph-rest-beta&preserve-view=true) an [access package assignment request](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta&preserve-view=true) to automatically retry a user's request for access to the package.
- [Reprocess](/graph/api/accesspackageassignment-reprocess?view=graph-rest-beta&preserve-view=true) an [access package assignment](/graph/api/resources/accesspackageassignment?view=graph-rest-beta&preserve-view=true) to automatically re-evaluate and enforce a user's assignments.
- [Get a set of policy requirements](/graph/api/accesspackage-getapplicablepolicyrequirements?view=graph-rest-beta&preserve-view=true) to create an [assignment request for an access package](/graph/api/resources/accesspackageassignmentrequestrequirements?view=graph-rest-beta&preserve-view=true).
- Get a collection of [access review reviewer](/graph/api/resources/accessreviewreviewer?view=graph-rest-beta&preserve-view=true) resources that is used to define reviewers contacted for an [instance of access reviews](/graph/api/resources/accessReviewInstance?view=graph-rest-beta&preserve-view=true).
- Get or set the duration of inactivity that recommendations are configured from in the [schedule settings of an access review](/graph/api/resources/accessReviewScheduleSettings?view=graph-rest-beta&preserve-view=true), by using the **recommendationLookBackDuration** property.

### <a name="identity-and-access--identity-and-sign-in"></a>Identity and access | Identity and sign-in
Organizations can use [policies to enforce best practices for apps using application authentication methods](/graph/api/resources/applicationauthmethodpolicy?view=graph-rest-beta&preserve-view=true). Such policies can apply to [specific applications and service principals](/graph/api/resources/appmanagementpolicy?view=graph-rest-beta&preserve-view=true), or to [all applications and service principals in a tenant](/resources/tenantappmanagementpolicy?view=graph-rest-beta&preserve-view=true).

## <a name="july-2021-new-and-generally-available"></a>July 2021: New and generally available

### <a name="cloud-communications--calls"></a>Cloud communications | Calls
Support for a capacity limit for the number of participants that an application can handle when [answering](/graph/api/call-answer) a [call](/graph/api/resources/call), in organizations that adopt [Teams policy-based recording](/microsoftteams/teams-recording-policy).

### <a name="identity-and-access--identity-and-sign-in"></a>Identity and access | Identity and sign-in
- GA of identity providers that share a common base type [identityProviderBase](/graph/api/resources/identityproviderbase):
  - Built-in identity providers for Azure AD B2B scenarios in an Azure AD tenant. These providers can support Azure AD, Microsoft account (MSA), or email one-time passcodes.
  - Social identity providers in an Azure AD B2C tenant to allow users to sign up and sign in for the service using a social media account, such as Microsoft, Google, Facebook, Amazon, LinkedIn, or Twitter.
- Deprecation of the earlier [identity provider](/graph/api/resources/identityprovider) API.

### <a name="users"></a>Users
Let a user [change their own password](/graph/api/user-changepassword) without requiring an administrator role.


## <a name="july-2021-new-in-preview-only"></a>July 2021: New in preview only

### <a name="devices-and-apps--cloud-pc"></a>Devices and apps | Cloud PC
An on-premises connection [health check](/graph/api/cloudpconpremisesconnection-runhealthcheck?view=graph-rest-beta&preserve-view=true) can identify a few more possible health check error types:
- Cloud PC computer account is not found in the organizational unit (`adJoinCheckComputerObjectAlreadyExists`).
- Cloud PC object is not found in Azure AD (`azureAdDeviceSyncCheckDeviceNotFound`).
- Timeout from checking if a cloud PC object has been synchronized to Azure AD (`azureAdDeviceSyncCheckLongSyncCircle`). 

See the [reference](/graph/api/resources/cloudpconpremisesconnectionhealthcheck?view=graph-rest-beta&preserve-view=true#cloudpconpremisesconnectionhealthcheckerrortype-values) for details and recommended remedial actions.

### <a name="devices-and-apps--corporate-management"></a>Devices and apps | Corporate management
Intune monthly updates for the beta version. Set the **Date** filter for July, 2021, and look for a section with this same heading.

### <a name="devices-and-apps--multi-tenant-management"></a>Devices and apps | Multi-tenant management
Debut of the [Microsoft 365 Lighthouse API](managedtenants-concept-overview.md) that lets Managed Service Providers (MSPs) remotely manage multiple customer tenants at scale for compliance and threat detection, and help get tenant devices in a healthy and secure state.

### <a name="education"></a>Education
- Get an error count and status message as part of the [status of a school data synchronization](/graph/api/resources/educationsynchronizationprofilestatus?view=graph-rest-beta&preserve-view=true).
- Get `extracting` or `validating` as possible states of a such a sync.

### <a name="identity-and-access--governance"></a>Identity and access | Governance
Get a collection of errors in the lifecycle of an [access review instance](/graph/api/resources/accessreviewinstance?view=graph-rest-beta&preserve-view=true).

### <a name="search"></a>Search
- Use the [Microsoft Search API to retrieve information about the people](search-concept-person.md) who are most relevant to a user. Relevance is determined by the user’s communication and collaboration patterns and business relationships. 
- Access the [connectors indexing API](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true) in the microsoft.graph.externalConnectors sub-namespace.

### <a name="teamwork"></a>Teamwork
- [Subscribe to change notifications on the chat resource](teams-changenotifications-chat.md).
- [Subscribe to change notifications of users in a chat](teams-changenotifications-chatmembership.md), in a [channel](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true), or in a [team](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true) (i.e., [conversationMember](/graph/api/resources/conversationmember?view=graph-rest-beta&preserve-view=true) resources).
- Get details of an event that happened in a chat, channgel or team by accessing [eventMessageDetail](/graph/api/resources/EventMessageDetail?view=graph-rest-beta&preserve-view=true) from a [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta&preserve-view=true) or [chat](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true). For example, members added to a channel or  chat, and team description updated.


## <a name="want-to-stay-in-the-loop"></a>Want to stay in the loop?

Here are some ways we can engage:

- Are there scenarios you'd like Microsoft Graph to support? Sugira e vote em novos recursos na [Comunidade Microsoft Tech](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph).
    Some new features originate as popular requests from the developer community. The Microsoft Graph team regularly evaluates customer needs and releases new features in the following order:

    1. Debut in **_preview_** status. Any related REST API updates are in the beta endpoint (`https://graph.microsoft.com/beta`).  

    2. Promoted to **_general availability_ (GA)** status, if sufficient feedback indicates viability. Any related REST API updates are added to the v1.0 endpoint (`https://graph.microsoft.com/v1.0`). 
- Be an active member in the Microsoft Graph community! [Join](https://aka.ms/microsoftgraphcall) the monthly Microsoft Graph community call.
- Sign up for the [Microsoft 365 developer program](https://developer.microsoft.com/office/dev-program), get a free Microsoft 365 subscription, and start developing!


## <a name="see-also"></a>See also
- Check out the [Microsoft Graph developer blog](https://developer.microsoft.com/graph/blogs/) periodically for release announcements and helpful resources.
- Browse details of Microsoft Graph API additions, and API behavior updates in the [changelog](https://developer.microsoft.com/graph/changelog/).
- Find [highlights of earlier releases](whats-new-earlier.md).
- Learn more about [versioning, support, and breaking change policies for Microsoft Graph](versioning-and-support.md).

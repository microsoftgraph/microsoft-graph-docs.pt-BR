---
title: Hightlights of earlier releases in Microsoft Graph
description: What was new earlier in Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 1a4f37f025beb5f84bb822940d8bbbb8c870caeb
ms.sourcegitcommit: 22bd45d272681658d46a8b99af3c3eabc7b05cb1
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2021
ms.locfileid: "58384440"
---
# <a name="highlights-of-earlier-releases"></a>Highlights of earlier releases

## <a name="june-2021-new-and-generally-available"></a>June 2021: New and generally available

### <a name="applications"></a>Applications
Get or set the status of an [application](/graph/api/resources/application) or [servicePrincipal](/graph/api/resources/serviceprincipal) to identify if Microsoft has disabled the application through the **disabledByMicrosoftStatus** property. Disabling reasons include suspicious, abusive, or malicious activity, or a violation of the Microsoft Services Agreement.

### <a name="change-notifications"></a>Change notifications
Extended the maximum length of a subscription before expiring for the following resources:
- OneDrive [driveItem](/graph/api/resources/driveitem) and SharePoint [list](/graph/api/resources/list) from 3 to 30 days.
- [group](/graph/api/resources/group), [user](/graph/api/resources/user), or other directory resources from 3 to 29 days.

### <a name="change-tracking"></a>Change tracking
Removed limitation for tracking changes in non-root folders in OneDrive for Business and SharePoint.

### <a name="education"></a>Education
The APIs for the education [assignments service](/graph/api/resources/educationassignment) are now generally available. 

### <a name="identity-and-access--governance"></a>Identity and access | Governance
GA of the [access review](/graph/api/resources/accessreviewsv2-root) API. Check out the [overview](accessreviews-overview.md) and tutorials to [review access to security groups](tutorial-accessreviews-securitygroup.md) and [access to Microsoft 365 groups](tutorial-accessreviews-m365group.md). Note that the [legacy access review API](/graph/api/resources/accessreviews-root?view=graph-rest-beta&preserve-view=true) is being deprecated and will stop returning data in May 2023.


## <a name="june-2021-new-in-preview-only"></a>June 2021: New in preview only

### <a name="cloud-communications--online-meetings"></a>Cloud communications | Online meetings
Customize audio and video control in an [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) by enabling or disabling attendees from turning on their cameras and microphones, through the **allowAttendeeToEnableCamera** and **allowAttendeeToEnableMic** respectively.

### <a name="devices-and-apps--cloud-pc"></a>Devices and apps | Cloud PC
- [Assign](/graph/api/cloudpcusersetting-assign?view=graph-rest-beta&preserve-view=true) and manage [cloudPcUserSetting](/graph/api/resources/cloudpcusersetting?view=graph-rest-beta&preserve-view=true) to enable local admin or self-service option for a user on a cloud PC. Currently assignments can be made at a group level (users belonging to a Microsoft 365 group or security group).
- [Get](/graph/api/cloudpc-get?view=graph-rest-beta&preserve-view=true) a few new properties of a [cloudPC](/graph/api/resources/cloudpc?view=graph-rest-beta&preserve-view=true): the names of the provisioning policy and of the on-premises connection used during provisioning, and the end date/time of the grace period by which reprovisioning or deprovisioning happens.
- Support for more status and error types upon a [health check](/graph/api/cloudpconpremisesconnection-runhealthcheck?view=graph-rest-beta&preserve-view=true) on an [on-premises connection](/graph/api/resources/cloudpconpremisesconnection?view=graph-rest-beta&preserve-view=true).

### <a name="education"></a>Education
- Teachers can now select the default behavior for a calendar when they publish assignments. Teachers can control the assignment calendar behavior by using the **addToCalendarAction** property of the [educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta&preserve-view=true) resource.
- Teachers can now also set a default behavior for a calendar when they publish assignments. Teachers can control the assignment default calendar behavior by using the **addToCalendarAction** property of the [educationAssignmentDefaults](/graph/api/resources/educationAssignmentDefaults?view=graph-rest-beta&preserve-view=true) resource.

### <a name="groups"></a>Groups
Allow a [group](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) to be assigned to an Azure AD role on creation by setting the **isAssignableToRole** property. If set, this property makes it convenient to manage roles for individuals - instead of having to assign a role to each individual person, eligible persons can join a group, and assigning the role to the group would by default assign the role to each new person joining the group. 

### <a name="identity-and-access--governance"></a>Identity and access | Governance
Set users or group members to be notified of the progress of an [access review](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true), by using the **additionalNotificationRecipients** property of the [schedule definition](/graph/api/resources/accessreviewscheduledefinition?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access--identity-and-sign-in"></a>Identity and access | Identity and sign-in
Define a filter to dynamically include or exclude devices, using the **deviceFilter** property of [conditionalAccessDevices](/graph/api/resources/conditionalAccessDevices?view=graph-rest-beta&preserve-view=true).

### <a name="sites-and-lists"></a>Sites and lists
Create or get an existing [sharingLink](/graph/api/resources/sharinglink?view=graph-rest-beta&preserve-view=true) for a [listItem](/graph/api/resources/listitem?view=graph-rest-beta&preserve-view=true) by calling [createLink](/graph/api/listitem-createlink?view=graph-rest-beta&preserve-view=true).

### <a name="teamwork"></a>Teamwork
- [Get](/graph/api/chat-get?view=graph-rest-beta&preserve-view=true) an opaque URL to a [chat](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true) via the **webUrl** property.
- [Subscribe to change notifications](/graph/webhooks?view=graph-rest-beta&preserve-view=true) of a [channel](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true), [conversationMember](/graph/api/resources/conversationmember?view=graph-rest-beta&preserve-view=true), or [team](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true) resource.
- Use [resource-specific consent](/microsoftteams/platform/graph-api/rsc/resource-specific-consent) permissions with the APIs for [channel](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true), [chat](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true), [chatMessage](/graph/api/resources/chatMessage?view=graph-rest-beta&preserve-view=true), [chatMessageHostedContent](/graph/api/resources/chatMessageHostedContent?view=graph-rest-beta&preserve-view=true), or [team](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true).
- Get a list of [resource-specific permissions grants](/graph/api/resources/resourcespecificpermissiongrant?view=graph-rest-beta&preserve-view=true) for a [team](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true), that specifies that team's apps and the corresponding resource-specific permissions that they have been granted.
- [Get](/graph/api/teamsasyncoperation-get?view=graph-rest-beta&preserve-view=true) a specific [asynchronous operation](/graph/api/resources/teamsasyncoperation?view=graph-rest-beta&preserve-view=true), or [list](/graph/api/chat-list-operations?view=graph-rest-beta&preserve-view=true) all the asynchronous operations that run on a [chat](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true).
- Can specify a [Teams app](/graph/api/resources/teamsapp?view=graph-rest-beta&preserve-view=true) when [creating a chat](/graph/api/chat-post?view=graph-rest-beta&preserve-view=true).
- Use a single action [provisionEmail](/graph/api/channel-provisionemail?view=graph-rest-beta&preserve-view=true) to get the email address of a [channel](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true) if one exists, or create one otherwise. Use the [removeEmail](/graph/api/channel-removeemail?view=graph-rest-beta&preserve-view=true) action to remove the email address.

### <a name="teamwork--shifts"></a>Teamwork | Shifts
- Support for the [offerShiftRequest](/graph/api/resources/offershiftrequest?view=graph-rest-beta&preserve-view=true), [timeOff](/graph/api/resources/timeoff?view=graph-rest-beta&preserve-view=true), [timeOffReason](/graph/api/resources/timeoffreason?view=graph-rest-beta&preserve-view=true), and [timeOffRequest](/graph/api/resources/timeoffrequest?view=graph-rest-beta&preserve-view=true) entities for synchronous change notifications.
- Support for managing [time card](/graph/api/resources/timecard?view=graph-rest-beta&preserve-view=true) resources and common functionality such as [clock in](/graph/api/timecard-clockin?view=graph-rest-beta&preserve-view=true), [clock out](/graph/api/timecard-clockout?view=graph-rest-beta&preserve-view=true), [start break](/graph/api/timecard-startbreak?view=graph-rest-beta&preserve-view=true), [end break](/graph/api/timecard-endbreak?view=graph-rest-beta&preserve-view=true), [confirm](/graph/api/timecard-confirm?view=graph-rest-beta&preserve-view=true), and [replace](/graph/api/timecard-replace?view=graph-rest-beta&preserve-view=true).


## <a name="may-2021-new-and-generally-available"></a>May 2021: New and generally available

### <a name="devices-and-apps--cloud-printing"></a>Devices and apps | Cloud printing
Find out when a printer last interacted with Universal Print, by using the **lastSeenDateTime** property of [printer](/graph/api/resources/printer).

### <a name="identity-and-access--identity-and-sign-in"></a>Identity and access | Identity and sign-in
Get or update the role of a guest user by using the **guestUserRoleId** property of [authorizationPolicy](/graph/api/resources/authorizationpolicy).

### <a name="mail"></a>Mail
- [Create drafts and send Outlook messages in MIME format](outlook-send-mime-message.md), attach S/MIME digital signatures, and encrypt message content in S/MIME.
- Create a [mailFolder](/graph/api/resources/mailfolder) as a [hidden folder](/graph/api/resources/mailfolder#hidden-mail-folders) by [setting the isHidden property](/graph/api/user-post-mailfolders#example).

### <a name="microsoft-graph-toolkit"></a>Microsoft Graph Toolkit
Try the following new features in the Microsoft Graph Toolkit 2.2:
- [File](/graph/toolkit/components/file) and [file list](/graph/toolkit/components/file-list) components
- [MSAL 2.0 authentication provider](/graph/toolkit/providers/msal2)
- [SharePoint Framework library](/graph/toolkit/get-started/mgt-spfx)

### <a name="reports--azure-ad-activity-reports"></a>Reports | Azure AD activity reports
GA of the reporting API to [list](/graph/api/provisioningobjectsummary-list) actions performed by the Azure AD provisioning service and its associated properties. Aligned the prior beta version to the v1.0 version of the API.

## <a name="may-2021-new-in-preview-only"></a>May 2021: New in preview only

### <a name="connecting-external-content"></a>Connecting external content
- Be aware of [implementation and operational limits](connecting-external-content-api-limits.md) when designing connectors.
- Try the [connectors API with Postman](connecting-external-content-connectors-api-postman.md).

### <a name="devices-and-apps--cloud-pc"></a>Devices and apps | Cloud PC
Request the least privileged application permissions, `CloudPC.Read.All` or `CloudPC.ReadWrite.All`, to access methods of the following resources:
  - Read and write operations, and [reprovision](/graph/api/cloudpc-reprovision?view=graph-rest-beta&preserve-view=true) method of [cloudPC](/graph/api/resources/cloudpc?view=graph-rest-beta&preserve-view=true).
  - Read and write operations, and [getSourceImages](/graph/api/cloudpcdeviceimage-getsourceimages?view=graph-rest-beta&preserve-view=true) method of [cloudPcDeviceImage](/graph/api/resources/cloudpcdeviceimage?view=graph-rest-beta&preserve-view=true).
  - Read and write operations, and [updateAdDomainPassword](/graph/api/cloudpconpremisesconnection-updateaddomainpassword?view=graph-rest-beta&preserve-view=true) method of [cloudPcOnPremisesConnection](/graph/api/resources/cloudpconpremisesconnection?view=graph-rest-beta&preserve-view=true).
  - Read and write operations, and [assign](/graph/api/cloudpcprovisioningpolicy-assign?view=graph-rest-beta&preserve-view=true) method of [cloudPcProvisioningPolicy](/graph/api/resources/cloudpcprovisioningpolicy?view=graph-rest-beta&preserve-view=true).

### <a name="devices-and-apps--corporate-management"></a>Devices and apps | Corporate management
Intune monthly updates for the beta version. Set the **Date** filter for June, 2021, and look for a section with this same heading.

### <a name="education"></a>Education
- [Set up a SharePoint resource folder](/graph/api/educationAssignment-setupresourcesfolder?view=graph-rest-beta&preserve-view=true) to upload and store all file-based resources in the same location for an [educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta&preserve-view=true).
- [Set up a SharePoint resource folder](/graph/api/educationsubmission-setupresourcesfolder?view=graph-rest-beta&preserve-view=true) to upload and store all file-based resources, such as a Word or Excel file, in the same location for an [educationSubmission](/graph/api/resources/educationsubmission?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access--governance"></a>Identity and access | Governance
- Get a collection of [accessPackageAssignment](/graph/api/resources/accessPackageAssignment?view=graph-rest-beta&preserve-view=true) resources by [filtering on the signed-in user](/graph/api/accesspackageassignment-filterbycurrentuser?view=graph-rest-beta&preserve-view=true).
- Get a collection of [accessPackageAssignmentRequest](/graph/api/resources/accessPackageAssignmentRequest?view=graph-rest-beta&preserve-view=true) resources by [filtering on the signed-in user](/graph/api/accesspackageassignmentrequest-filterbycurrentuser?view=graph-rest-beta&preserve-view=true).

### <a name="use-sdks"></a>Use SDKs
Try the preview version of [Microsoft Graph .NET SDK v4](https://www.nuget.org/packages/Microsoft.Graph/4.0.0-preview.4), and take advantage of the following improvements:
- Use a single API to authenticate against Microsoft Graph and Azure .NET clients.
- New support for JSON serialization and deserialization.
- Easy access to response information.
- Better experience upgrading dependencies.

## <a name="april-2021-new-and-generally-available"></a>April 2021: New and generally available

### <a name="identity-and-access--identity-and-sign-in"></a>Identity and access | Identity and sign-in
- Manage an [authentication policy](/graph/api/resources/authenticationflowspolicy) at a tenant level, to enable or disable [self-service sign-up](/graph/api/resources/selfservicesignupauthenticationflowconfiguration) of external users.
- Administrators can associate user flows with apps that are shared with external users and enable [self-service sign-up](/azure/active-directory/external-identities/self-service-sign-up-overview) on those apps. They can customize a self-service sign-up user flow and create a personalized sign-up experience. Once an application is associated with the user flow, users who go to that application will be able to initiate a sign-up flow that provisions a guest account.
- Configure [user flow attributes](/graph/api/resources/identityuserflowattribute) in your Azure AD tenant allows you to collect information about a user during sign-up. You can collect a built-in set of attributes, or configure custom user flow attributes to collect information from a user that is not built in to the directory. 
- In an [Azure Active Directory user flow](/graph/api/resources/b2xidentityuserflow), you can manage language defaults and [customize the language and strings displayed to users in the user flow](/graph/api/resources/userflowlanguageconfiguration).
- Use an [API connector](/graph/api/resources/identityapiconnector) in user flows for Azure AD self-service sign-up and Azure AD B2C sign-up, to call an API at a specific step to affect the execution of the user flow.

### <a name="teamwork"></a>Teamwork
- Identify the channel by the **channelIdentity** property, if a [chatMessage](/graph/api/resources/chatmessage) is within a [channel](/graph/api/resources/channel).
- Identify the chat by the **chatId** property, if the **[chatMessage](/graph/api/resources/chatmessage)** is in a [chat](/graph/api/resources/chat).
- Use the **messages** relationship to get all the [chatMessage](/graph/api/resources/chatmessage) resources in a [chat](/graph/api/resources/chat).
- Use application permissions to [get](/graph/api/chat-get) the properties of a specified [chat](/graph/api/resources/chat).
- Use application permissions to [get a specified chat member](/graph/api/chat-get-members) or [get all the chat members](/graph/api/chat-list-members) included in a chat. Because data for users as chat members is sensitive, other than obtaining application permissions, please [request additional access](teams-protected-apis.md) to these operations.

### <a name="use-the-toolkit"></a>Use the Toolkit
New to the [Microsoft Graph Toolkit](/graph/toolkit/overview)? Try the new [Toolkit learning path](/learn/paths/m365-msgraph-toolkit/?WT.mc_id=m365-19989-cxa), use the Toolkit set of web components and authentication providers to connect a web app to Microsoft Graph, and load data from Microsoft 365.

## <a name="april-2021-new-in-preview-only"></a>April 2021: New in preview only

### <a name="cloud-communications--online-meetings"></a>Cloud communications | Online meetings
- Get a [report](/graph/api/resources/meetingattendancereport?view=graph-rest-beta&preserve-view=true) of [each attendee's attendance](/graph/api/resources/attendancerecord?view=graph-rest-beta&preserve-view=true) in a scheduled online meeting, through the **meetingAttendanceReport** property of the [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true).
- Enable, disable, or limit duration of chat for an online meeting by using the **allowMeetingChat** property.
- Enable or disable reactions for an online meeting, by using the **allowTeamworkReactions** property.

### <a name="compliance"></a>Compliance
[Get](/graph/api/ediscovery-settings-get?view=graph-rest-beta&preserve-view=true), [update](/graph/api/ediscovery-settings-update?view=graph-rest-beta&preserve-view=true), or [reset to default](/graph/api/ediscovery-settings-resettodefault?view=graph-rest-beta&preserve-view=true) the following [settings](/graph/api/resources/ediscovery-settings?view=graph-rest-beta&preserve-view=true) for an eDiscovery [case](/graph/api/resources/ediscovery-case?view=graph-rest-beta&preserve-view=true):
- [Detection of duplicates, near-duplicate](/microsoft-365/compliance/near-duplicate-detection-in-advanced-ediscovery?view=o365-worldwide&preserve-view=true), and [email threading](/microsoft-365/compliance/email-threading-in-advanced-ediscovery?view=o365-worldwide&preserve-view=true), through the **redundancyDetection** property.
- [Identifying themes](/microsoft-365/compliance/themes-in-advanced-ediscovery?view=o365-worldwide&preserve-view=true) which are prevalent ideas in documents of a review set, through the **topicModeling** property.
- [Extracting text from image files by optical character recognition (OCR)](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery?view=o365-worldwide&preserve-view=true#optical-character-recognition-ocr), through the **ocr** property.

These settings provide analytics functionality that [culls data intelligently](/microsoft-365/compliance/overview-ediscovery-20?view=o365-worldwide&preserve-view=true#cull-data-intelligently) in the end-to-end workflow of [Advanced eDiscovery](/microsoft-365/compliance/overview-ediscovery-20?view=o365-worldwide&preserve-view=true).

### <a name="devices-and-apps--device-updates"></a>Devices and apps | Device updates
Debut of APIs for the Windows Update for Business deployment service. The service supports deploying Windows 10 feature updates and expediting Windows 10 security updates on devices. To learn more, start with the [Windows updates API overview](windowsupdates-concept-overview.md).

### <a name="education"></a>Education
- Associate a folder with an [educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta&preserve-view=true) to  store all the related file resources, through the **resourcesFolderUrl** property.
- Deep link into an [educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta&preserve-view=true) through the **webUrl** property.

### <a name="identity-and-access--governance"></a>Identity and access | Governance
Administrators can [get](/graph/api/accessreviewpolicy-get?view=graph-rest-beta&preserve-view=true) or [update](/graph/api/accessreviewpolicy-update?view=graph-rest-beta&preserve-view=true) policies at the directory-level to review access, by using the [accessReviewPolicy](/graph/api/resources/accessreviewpolicy?view=graph-rest-beta&preserve-view=true) resource. For example, administrators can use an access review policy to enable or disable group owners reviewing access on groups that they own.

### <a name="search"></a>Search
[Enable spelling suggestions or corrections](search-concept-speller.md) for a user query. This is useful when a user query contains typing errors, or when the errors render no search results.

### <a name="teamwork"></a>Teamwork
- Use [resource-specific permission grant](/graph/api/resources/resourcespecificpermissiongrant?view=graph-rest-beta&preserve-view=true) to list the apps with access to a specified [group](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) or [chat](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true).
- [Get](/graph/api/teamsappicon-get?view=graph-rest-beta&preserve-view=true) the properties of an [icon](/graph/api/resources/teamsAppIcon?view=graph-rest-beta&preserve-view=true) associated with a Teams app. To get the actual image of the icon, use [get hosted content](/graph/api/teamworkhostedcontent-get?view=graph-rest-beta&preserve-view=true).

### <a name="use-sdks"></a>Use SDKs
- Try the [preview release of the Microsoft Graph JavaScript client library, version 3.0.0](https://www.npmjs.com/package/@microsoft/microsoft-graph-client/v/3.0.0-Preview.1).This release enables multiple authentication flows, server-side authentication, Node.js Stream large file upload and progress tracking, and more. See the [upgrade guide](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/changelogs/v3-upgrade-guide.md) for details.
- Try a new learning path to [explore Microsoft Graph scenarios for JavaScript development](/learn/paths/m365-msgraph-scenarios/?WT.mc_id=m365-16105-cxa).


## <a name="march-2021-new-and-generally-available"></a>March 2021: New and generally available

### <a name="applications"></a>Applications
- GA of the [applicationTemplate](/graph/api/resources/applicationtemplate) resource which supports [listing](/graph/api/applicationtemplate-list) applications in the Azure AD application gallery, and [adding](/graph/api/applicationtemplate-instantiate) an instance of such an application to a directory.
- Use app-only permission `Application.ReadWrite.OwnedBy` when [adding](/graph/api/applicationtemplate-instantiate) such an instance.
- Use the **signInAudience** property of [servicePrincipal](/graph/api/resources/serviceprincipal) to get the user accounts supported by the current application.

### <a name="devices-and-apps--cloud-printing"></a>Devices and apps | Cloud printing
- GA of the [cloud printing API](universal-print-concept-overview.md) for Universal Print! See the [announcement](https://techcommunity.microsoft.com/t5/windows-it-pro-blog/universal-print-is-ready-for-business/ba-p/2176778), and check out how to [get started with Universal Print](/universal-print/fundamentals/universal-print-license).
- [Subscribe to change notifications](universal-print-webhook-notifications.md) on a [print task definition](/graph/api/resources/printtaskdefinition) or [printer](/graph/api/resources/printer) resource.

### <a name="identity-and-access--governance"></a>Identity and access | Governance
- Use Azure Active Directory (Azure AD) [consent requests](/graph/api/resources/consentrequests-root) to manage the request workflow for users attempting to access apps that require admin approval. The API makes use of the following resources:
  - The [adminConsentRequestPolicy](/graph/api/resources/adminconsentrequestpolicy) resource for creating and managing requests for app access for the organization.
  - The [appConsentRequest](/graph/api/resources/appconsentrequest) resource for aggregating and managing user requests to access a specific app.
  - The [userConsentRequest](/graph/api/resources/userConsentRequest) resource for users requesting access to an app which requires admin authorization. 
  - The [accessReviewReviewerScope](/graph/api/resources/accessReviewReviewerScope) resource defines who is specified in the **adminConsentRequestPolicy** to review **appConsentRequest** and **userConsentRequest** objects.
  - The [approval](/graph/api/resources/approval) resource represents an approval decision for a request.
- GA of the Terms of Use API which supports a tenant's customizable [Terms of Use agreement](/graph/api/resources/agreement) in Azure AD.

### <a name="identity-and-access--identity-and-sign-in"></a>Identity and access | Identity and sign-in
- GA of [authentication methods](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta&preserve-view=true) including [FIDO2 security keys](/graph/api/resources/fido2authenticationmethod), [Microsoft Authenticator app](/graph/api/resources/microsoftauthenticatorauthenticationmethod), and [Windows Hello for Business](/graph/api/resources/windowshelloforbusinessauthenticationmethod).
- GA of [authentication method policies](/graph/api/resources/authenticationmethodspolicies-overview) that define authentication methods and the users that are allowed to use them to sign in and perform multi-factor authentication (MFA) in Azure AD. Authentication methods policies that can be managed in Microsoft Graph include [FIDO2 security keys](/graph/api/resources/fido2authenticationmethodconfiguration), Passwordless Phone Sign-in with [Microsoft Authenticator app](/graph/api/resources/microsoftauthenticatorauthenticationmethodconfiguration), and tenant's [email OTP authentication methods policy](/graph/api/resources/emailauthenticationmethodconfiguration).
- GA of [feature rollout policy](/graph/api/resources/featureRolloutPolicy) that helps tenant administrators to pilot features to specific groups before enabling them for the entire organization.
- GA of the [organization branding properties](/graph/api/resources/organizationalbrandingproperties) which enables a custom look and feel of Azure Active Directory sign-in screens. Organizations can customize based on locale for specific users.

### <a name="tasks-and-plans"></a>Tasks and plans
- Use the delegated permission of `Tasks.Read` to read operations of all Planner resources.
- Use the delegated permission of `Tasks.ReadWrite` to read and write operations of all Planner resources.

### <a name="teamwork"></a>Teamwork
- GA of [chat](/graph/api/resources/chat) operations, chat [conversationMember](/graph/api/resources/conversationmember), chat [app](/graph/api/resources/teamsappinstallation), chat [tab](/graph/api/resources/teamstab), and their methods.
- GA of a few more properties of [teamsAppDefinition](/graph/api/resources/teamsAppDefinition), which represent details of a version of an app in the Microsoft Teams app catalog, including the following:
  - **createdBy**, **description**, **shortDescription**, **lastModifiedDateTime**
  - **publishingState** which can be one of `submitted` and under review, `published`, or `rejected` by the admin
  - **bot** relationship of the [teamworkBot](/graph/api/resources/teamworkbot) type, representing the details of the bot specified in the teams app manifest.
- Use the activity feed notifications API to better engage users in three contexts:
  - [Send notification to user in a chat](/graph/api/chat-sendactivitynotification)
  - [Send notification to user in a team](/graph/api/team-sendactivitynotification)
  - [Send notification to user](/graph/api/userteamwork-sendactivitynotification)
- Migrate users' message history and data from an external system into a Teams channel, allowing users to continue their communications seamlessly. Use the following methods that support the migration scenario:
  - [Create team](/graph/api/team-post)
  - [Create channel](/graph/api/channel-post)
  - [Create chatMessage in a channel](/graph/api/channel-post-messages)
  - [Reply to a message in a channel](/graph/api/channel-post-messagereply)
  - [Complete message migration in a team](/graph/api/team-completemigration)
  - [Complete message migration in a channel](/graph/api/channel-completemigration)
- [List](/graph/api/chatmessage-list-chatmessagehostedcontents) or [get](/graph/api/chatmessagehostedcontent-get) rich content hosted in a [chatMessage](/graph/api/resources/chatmessage), such as images or code snippets.
- Delegated permissions support of `ChannelMessage.Read.All` for subscribing change notifications on [chatMessage](/graph/api/resources/chatmessage) resources.

## <a name="march-2021-new-in-preview-only"></a>March 2021: New in preview only

### <a name="applications"></a>Applications
[Create and add self-signed certificates](/graph/api/servicePrincipal-addTokenSigningCertificate?view=graph-rest-beta&preserve-view=true) to your SAML applications. Use this to help enable single sign-on for Azure AD gallery apps in your tenant by allowing Azure AD to sign SAML responses.

### <a name="devices-and-apps--cloud-pc"></a>Devices and apps | Cloud PC
Added to the [cloudPcDeviceImage](/graph/api/resources/cloudpcdeviceimage?view=graph-rest-beta&preserve-view=true) resource two more reasons for failure to upload a device source image: operating system not supported (`osVersionNotSupported`), or an invalid source image to provision a Windows VM (`sourceImageInvalid`).

### <a name="devices-and-apps--cloud-printing"></a>Devices and apps | Cloud printing
Get the most recent date/time (**lastSeenDateTime** property) when a printer interacted with Universal Print.

### <a name="devices-and-apps--corporate-management"></a>Devices and apps | Corporate management
Intune [March](https://developer.microsoft.com/graph/changelog/?from=2021-03-01&to=2021-03-31&filterBy=Corporate%20management) updates for the beta version.

### <a name="identity-and-access--governance"></a>Identity and access | Governance
Apply the new model of [access reviews](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) to group memberships and all other supported resource types. Deprecate the [legacy model of access reviews](/graph/api/resources/accessreviews-root?view=graph-rest-beta&preserve-view=true).

### <a name="sites-and-lists"></a>Sites and lists
- Support a specific content type or template for documents or document sets in specific site collections, through a set of new properties and methods on the [contentType](/graph/api/resources/contentType?view=graph-rest-beta&preserve-view=true) entity. The methods include the following:
  - [addCopy](/graph/api/contenttype-addcopy?view=graph-rest-beta&preserve-view=true)
  - [associateWithHubSites](/graph/api/contenttype-associatewithhubsites?view=graph-rest-beta&preserve-view=true)
  - [copyToDefaultContentLocation](/graph/api/contenttype-copytodefaultcontentlocation?view=graph-rest-beta&preserve-view=true)
  - [isPublished](/graph/api/contenttype-ispublished?view=graph-rest-beta&preserve-view=true)
  - [publish](/graph/api/contenttype-publish?view=graph-rest-beta&preserve-view=true)
  - [unpublish](/graph/api/contenttype-unpublish?view=graph-rest-beta&preserve-view=true)
- Customize content types by their columns. Columns are represented by the [columnDefinition](/graph/api/resources/columndefinition?view=graph-rest-beta&preserve-view=true) entity, and support the full set of CRUD operations.
- [Get content types of a site that can be applied to a list](/graph/api/site-getApplicableContentTypesForList?view=graph-rest-beta&preserve-view=true).
- Differentiate column types by the following properties in the **columnDefinition** entity: boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text. These properties are mutually exclusive.

### <a name="sites-and-lists--taxonomy"></a>Sites and lists | Taxonomy
- Navigate from a [site](/graph/api/resources/site?view=graph-rest-beta&preserve-view=true) to a [taxonomy term store](/graph/api/resources/termstore-store?view=graph-rest-beta&preserve-view=true) using the **termStore** relationship.
- In the reverse direction, get the ID of the parent site of a term store using the **parentSiteId** property.

### <a name="users"></a>Users
- [Get](/graph/api/regionalandlanguagesettings-get?view=graph-rest-beta&preserve-view=true) or [update](/graph/api/regionalandlanguagesettings-update?view=graph-rest-beta&preserve-view=true) a user's [preferences for translating languages](/graph/api/resources/translationpreferences?view=graph-rest-beta&preserve-view=true). For example, whether or not to translate, translate automatically, or prompt before translating specific languages in messages, chats, and web pages, and any [translation overrides](/graph/api/resources/translationlanguageoverride?view=graph-rest-beta&preserve-view=true).
- [Activate a service plan](/graph/api/user-activateServicePlan?view=graph-rest-beta&preserve-view=true) for a user.


## <a name="february-2021-new-and-generally-available"></a>February 2021: New and generally available

### <a name="cloud-communications--online-meeting"></a>Cloud communications | Online meeting
Use policy-based application permissions of `OnlineMeetings.Read.All` or `OnlineMeetings.ReadWrite.All` on operations and methods of the [onlineMeeting](/graph/api/resources/onlinemeeting) resource. This means administrators can [configure application access policy](cloud-communication-online-meeting-application-access-policy.md) to allow apps to access online meetings on behalf of a user.

### <a name="sites-and-lists"></a>Sites and lists
Use the [permission](/graph/api/resources/permission) resource and its CRUD operations to manage sharing permission granted for a [driveItem](/graph/api/resources/driveitem). Permissions with a link facet represent sharing links created on the item. Permissions with an invitation facet represent permissions added by inviting specific users or groups to have access to the file.

## <a name="february-2021-new-in-preview-only"></a>February 2021: New in preview only

### <a name="applications"></a>Applications
Use application permissions for the [synchronization APIs](/graph/api/resources/synchronization-overview?view=graph-rest-beta&preserve-view=true) that automate provisioning (creation, maintenance) and de-provisioning (removal) of identities in Azure AD.

### <a name="cloud-communications--calls"></a>Cloud communications | Calls
Support for [policy-based recording for calls](/microsoftteams/teams-recording-policy) where using administrative policy, calls are automatically recorded for subsequent processing and retention as required by relevant corporate or regulatory policy. Before a policy-based participant joins a call, policy stipulates sending a [participantJoiningNotification ](/graph/api/resources/participantJoiningNotification?view=graph-rest-beta&preserve-view=true) to the bot associated with the policy that has available capacity to handle the new participant. The bot responds with one of [acceptJoinResponse](/graph/api/resources/acceptjoinresponse?view=graph-rest-beta&preserve-view=true), [rejectJoinResponse](/graph/api/resources/rejectjoinresponse?view=graph-rest-beta&preserve-view=true), or [inviteNewBotResponse](/graph/api/resources/invitenewbotresponse?view=graph-rest-beta&preserve-view=true) in its response payload.

### <a name="compliance--ediscovery"></a>Compliance | eDiscovery
- Use the [legalHold](/graph/api/resources/ediscovery-legalhold?view=graph-rest-beta&preserve-view=true) resource and its APIs to protect content indefinitely from deletion, for the purpose of litigation, internal investigation, or other legal actions.
- Use the [sourceCollection](/graph/api/resources/ediscovery-sourcecollection?view=graph-rest-beta&preserve-view=true) resource and its APIs to search for and identify relevant documents from custodial and non-custodial locations in Microsoft 365.
- Use the [tag](/graph/api/resources/ediscovery-tag?view=graph-rest-beta&preserve-view=true) resource and APIs to mark documents during review to separate responsive and non-responsive content.
- [Export](/graph/api/ediscovery-reviewset-export?view=graph-rest-beta&preserve-view=true) documents from a [review set](/graph/api/resources/ediscovery-reviewset?view=graph-rest-beta&preserve-view=true).
- Use the [addToReviewSet](/graph/api/ediscovery-reviewset-addtoreviewset?view=graph-rest-beta&preserve-view=true) action to add documents in a **sourceCollection** to a **reviewSet**.
- [Apply tags](/graph/api/ediscovery-reviewsetquery-applytags?view=graph-rest-beta&preserve-view=true) to documents based on a [review set query](/graph/api/resources/ediscovery-reviewsetquery?view=graph-rest-beta&preserve-view=true).
- Defined all eDiscovery API in the `microsoft.graph.ediscovery` namespace.
- Changed delegated permissions model from `User.Read` to `eDiscovery.Read.All` and `eDiscovery.ReadWrite.All`.

### <a name="devices-and-apps--corporate-management"></a>Devices and apps | Corporate management
- Intune [February](https://developer.microsoft.com/graph/changelog/?from=2021-02-01&to=2021-02-28&filterBy=Corporate%20management) updates for the beta version.
- New properties set by Intune on the [device](/graph/api/resources/device?view=graph-rest-beta&preserve-view=true) resource: **deviceCategory**, **deviceOwnership**, **domainName**, **enrollmentProfileName**, **enrollmentType**, **isRooted**, **managementType**, and **registrationDateTime**.

### <a name="education"></a>Education
Use [educationAssignmentDefaults](/graph/api/resources/educationAssignmentDefaults?view=graph-rest-beta&preserve-view=true) to specify default practices on an assignment for a class, for example, assignment due time, channel URL for notifications on an assignment. You can still customize values when creating an assignment.

### <a name="identity-and-access--identity-and-sign-in"></a>Identity and access | Identity and sign-in
- Use the [smsAuthenticationMethodConfiguration](/graph/api/resources/smsAuthenticationMethodConfiguration?view=graph-rest-beta&preserve-view=true) resource to [get](/graph/api/smsauthenticationmethodconfiguration-get?view=graph-rest-beta&preserve-view=true), [update](/graph/api/smsauthenticationmethodconfiguration-update?view=graph-rest-beta&preserve-view=true), or [delete](/graph/api/smsauthenticationmethodconfiguration-delete?view=graph-rest-beta&preserve-view=true) the configuration settings of a text message authentication policy in an organization.
- Use the [temporaryAccessPassAuthenticationMethodConfiguration](/graph/api/resources/temporaryaccesspassauthenticationmethodconfiguration?view=graph-rest-beta&preserve-view=true) resource to [get](/graph/api/temporaryaccesspassauthenticationmethodconfiguration-get?view=graph-rest-beta&preserve-view=true), [update](/graph/api/temporaryaccesspassauthenticationmethodconfiguration-update?view=graph-rest-beta&preserve-view=true), and [delete](/graph/api/temporaryaccesspassauthenticationmethodconfiguration-delete?view=graph-rest-beta&preserve-view=true) the configuration settings of a temporary access pass authentication policy in an organization.

### <a name="identity-and-access--governance"></a>Identity and access | Governance
- Assign geolocation information to an [access package](/graph/api/resources/accesspackage?view=graph-rest-beta&preserve-view=true) resource in the [access package assignment request](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta&preserve-view=true).
- Get a list of all [access package resource environments](/graph/api/resources/accesspackageresourceenvironment?view=graph-rest-beta&preserve-view=true) that represent the geolocations that store SharePoint Online resources.
- Use application permissions (`EntitlementManagement.Read.All` or `EntitlementManagement.ReadWrite.All`) for operations of the following resources:
  - [accessPackage](/graph/api/resources/accesspackage?view=graph-rest-beta&preserve-view=true)
  - [accessPackageAssignment](/graph/api/resources/accesspackageassignment?view=graph-rest-beta&preserve-view=true)
  - [accessPackageAssignmentPolicy](/graph/api/resources/accesspackageassignmentpolicy?view=graph-rest-beta&preserve-view=true)
  - [accessPackageAssignmentRequest](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta&preserve-view=true)
  - [accessPackageAssignmentResourceRole](/graph/api/resources/accesspackageassignmentresourcerole?view=graph-rest-beta&preserve-view=true)
  - [accessPackageCatalog](/graph/api/resources/accesspackagecatalog?view=graph-rest-beta&preserve-view=true)
  - [accessPackageResourceRequest](/graph/api/resources/accesspackageresourcerequest?view=graph-rest-beta&preserve-view=true)
  - [connectedOrganization](/graph/api/resources/connectedorganization?view=graph-rest-beta&preserve-view=true)
  - [entitlementManagementSettings](/graph/api/resources/entitlementmanagementsettings?view=graph-rest-beta&preserve-view=true)

### <a name="reports--microsoft-365-usage-reports"></a>Reports | Microsoft 365 usage reports
Get more properties included in [detail reports for SharePoint site usage](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-beta&preserve-view=true): anonymousLinkCount, companyLinkCount, externalSharing, geolocation, secureLinkForGuestCount, secureLinkForMemberCount, siteSensitivityLabelId, and unmanagedDevicePolicy.

### <a name="tasks-and-plans"></a>Tasks and plans
- Define up to 25 categories in a [plan details](/graph/api/resources/plannerplandetails?view=graph-rest-beta&preserve-view=true) object for a plan. For each category, specify a descriptive label and associate tasks in a plan with one or more of these categories. 
- Use a [roster](/graph/api/resources/plannerRoster?view=graph-rest-beta&preserve-view=true) to represent a collection of users collaborating on a [plan](/graph/api/resources/plannerplan?view=graph-rest-beta&preserve-view=true). Use the **rosterPlans** relationship to get the rosters of which the user is a [member](/graph/api/resources/plannerrostermember?view=graph-rest-beta&preserve-view=true). 
- For plans that are surfaced in experiences outside of Planner, such as Microsoft Teams, specify in the [plan context details](/graph/api/resources/plannerplancontextdetails?view=graph-rest-beta&preserve-view=true) how to display the link to the [plan context](/graph/api/resources/plannerPlanContext?view=graph-rest-beta&preserve-view=true). 

### <a name="use-sdks"></a>Use SDKs
Try the preview release of the [Microsoft Graph Java SDK v3](https://github.com/microsoftgraph/msgraph-sdk-java/tree/feature/v3)! For more information, see the related [blog post](https://developer.microsoft.com/graph/blogs/announcing-the-public-preview-of-microsoft-graph-java-sdk-v3/).

## <a name="january-2021-new-in-preview-only"></a>January 2021: New in preview only

### <a name="cloud-communications"></a>Cloud communications
- Organize a live event as an [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) - see an [example](/graph/api/application-post-onlinemeetings?view=graph-rest-beta&preserve-view=true#example-3-create-a-live-event-with-a-user-token). 
- Get the content stream of an [attendee report](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true#example-4-retrieve-the-attendee-report-of-a-live-event), [recording](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true#example-5-retrieve-the-recording-of-a-live-event), or alternative recording of the live event.
- Get the [presence](/graph/api/resources/presence?view=graph-rest-beta&preserve-view=true) status of a user who is [out-of-office](/graph/api/resources/outofofficesettings?view=graph-rest-beta&preserve-view=true), and any message set for that status.

### <a name="devices-and-apps--cloud-pc"></a>Devices and apps | Cloud PC
- [Update an Active Directory domain password](/graph/api/cloudpconpremisesconnection-updateaddomainpassword?view=graph-rest-beta&preserve-view=true) for a successful [on-premises network connection](/graph/api/resources/cloudPcOnPremisesConnection?view=graph-rest-beta&preserve-view=true).
- [Running health checks on an on-premises network connection](/graph/api/cloudpconpremisesconnection-runhealthcheck?view=graph-rest-beta&preserve-view=true) can now expose 5 additional error types in the [on-premises connection health check](/graph/api/resources/cloudpconpremisesconnectionhealthcheck?view=graph-rest-beta&preserve-view=true) resource. For more information on the error types, see the [changelog](https://developer.microsoft.com/graph/changelog) for January 2021.

### <a name="devices-and-apps--cloud-printing"></a>Devices and apps | Cloud printing
- [Subscribe to change notifications of cloud printing](universal-print-webhook-notifications.md) - when a print job is started, and when the print job is ready to be downloaded by a printer.
- Get a fuller range of [possible values](/graph/api/resources/printerstatus?view=graph-rest-beta&preserve-view=true#printerprocessingstatedetail-values) for the status of a [printer](/graph/api/resources/printer?view=graph-rest-beta&preserve-view=true).
- Use delegated permissions in apps on behalf of the signed-in user:
  - `PrinterShare.ReadBasic.All` to read basic information about printer shares, excluding access control information.
  - `PrintConnector.Read.All` to read print connectors.
  - `PrintConnector.ReadWrite.All` to read or write print connectors.
  - `PrintJob.Create` to create print jobs and upload content to print jobs.
  - `PrintSettings.Read.All` to read tenant-wide print settings.
  - `PrintSettings.ReadWrite.All` to read or write tenant-wide print settings.
  - `Reports.Read.All` to read print usage summary per specified user or per printer.

### <a name="education"></a>Education
Use class-level [assignment settings](/graph/api/resources/educationAssignmentSettings?view=graph-rest-beta&preserve-view=true) to enable or disable animation to celebrate turning in an assignment.

### <a name="groups"></a>Groups
Get the processing status of a rule-based dynamic group by using the **membershipRuleProcessingStatus** property. This is useful when an attribute of a user changes, the user's membership in a rule-based [Microsoft 365 group](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) is re-evaluated based on the group membership rules set for the organization. 

### <a name="identity-and-access--directory-management"></a>Identity and access | Directory management
Get the [usage right](/graph/api/resources/UsageRight?view=graph-rest-beta&preserve-view=true) that a user or device has over third-party software built on PowerApps, or, usage right of a device over a subscription. Usage right includes identifiers for the corresponding service or product, and the current state of the usage right such as active, inactive, in warning, or suspended.

### <a name="identity-and-access--identity-and-sign-in"></a>Identity and access | Identity and sign-in
- Apps can use application permissions to let administrators manage [authentication methods](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta&preserve-view=true) for users.
- Support [Microsoft Authenticator](/graph/api/resources/microsoftauthenticatorauthenticationmethod?view=graph-rest-beta&preserve-view=true) as an authentication method of a user to sign in or perform multi-factor authentication to Azure AD.
- Use [Microsoft Authenticator policy](/graph/api/resources/microsoftauthenticatorauthenticationmethodconfiguration?view=graph-rest-beta&preserve-view=true) to define configuration settings and users or groups that are enabled to use Microsoft Authenticator as an authentication method. Use Microsoft Authenticator policy in place of [Microsoft Authenticator passwordless phone sign-in policy](/graph/api/resources/passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration?view=graph-rest-beta&preserve-view=true) which is deprecated. 
- Support [Windows Hello for Business](/graph/api/resources/windowshelloforbusinessauthenticationmethod?view=graph-rest-beta&preserve-view=true) as an authentication method of a user to sign in on Windows devices without using a password.

### <a name="reports--identity-and-access-reports"></a>Reports | Identity and access reports
- [Get a report of the number of users who are registered, or who are capable of various registration features](/graph/api/authenticationmethodsroot-usersregisteredbyfeature?view=graph-rest-beta&preserve-view=true), including multi-factor authentication, self-service password reset, or passwordless authentication.
- [Get a report of the number of users registered for each authentication method](/graph/api/authenticationmethodsroot-usersregisteredbymethod?view=graph-rest-beta&preserve-view=true), including password, Windows Hello for Business, or passwordless phone sign-in.

## <a name="december-2020-new-and-generally-available"></a>December 2020: New and generally available

### <a name="calendar"></a>Calendar
- Meeting organizers can use the **hideAttendees** property of an [event](/graph/api/resources/event) to control whether attendees can see one another in the meeting **Tracking** list.
- GA of the **isDraft** property and [cancel](/graph/api/event-cancel) method that are available to organizers, and the [forward](/graph/api/event-forward) method available to organizers and attendees to better manage [event](/graph/api/resources/event) resources in a calendar.
- GA of the **hexColor** and **isDefault** properties of a [calendar](/graph/api/resources/calendar) to better manage calandars.

### <a name="cloud-communications"></a>Cloud communications
GA of the [presence](/graph/api/resources/presence) resource, allowing getting presence information of one or more users, such as their availability and user activity.

### <a name="identity-and-access--identity-and-sign-in"></a>Identity and access | Identity and sign-in
Try a new [tutorial](tutorial-riskdetection-api.md) to learn how to use the [identity protection API](/graph/api/resources/identityprotectionroot) to identify risk and configure a workflow to confirm compromise or enable remediation.

### <a name="teamwork"></a>Teamwork
- GA of the [API to manage the installation of a Teams app](/graph/api/resources/teamsappinstallation), including getting installed apps, or adding, removing, or upgrading of the app in a team or in the personal scope of a user.
- [Get a chat between a user and a Teams app](/graph/api/userscopeteamsappinstallation-get-chat).

### <a name="use-the-toolkit"></a>Use the Toolkit
GA of Microsoft Graph Toolkit 2.0 - this release includes a new [component for Microsoft Graph To-Do tasks](./toolkit/components/todo.md), distinct from the[Planner tasks component](./toolkit/components/tasks.md), and an enhanced [person card component](./toolkit/components/person-card.md). See the [related blog post](https://developer.microsoft.com/graph/blogs/announcing-the-general-availability-of-microsoft-graph-toolkit-2-0/) for more information.


## <a name="december-2020-new-in-preview-only"></a>December 2020: New in preview only

### <a name="compliance--ediscovery"></a>Compliance | eDiscovery
Continuing to fulfill the pipeline of [Microsoft 365 compliance APIs](/graph/api/resources/ediscoveryapioverview?view=graph-rest-beta&preserve-view=true) are the [custodian](/graph/api/resources/custodian?view=graph-rest-beta&preserve-view=true) resource and its related operations and methods to [release](/graph/api/custodian-release?view=graph-rest-beta&preserve-view=true) or [activate](/graph/api/custodian-activate?view=graph-rest-beta&preserve-view=true) a custodian. Use the **custodian** resource to access the custodian's data ([userSource](/graph/api/resources/userSource?view=graph-rest-beta&preserve-view=true)) in an Exchange Online mailbox and OneDrive for Business, SharePoint sites ([siteSource](/graph/api/resources/siteSource?view=graph-rest-beta&preserve-view=true)), and Microsoft 365 groups ([unifiedGroupSource](/graph/api/resources/unifiedGroupSource?view=graph-rest-beta&preserve-view=true)).

### <a name="devices-and-apps--cloud-pc"></a>Devices and apps | Cloud PC
Identify the failure status of a cloud-managed virtual desktop collectively as `failed`, in the **status** property of the [cloudPC](/graph/api/resources/cloudpc?view=graph-rest-beta&preserve-view=true) resource.

### <a name="devices-and-apps--cloud-printing"></a>Devices and apps | Cloud printing
- [Update](/graph/api/printjob-update-configuration?view=graph-rest-beta&preserve-view=true) the [configuration](/graph/api/resources/printjobconfiguration?view=graph-rest-beta&preserve-view=true) of a [print job](/graph/api/resources/printjob?view=graph-rest-beta&preserve-view=true).
- For details on the renaming of a few properties and retyping of relationships, see the December 2020 section of the [API changelog](https://developer.microsoft.com/graph/changelog/) for details.

### <a name="education"></a>Education
- If students are added after publishing the assignment, teachers can control the assignment behavior by using the **addedStudentAction** property of the [educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta&preserve-view=true) resource.
- Teachers can post assignment publish notification through the **notificationChannelUrl** property of the **educationAssignment** resource.

### <a name="identity-and-access"></a>Identity and access
Get or set the version and creation metadata for an Azure AD [terms of use](/graph/api/resources/agreement?view=graph-rest-beta&preserve-view=true) [agreement](/graph/api/resources/agreement?view=graph-rest-beta&preserve-view=true), [agreement file](/graph/api/resources/agreementfile?view=graph-rest-beta&preserve-view=true), and [agreementfilelocalization](/graph/api/resources/agreementfilelocalization?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access--governance"></a>Identity and access | Governance
As part of Azure Active Directory [entitlement management](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta&preserve-view=true), when users wishing to access groups, applications, or SharePoint Online sites request an assignment to an [access package](/graph/api/resources/accesspackage?view=graph-rest-beta&preserve-view=true), they can now respond to [questions](/graph/api/resources/accesspackagequestion?view=graph-rest-beta&preserve-view=true) represented in [localized content](/graph/api/resources/accesspackagelocalizedcontent?view=graph-rest-beta&preserve-view=true) in the [access package assignment request](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access--identity-and-sign-in"></a>Identity and access | Identity and sign-in
- Administrators can associate user flows with apps that are shared with external users and enable [self-service sign-up](/azure/active-directory/external-identities/self-service-sign-up-overview) on those apps. They can customize a self-service sign-up user flow and create a personalized sign-up experience. Specifically, they create a [listener for a sign-up-start event to invoke a custom user flow](/graph/api/resources/invokeuserflowlistener?view=graph-rest-beta&preserve-view=true). Once an application is associated with the user flow, users who go to that application will be able to initiate a sign-up flow that provisions a guest account.
- In an [Azure Active Directory user flow](/graph/api/resources/b2xidentityuserflow?view=graph-rest-beta&preserve-view=true) or [Azure Active Directory B2C tenant user flow](/graph/api/resources/b2cidentityuserflow?view=graph-rest-beta&preserve-view=true), you can manage language defaults and [customize the language and strings displayed to users in the user flow](/graph/api/resources/userflowlanguageconfiguration?view=graph-rest-beta&preserve-view=true).
- Use an [API connector](/graph/api/resources/identityapiconnector?view=graph-rest-beta&preserve-view=true) in user flows for Azure AD self-service sign-up and Azure AD B2C sign-up, to call an API at a specific step to affect the execution of the user flow.
- Define an [email OTP authentication methods policy](/graph/api/resources/emailauthenticationmethodconfiguration?view=graph-rest-beta&preserve-view=true) for a tenant.

### <a name="teamwork"></a>Teamwork
- For a [member](/graph/api/resources/conversationmember?view=graph-rest-beta&preserve-view=true) resource in a [team](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true), [channel](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true), or a [chat](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true) context, you can now:
  - Differentiate a member who is an [Azure AD user](/graph/api/resources/aaduserconversationmember?view=graph-rest-beta&preserve-view=true), noting the user ID, email address, and Azure AD tenant ID. 
  - [Add multiple users as members of a team](/graph/api/conversationmembers-add?view=graph-rest-beta&preserve-view=true).
- For a [chat](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true) resource:
  - [Get all the messages in chats that the specified user has participated in](/graph/api/chats-getallmessages?view=graph-rest-beta&preserve-view=true), including one-on-one chats, group chats, and meeting chats.
  - Use the full range of functionality to list, get, add, remove, and update an [app](/graph/api/resources/teamsappinstallation?view=graph-rest-beta&preserve-view=true) or a [tab](/graph/api/resources/teamstab?view=graph-rest-beta&preserve-view=true) in a chat.
  - Use the **chatType** property to distinguish a one-on-one chat from a group chat or from a chat associated with an online meeting.
  - [Create](/graph/api/chat-post?view=graph-rest-beta&preserve-view=true) or [update](/graph/api/chat-patch?view=graph-rest-beta&preserve-view=true) a chat.
  - For a member in a chat context, use the **visibleHistoryStartDateTime** property to set or get a timestamp that represents how far back a conversation's history is shared with that member.
  - [Create](/graph/api/chat-post-members?view=graph-rest-beta&preserve-view=true) to or [delete](/graph/api/chat-delete-members?view=graph-rest-beta&preserve-view=true) a member from a specified chat. 
- For a [channel](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true) resource:
  - [Get all the messages across all the channels in a team](/graph/api/channels-getallmessages?view=graph-rest-beta&preserve-view=true).
  - Team owners can turn on [moderation for a channel](/graph/api/resources/channelmoderationsettings?view=graph-rest-beta&preserve-view=true) to control who can start new posts or reply to posts in that channel, using the **moderationSettings** property of the channel.
- As part of a [Teams app definition](/graph/api/resources/teamsappdefinition?view=graph-rest-beta&preserve-view=true), use the **bot** relationship to connect to a [teamwork bot](/graph/api/resources/teamworkbot?view=graph-rest-beta&preserve-view=true).

### <a name="to-do-tasks"></a>To-do tasks
Subscribe to [change notifications](webhooks.md) of a [To Do task](/graph/api/resources/todoTask?view=graph-rest-beta&preserve-view=true).


## <a name="november-2020-new-and-generally-available"></a>November 2020: New and generally available

### <a name="cloud-communications"></a>Cloud communications
- GA of the **role** property of the [meetingParticipantInfo](/graph/api/resources/meetingParticipantInfo) type, that distinguishes the role of a participant in an [online meeting](/graph/api/resources/onlinemeeting) as an attendee or presenter.
- GA of the **lobbyBypassSettings** property and its [values](/graph/api/resources/lobbybypasssettings#lobbybypassscope-values) to admit users to an online meeting.
- GA of the **isEntryExitAnnounced** property to customize settings for announcing callers joining or leaving an online meeting.
- GA of the **allowedPresenters** property to allow specific presenters in the meeting.

### <a name="search"></a>Search
- GA of the Microsoft Search [query API](/graph/api/resources/search-api-overview), supporting scoped searching of the following types of data:
  - [Outlook messages](./search-concept-messages.md)
  - [Outlook calendar events](./search-concept-events.md)
  - [OneDrive and SharePoint resources](./search-concept-files.md).

### <a name="teamwork"></a>Teamwork

- GA of resource-specific consent (RSC) permissions. RSC permissions allow team owners to grant granular consent to a production app to access and/or modify specific data of a team, for example, reading the team's settings, or modifying channel names, descriptions, and other settings.
- GA of APIs that apply to a [channel](/graph/api/resources/channel) or messages within a channel. The APIs include:
  - [Create](/graph/api/conversationmember-add) or [delete](/graph/api/conversationmember-delete) a conversation member from a channel.
  - [Update the role of a member](/graph/api/conversationmember-update) in a channel.
  - Get a specific message or all messages in a channel.
  - Get a specific reply or all replies in a channel.
  - [Track new or updated messages in a channel](/graph/api/chatmessage-delta).


## <a name="november-2020-new-in-preview-only"></a>November 2020: New in preview only

### <a name="devices-and-apps--cloud-pc"></a>Devices and apps | Cloud PC
Debut of the [cloud PC API](/graph/api/resources/virtualendpoint?view=graph-rest-beta&preserve-view=true) that lets organizations provision and manage virtual desktops for employees. Use it in conjunction with the Intune API to manage physical and virtual endpoints.

### <a name="devices-and-apps--cloud-printing"></a>Devices and apps | Cloud printing
[Subscribe to change notifications](webhooks.md) on a [print task definition](/graph/api/resources/printtaskdefinition?view=graph-rest-beta&preserve-view=true).

### <a name="devices-and-apps--corporate-management"></a>Devices and apps | Corporate management
Intune [November](changelog.md#november-2020) updates for the beta version.

### <a name="identity-and-access"></a>Identity and access
- Specify URLs for sending sign-in user tokens, and URIs for authorization codes and access tokens, in the **spa** property of [application](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true).
- Customize the look and feel of Azure Active Directory sign-in screens through the [organization branding properties](/graph/api/resources/organizationalbrandingproperties?view=graph-rest-beta&preserve-view=true). Organizations can customize based on locale for specific users.

### <a name="identity-and-access--governance"></a>Identity and access | Governance
Debut of [access review API for group membership](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) to review user access regularly, make sure only the right people have continued access, and efficiently manage group memberships.

### <a name="search"></a>Search
You can aggregate numeric or string type search results that are imported by [Microsoft Graph connectors](/microsoftsearch/connectors-overview) and that are set to be refinable in the [schema](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true). See more information about [refining search results using aggregations](search-concept-aggregation.md).

## <a name="october-2020-new-and-generally-available"></a>October 2020: New and generally available

### <a name="application"></a>Application
- Allow [email as an alternate login ID to Azure AD](/azure/active-directory/authentication/howto-authentication-use-email-signin), using a [Home Realm Discovery](/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#home-realm-discovery) policy. A Home Realm Discovery policy determines after a user provides a sign-in ID, whether to prompt the user to authenticate. In this case, setting the **AlternateIdLogin** property of a [homeRealmDiscoveryPolicy](/graph/api/resources/homerealmdiscoverypolicy) resource can enable a user to sign in with an email address.
- Get the verified publisher information for an [application](/graph/api/resources/application) or [servicePrincipal](/graph/api/resources/serviceprincipal), and [set](/graph/api/application-setverifiedpublisher) or [remove](/graph/api/application-unsetverifiedpublisher) verified publisher information for an **application**.

### <a name="change-notifications"></a>Change notifications
Production apps can now subscribe to lifecycle notifications of Outlook [message](/graph/api/resources/message), [event](/graph/api/resources/event), and [contact](/graph/api/resources/contact), and Teams [chatMessage](/graph/api/resources/chatmessage), in order to [reduce missing subscriptions and change notifications](webhooks-lifecycle.md).

### <a name="identity-and-access"></a>Identity and access
- GA of advanced OData system query options (`$count`, `$search`, and `$filter`) on directory objects.
- Check out examples that show OData cast on directory objects.
- See the Identity and access section of the [October](changelog.md#october-2020) updates in the changelog for the lists of enhanced APIs.

### <a name="teamwork"></a>Teamwork
- GA of the full set of CRUD operations for [conversationMember](/graph/api/resources/conversationmember) and [aadUserConversationMember](/graph/api/resources/aaduserconversationmember). These resources represent a member in a chat or channel conversation, who may or may not be a user in Azure AD.
- GA of lifecycle notifications for Teams [chatMessage](/graph/api/resources/chatmessage) resources, to [reduce missing subscriptions and change notifications](webhooks-lifecycle.md).

### <a name="to-do-tasks"></a>To-do tasks
GA of the [Microsoft To Do API](/graph/api/resources/todo-overview?view=graph-rest-1.0&preserve-view=true) - use the to-do API in a production app to create and manage tasks that are part of a user's workflow, such as creating a task off an email.  

### <a name="users"></a>Users
Get new properties applicable to a [user](/graph/api/resources/user) who is corporate employee: hire date, organizational association such as division and cost center, and employee type such as consultant, contractor, or vendor. These properties require specifying the `$select` OData query parameter in the GET operation.

## <a name="october-2020-new-in-preview-only"></a>October 2020: New in preview only

### <a name="cloud-communications--online-meeting"></a>Cloud communications | Online meeting
- Distinguish the role of a participant in an [online meeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) as an attendee or presenter, by using the **role** property of the [meetingParticipantInfo](/graph/api/resources/meetingParticipantInfo?view=graph-rest-beta&preserve-view=true) type.
- Get an [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) by [filtering on the joinWebUrl property of the meeting](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true#example-3-retrieve-an-online-meeting-by-joinweburl).

### <a name="devices-and-apps--cloud-printing"></a>Devices and apps | Cloud printing

- Deprecate the **uploadData** action in favor of [creating an upload session](/graph/api/printdocument-createuploadsession?view=graph-rest-beta&preserve-view=true) to [upload a document](upload-data-to-upload-session.md) to a printer or printer share.
- Deprecate the **configuration** property on [printDocument](/graph/api/resources/printdocument?view=graph-rest-beta&preserve-view=true) in favor of a similar **configuration** property on [printJob](/graph/api/resources/printjob?view=graph-rest-beta&preserve-view=true).
- Get the source or destination job URL for a **printJob** that is being redirected, by using the **redirectedFrom** or **redirectedTo** property.
- Get the current status of a **printJob** by using the **state** property and new **details** property.
- Get the collection of printer shares associated with a [printer](/graph/api/resources/printer?view=graph-rest-beta&preserve-view=true) by using the **shares** relationship. 
- Deprecate the **processingStateReasons** property of **printer** in favor of the **status** property. The **status** property is of the type [printer status](/graph/api/resources/printerstatus?view=graph-rest-beta&preserve-view=true) and exposes a **details** property. Use the **details** property to identify the reason for a printer to be in the current state.
- Deprecate the **feedDirections** property on [printerCapabilities](/graph/api/resources/printercapabilities?view=graph-rest-beta&preserve-view=true) in favor of the **feedOrientations** property, to get feed orientations supported by a printer.
- See the cloud printing section of the [October](changelog.md#october-2020) updates in the changelog for a few renaming of API and properties, and a few other deprecations.

### <a name="devices-and-apps--corporate-management"></a>Devices and apps | Corporate management
Intune [October](changelog.md#october-2020) updates for the beta version.

### <a name="files"></a>Files
[Revoke](/graph/api/permission-revokegrants?view=graph-rest-beta&preserve-view=true) access to a [listItem](/graph/api/resources/listitem?view=graph-rest-beta&preserve-view=true) or [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true) granted via a sharing link.

### <a name="identity-and-access--identity-and-sign-in"></a>Identity and access | Identity and sign-in
- Manage [authentication method policies](/graph/api/resources/authenticationmethodspolicies-overview?view=graph-rest-beta&preserve-view=true) to identify users who can use specific multi-factor authentication methods to sign into Azure Active Directory. Configure policies to define the following:
  - The types of FIDO2 security keys that can be used in the Azure AD tenant.
  - The users or groups of users who are allowed to use FIDO2 Security Keys or Passwordless Phone Sign-in to sign in to Azure AD.
- Configure an [email authentication method](/graph/api/resources/emailauthenticationmethod?view=graph-rest-beta&preserve-view=true) for users to self-serve password resets.
- Use [Azure AD B2C](/azure/active-directory-b2c/overview) and [choose a mechanism to configure and let end users authenticate via local accounts](/graph/api/resources/b2cauthenticationmethodspolicy?view=graph-rest-beta&preserve-view=true).
- Use `Policy.ReadWrite.AuthenticationMethod` to read or write an organization's authentication method policies, as a delegated permission on behalf of a signed-in user, or as an application permission without a signed-in user present.
- Specify in an [authorization policy](/graph/api/resources/authorizationpolicy?view=graph-rest-beta&preserve-view=true) if and who can invite external users to an organization.

### <a name="people-and-workplace-intelligence--insights"></a>People and workplace intelligence | Insights 
Administrators can see [examples of using PowerShell cmdlets](insights-customize-item-insights-privacy.md#how-to-configure-item-insights-settings-via-powershell) to customize item insight settings for an organization.

### <a name="teamwork"></a>Teamwork
- Use the instance attribute **channelCreationMode** to indicate that a [channel](/graph/api/resources/channel?preserve-view=true&view=graph-rest-beta#instance-attributes) is being created to serve migration of data. Use the [completeMigration](/graph/api/channel-completemigration?view=graph-rest-beta&preserve-view=true) to indicate migration is over, such that members can post and read messages.
- Use the instance attribute **teamCreationMode** to indicate that a [team](/graph/api/resources/team?preserve-view=true&view=graph-rest-beta#instance-attributes) is being created to serve migration. Use the [completeMigration](/graph/api/team-completemigration?view=graph-rest-beta&preserve-view=true) to indicate migration is over, such that member operations can happen, and members can post messages.

## <a name="september-2020-new-and-generally-available"></a>September 2020: New and generally available

### <a name="calendar"></a>Calendar
GA of the **transactionId** property of the [event](/graph/api/resources/event) resource, which is optionally set by a client app to avoid redundant POST operations in case of client retries to create the same event. This is useful when low network connectivity causes the client to time out before receiving a response from the server for the client's prior create-event request.

### <a name="cloud-communications"></a>Cloud communications
[Delete a participant](/graph/api/participant-delete) from a [call](/graph/api/resources/call). You can use this operation even in situations where it's necessary to delete a participant from an active call.

### <a name="devices-and-apps--corporate-management"></a>Devices and apps | Corporate management
Intune [September](changelog.md#september-2020) updates for the v1.0 version.

### <a name="identity-and-access--directory-management"></a>Identity and access | Directory management
GA of the [administrative units API](/graph/api/resources/administrativeunit) that allow organizations to subdivide their Azure Active Directory, manage and delegate administrative duties to these subdivisions. These subdivisions can represent regions, departments, cost centers, and so on.

### <a name="reports"></a>Reports
[Get a report that includes the count of unique users](/graph/api/reportroot-getemailappusageversionsusercounts) for Outlook 2019 and for Outlook on Microsoft 365.

### <a name="teamwork"></a>Teamwork
- Get the **lastEditedDateTime** property to find out when a sender last edits a [chat message](/graph/api/resources/chatmessage).
- Get the **lastModifiedDateTime** property to find out when a sender creates a chat message or when anyone modifies it in other ways, including adding or removing a reaction. 
- [Get notifications on changes](webhooks.md) in [chat messages](/graph/api/resources/chatmessage).
- [Update](/graph/api/chatmessage-update?view=graph-rest-beta&preserve-view=true) the **policyViolation** property of a [chatMessage](/graph/api/resources/chatmessagepreserve-view=true) within a [channel](/graph/api/resources/channel&preserve-view=true) or [chat](/graph/api/resources/chat&preserve-view=true), enabling data loss prevention (DLP) apps to monitor [chat message policy violation](/graph/api/resources/chatmessagepolicyviolation?preserve-view=true) to prevent messages from containing data that users are not supposed to send.

### <a name="use-the-sdks"></a>Use the SDKs
GA of the [Microsoft Graph PowerShell SDK](https://github.com/microsoftgraph/msgraph-sdk-powershell) which enables access to the entire surface of Microsoft Graph in a straightforward and consistent way.

### <a name="use-the-toolkit"></a>Use the Toolkit
Try the new step-by-step getting-started tutorials for Microsoft Graph Toolkit and experience the convenience the toolkit brings:
- [Build a web application in JavaScript](./toolkit/get-started/build-a-web-app.md)
- [Build a SharePoint web part](./toolkit/get-started/build-a-sharepoint-web-part.md)
- [Build a Microsoft Teams tab](./toolkit/get-started/build-a-microsoft-teams-tab.md)
- [Use the toolkit with React](./toolkit/get-started/use-toolkit-with-react.md)
- [Use the toolkit with Angular](./toolkit/get-started/use-toolkit-with-angular.md)

### <a name="users"></a>Users
Aside from getting the SMTP address of a [user](/graph/api/resources/user) through the **mail** property, you can now set that property and update the user's email address. 

## <a name="september-2020-new-in-preview-only"></a>September 2020: New in preview only

### <a name="application"></a>Application
Create, list, or delete [classifications of delegated permissions](/graph/api/resources/delegatedpermissionclassification?view=graph-rest-beta&preserve-view=true) that a [service principal](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true) exposes. Use delegated permission classifications in combination with [user consent settings](/azure/active-directory/manage-apps/configure-user-consent) to set limits on when end-users are allowed to grant consent to apps.

### <a name="cloud-communications"></a>Cloud communications
- Deprecation of the **autoAdmittedUsers** property of [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true). Instead, use the new **lobbyBypassSettings** property and its [values](/graph/api/resources/lobbybypasssettings?view=graph-rest-beta&preserve-view=true#lobbybypassscope-values).
- Use additional settings about announcing callers joining or leaving an online meeting (**isEntryExitAnnounced** property), and allowing specific presenters in the meeting (**allowedPresenters** property).

### <a name="devices-and-apps--cloud-printing"></a>Devices and apps | Cloud printing
- [Get the documents for each of the print jobs associated with a printer](/graph/api/printer-list-jobs?view=graph-rest-beta&preserve-view=true), by applying an `$expand` [OData system query option](/graph/api/printer-list-jobs?view=graph-rest-beta&preserve-view=true#optional-query-parameters). 
- Filter print jobs by the user who created them, by applying a `$filter` [OData system query option](/graph/api/printer-list-jobs?view=graph-rest-beta&preserve-view=true#optional-query-parameters).

### <a name="devices-and-apps--corporate-management"></a>Devices and apps | Corporate management
Intune [September](changelog.md#september-2020) updates for the beta version.

### <a name="identity-and-access--directory-management"></a>Identity and access | Directory management
- [Get a BitLocker recovery key](/graph/api/bitlockerrecoverykey-get?view=graph-rest-beta&preserve-view=true) on behalf of the signed-in user who's the device owner or in an appropriate role. Getting a recovery key generates an [audit log](/azure/active-directory/reports-monitoring/concept-audit-logs), in parity with the end user experience.
- Get the total and used amount of the [directory quota](/graph/api/resources/directorysizequota?view=graph-rest-beta&preserve-view=true) of an [organization](/graph/api/resources/organization?view=graph-rest-beta&preserve-view=true), through the **directorySizeQuota** property.

### <a name="identity-and-access--governance"></a>Identity and access | Governance
Be able to include a [schedule](/graph/api/resources/requestschedule?view=graph-rest-beta&preserve-view=true) when requesting or removing an [assignment of a user to an access package](/graph/api/resources/accesspackageassignment?view=graph-rest-beta&preserve-view=true), that specifies access to groups, applications, or SharePoint sites.

### <a name="identity-and-access--identity-and-sign-in"></a>Identity and access | Identity and sign-in
Organizations can [get](/graph/api/continuousaccessevaluationpolicy-get?view=graph-rest-beta&preserve-view=true) or [update](/graph/api/continuousaccessevaluationpolicy-update?view=graph-rest-beta&preserve-view=true) a [continuous access evaluation policy](/graph/api/resources/continuousAccessEvaluationPolicy?view=graph-rest-beta&preserve-view=true) to manage authentication sessions in real time.

### <a name="search"></a>Search

- Use additional capabilities in the [Microsoft Search API](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true) for OneDrive, SharePoint, Microsoft Graph connectors: 

  - Get [additional types](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true#scope-search-based-on-entity-types) of content from OneDrive and SharePoint: **drive**, **list**, **listItem**, and **site**. 
  - Scope properties in search results to [selected properties](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true#get-selected-properties). 
  - Get custom properties on [listItem](/graph/api/resources/listitem?view=graph-rest-beta&preserve-view=true) resources.
  - [Sort](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true#sort-search-results) search results for OneDrive and SharePoint on any sortable property.
  - [Refine results using aggregations](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true#refine-results-using-aggregations) for OneDrive and SharePoint.
- Query external data ingested by Microsoft Graph connectors across [more than one connection](./search-concept-custom-types.md).
- Take advantage of enhanced content for Microsoft Graph connectors to learn about:
  - [Managing connections](connecting-external-content-manage-connections.md)
  - [Managing schema](connecting-external-content-manage-schema.md)
  - [Managing items](connecting-external-content-manage-items.md)
- Track the state of a Microsoft Graph [connection](/graph/api/resources/externalconnection?view=graph-rest-beta&preserve-view=true).
- Define an [external group](/graph/api/resources/externalgroup?view=graph-rest-beta&preserve-view=true) to set permissions on [external item](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) objects added to a Microsoft Graph [connection](/graph/api/resources/externalconnection?view=graph-rest-beta&preserve-view=true). External groups can represent non-Azure Active Directory groups or group-like constructs, such as business units, that determine permissions over the content in the external data source.

### <a name="teamwork"></a>Teamwork
- Get the date/time at which a Teams [channel](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true) or [team](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true) is created.


## <a name="august-2020-new-and-generally-available"></a>August 2020: New and generally available

### <a name="change-notifications"></a>Change notifications
[Acompanhar alterações](delta-query-overview.md) de recursos com suporte no Microsoft Graph para a nuvem nacional do governo dos EUA.

### <a name="cloud-communications"></a>Cloud communications
- [Cancel](/graph/api/call-cancelmediaprocessing) any Interactive Voice Response (IVR) actions that are in process or in queue, that are either [playing an audio prompt](/graph/api/call-playprompt) or [recording a response](/graph/api/call-record).
- Get [call transcription information](/graph/api/resources/calltranscriptioninfo) through the **transcription** property.

### <a name="teamwork"></a>Teamwork
- Use an alternative way to [create a team](/graph/api/team-post) directly without first creating a group.
- Use the **members** navigation property to add members to a team with increased reliability and lower latency.
- Get the publishing status of a Microsoft Teams [app](/graph/api/resources/teamsapp) through the **publishingState** property of the [app definition](/graph/api/resources/teamsappdefinition). The possible status values are `submitted`, `published`, and `rejected`. See an [example](/graph/api/teamsapp-list?view=graph-rest-beta&preserve-view=true#example-3-list-applications-with-a-given-id-and-return-the-submission-review-state).
- Use the `AppCatalog.Submit` delegated permission to allow a user to [submit an app](/graph/api/teamsapp-publish) and request administrator review. Use the same permission for a user to [cancel](/graph/api/teamsapp-delete) an app submitted in the past that has not been published. 


## <a name="august-2020-new-in-preview-only"></a>August 2020: New in preview only

### <a name="applications"></a>Applications
Support password-based single-sign-on in [service principal](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true) application resources and specify such [settings](/graph/api/resources/passwordsinglesignonsettings?view=graph-rest-beta&preserve-view=true) in the **passwordSingleSignOnSettings** property. For information about password-based single sign-on in Azure AD, see [configure password-based single-sign-on](/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications).

### <a name="calendar"></a>Calendar
Enhance programmatic support for scenarios involving a recurring [event](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true):
- Reliably identify any occurrence in a recurring series, including a modified or cancelled occurrence, by using the **occurrenceId** property.
- Get any exceptions in a recurring series by using the **exceptionOccurrences** property.
- Get any cancellations in a series using the **cancelledOccurrences** property.

### <a name="change-notifications"></a>Change notifications
- Use the **includeResourceData** property of a [subscription](/graph/api/resources/subscription?view=graph-rest-beta&preserve-view=true), to [set up change notifications that include resource data](webhooks-with-resource-data.md). Do not use the **includeProperties** property.
- Get [change notifications delivered via Event Hub](change-notifications-delivery.md).

### <a name="devices-and-apps--cloud-printing"></a>Devices and apps | Cloud printing
- Grant all users and groups access to a [printer share](/graph/api/resources/printershare?view=graph-rest-beta&preserve-view=true) by using the **allowAllUser** property.
- Use new delegated and application permissions to access or manage a [print document](/graph/api/resources/printDocument?view=graph-rest-beta&preserve-view=true), [print job](/graph/api/resources/printjob?view=graph-rest-beta&preserve-view=true), [printer](/graph/api/resources/printer?view=graph-rest-beta&preserve-view=true), [printer share](/graph/api/resources/printershare?view=graph-rest-beta&preserve-view=true), or [print task definition](/graph/api/resources/printtaskdefinition?view=graph-rest-beta&preserve-view=true). For details, see cloud printing [August](changelog.md#august-2020) updates.

### <a name="devices-and-apps--corporate-management"></a>Devices and apps | Corporate management
Intune [August](changelog.md#august-2020) updates in beta.

### <a name="identity-and-access--governance"></a>Identity and access | Governance
- Customize a [terms of use agreement](/graph/api/resources/agreement?view=graph-rest-beta&preserve-view=true) to support an agreement expiration date and cadence, require the user to accept the agreement per device, or to re-accept the agreement on a set frequency. 
- Use the **file** property to navigate to a [custom agreement](/graph/api/resources/agreementfile?view=graph-rest-beta&preserve-view=true) for terms of use. Do not use the **files** property.
- Add, remove, and list internal or external sponsors who can approve requests from a [connected organization](/graph/api/resources/connectedorganization?view=graph-rest-beta&preserve-view=true) to access a group, application, or SharePoint Online site. See [entitlement management](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta&preserve-view=true) for more information.

### <a name="identity-and-access--identity-and-sign-in"></a>Identity and access | Identity and sign-in
- Enable further customizing an [authorization policy](/graph/api/resources/authorizationpolicy?view=graph-rest-beta&preserve-view=true) for a tenant, such as allowing the [default user role](/graph/api/resources/defaultuserrolepermissions?view=graph-rest-beta&preserve-view=true) to create applications or security groups or to read other users, allowing users to sign up for email-based subscriptions or to join the tenant by email validation, or letting users self-serve password resets.
- Manage [predefined, configurable policies as user flows within an Azure Active Directory B2C tenant](/graph/api/resources/b2cuserflows?view=graph-rest-beta&preserve-view=true). See more information about [B2C user flows](/azure/active-directory-b2c/user-flow-overview).
- Enable [self-service sign-up experience as B2X user flows in an Azure Active Directory tenant](/graph/api/resources/b2xuserflows?view=graph-rest-beta&preserve-view=true). See more information about [self-service sign-up](/azure/active-directory/external-identities/self-service-sign-up-overview).

### <a name="people-and-workplace-intelligence--profile"></a>People and workplace intelligence | Profile
Add and manage the following additional properties in a user's [profile](/graph/api/resources/profile?view=graph-rest-beta&preserve-view=true), and that can be surfaced in shared, people experiences across Microsoft 365 and third-party apps:
- [addresses](/graph/api/resources/itemAddress?view=graph-rest-beta&preserve-view=true)
- [anniversaries](/graph/api/resources/personAnniversary?view=graph-rest-beta&preserve-view=true)
- [awards](/graph/api/resources/personAward?view=graph-rest-beta&preserve-view=true)
- [certifications](/graph/api/resources/personCertification?view=graph-rest-beta&preserve-view=true)
- [notes](/graph/api/resources/personAnnotation?view=graph-rest-beta&preserve-view=true)
- [patents](/graph/api/resources/itemPatent?view=graph-rest-beta&preserve-view=true)
- [publications](/graph/api/resources/itemPublication?view=graph-rest-beta&preserve-view=true)


### <a name="reports--microsoft-365-usage-reports"></a>Reports | Microsoft 365 usage reports
Get [reports on Microsoft 365 apps usage](/graph/api/resources/microsoft-365-apps-usage-report?view=graph-rest-beta&preserve-view=true), specifically on user detail, user counts, and platform user counts.

### <a name="teamwork"></a>Teamwork
Get [content hosted in a chat message](/graph/api/resources/chatMessageHostedContent?view=graph-rest-beta&preserve-view=true), such as images or code snippets. See an [example](/graph/api/chatmessagehostedcontent-get?view=graph-rest-beta&preserve-view=true&branch=master#example-2-get-hosted-content-bytes-for-an-image) to get the content bytes of an image.

### <a name="to-do-tasks"></a>To-do tasks
- Debut of a new set of API for [Microsoft To Do](todo-concept-overview.md), allowing app users to organize and track personal tasks across Microsoft 365 client apps. See [Use the Microsoft To Do API](/graph/api/resources/todo-overview?view=graph-rest-beta&preserve-view=true) for more information.
- Deprecation of the [Outlook tasks API](/graph/api/resources/outlooktask?view=graph-rest-beta&preserve-view=true).


## <a name="july-2020-new-and-generally-available"></a>July 2020: New and generally available

### <a name="calendar"></a>Calendar
GA of the feature that allows organizers to allow alternate meeting time proposals, and invitees to [propose new times for a meeting](outlook-calendar-meeting-proposals.md) when they [tentatively accept](/graph/api/event-tentativelyaccept?view=graph-rest-1.0&preserve-view=true&preserve-view=true) or [decline](/graph/api/event-decline?view=graph-rest-1.0&preserve-view=true&preserve-view=true) an event.

### <a name="change-notifications"></a>Change notifications
Removed the erroneously introduced **sequenceNumber** property from the [changeNotification](/graph/api/resources/changenotification) resource.

### <a name="groups"></a>Groups
GA of the following properties for the [group](/graph/api/resources/group) entity: **assignedLabels**, **expirationDateTime**, **membershipRule**, **membershipRuleProcessingState**, **preferredLanguage**, and **theme**.

### <a name="identity-and-access"></a>Identity and access
- Remove a user as a registered owner or user of a [device](/graph/api/resources/device).
- Track changes to newly created, updated, or deleted local representation of applications (represented by [servicePrincipals](/graph/api/resources/serviceprincipal) resources) and delegated permissions grants (represented by [oAuth2PermissionGrant](/graph/api/resources/oauth2permissiongrant) resources) without performing a full read of the entire resource collection.
- GA of the [policy to enforce security defaults](/graph/api/resources/identitysecuritydefaultsenforcementpolicy) that protect organizations against common attacks.

### <a name="identity-and-access--identity-and-sign-in"></a>Identity and access | Identity and sign-in
- GA of [conditional access policies](/graph/api/resources/conditionalAccessPolicy) that are custom rules that define an access scenario.
- GA of [named locations](/graph/api/resources/namedLocation) representing custom rules that define network locations used in a conditional access policy.

### <a name="schema-extensions"></a>Schema extensions
The [schema extensions](/graph/api/resources/schemaextension) feature is now generally available in [Microsoft Cloud for US Government](./deployments.md).

### <a name="teamwork"></a>Teamwork
Use the delegated permissions of `TeamsAppInstallation.ReadForTeam` or `TeamsAppInstallation.ReadWriteForTeam`, or application permissions of `TeamsAppInstallation.ReadForTeam.All` or `TeamsAppInstallation.ReadWriteForTeam.All` to [list apps that are installed in a team](/graph/api/teamsappinstallation-list).

## <a name="july-2020-new-in-preview-only"></a>July 2020: New in preview only

### <a name="cloud-communications"></a>Cloud communications
- Use the [update](/graph/api/onlinemeeting-update?view=graph-rest-beta&preserve-view=true&preserve-view=true) operation to update the **startDateTime**, **endDateTime**, **participants**, or **subject** property of an [online meeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true&preserve-view=true).
- Subscribe to notifications on changes to the availability of a user on Microsoft Teams, as represented by the [presence](/graph/api/resources/presence?view=graph-rest-beta&preserve-view=true) resource.

### <a name="cloud-communications--call-records"></a>Cloud communications | Call records
- [Get](/graph/api/callrecords-callrecord-getpstncalls?view=graph-rest-beta&preserve-view=true) records of Public Switch Telephone Network (PSTN) calls.
- [Get](/graph/api/callrecords-callrecord-getdirectroutingcalls?view=graph-rest-beta&preserve-view=true) records of direct routing calls.

### <a name="compliance--ediscovery"></a>Compliance | eDiscovery
Debut of [eDiscovery cases](/graph/api/resources/ediscoverycase?view=graph-rest-beta&preserve-view=true) that can contain custodians, holds, collections, review sets, and exports that can be used as evidence in legal cases.
Apps can now [query](/graph/api/resources/reviewsetquery?view=graph-rest-beta&preserve-view=true) and cull [review set data](/graph/api/resources/reviewset?view=graph-rest-beta&preserve-view=true) collected for use in a litigation, investigation, or regulatory request. This debut is part of Microsoft 365 [Advanced eDiscovery](/microsoft-365/compliance/overview-ediscovery-20?view=o365-worldwide&preserve-view=true).

### <a name="devices-and-apps--cloud-printing"></a>Devices and apps | Cloud printing
- Use the application permission `Printer.ReadWrite.All` and [Internet Printing Protocol (IPP) encoding](https://tools.ietf.org/html/rfc8010) to [update a printer](/graph/api/printer-update?view=graph-rest-beta&preserve-view=true).
- Use one of the application permissions, `PrintJob.ReadBasic.All`, `PrintJob.Read.All`, `PrintJob.ReadWriteBasic.All`, or `PrintJob.ReadWrite.All`, to [get a print job](/graph/api/printjob-get?view=graph-rest-beta&preserve-view=true) or [list print jobs for a printer](/graph/api/printer-list-jobs?view=graph-rest-beta&preserve-view=true).
- When [getting a print job](/graph/api/printjob-get?view=graph-rest-beta&preserve-view=true), use `$expand` to get [print tasks](/graph/api/resources/printtask?view=graph-rest-beta&preserve-view=true) that are executing or have executed against the job. Print tasks, [task definitions](/graph/api/resources/printtaskdefinition?view=graph-rest-beta&preserve-view=true), and [task triggers](/graph/api/resources/printtasktrigger?view=graph-rest-beta&preserve-view=true) are used in [pull printing](universal-print-concept-overview.md#extending-universal-print-to-support-pull-printing).
- [Redirect a print job](/graph/api/printjob-redirect?view=graph-rest-beta&preserve-view=true) to a different printer, as part of pull printing.

### <a name="devices-and-apps--corporate-management"></a>Devices and apps | Corporate management
Intune [July](changelog.md#july-2020) updates in beta.

### <a name="groups"></a>Groups
Use the **isAssignableToRole** property of a Microsoft 365 [group](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) and set it during group creation to indicate whether the group can be assigned to an Azure AD role. This [helps manage role assignments in Azure AD](/azure/active-directory/users-groups-roles/roles-groups-concept), such that instead of assigning individual users an Azure AD role, a privileged role admin or global admin can create a Microsoft 365 group and assign the group that role, so that when users join the _group_, they are assigned the intended role indirectly.

### <a name="identity-and-access"></a>Identity and access
- [Acquire an access token](/graph/api/synchronization-synchronization-acquireAccessToken?view=graph-rest-beta&preserve-view=true) to authorize the Azure AD provisioning service to provision users into an application.
- [Get](/graph/api/entitlementmanagementsettings-get?view=graph-rest-beta&preserve-view=true) or [update](/graph/api/entitlementmanagementsettings-update?view=graph-rest-beta&preserve-view=true) entitlement management settings that control access to groups, applications, and SharePoint Online sites for users internal and external to your organization. 

### <a name="identity-and-access--identity-and-sign-in"></a>Identity and access | Identity and sign-in
- Include user risk levels (`low`, `medium`, `high`, `none`) as a consideration for applying a [conditional access policy](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true).
- [Use password change as a grant control](/graph/api/resources/conditionalaccessgrantcontrols?view=graph-rest-beta&preserve-view=true#special-considerations-when-using-passwordchange-as-a-control) in order to pass a conditional access policy.
- Use an [Open ID Connect provider](/graph/api/resources/openidconnectprovider?view=graph-rest-beta&preserve-view=true) (ODIC) as an identity provider in an Azure AD tenant and an Azure AD B2C tenant. Its **claimsMapping** property allows Azure AD to [map the claims](/graph/api/resources/claimsmapping?view=graph-rest-beta&preserve-view=true) from an OIDC provider to the claims that Azure AD recognizes and uses.

### <a name="people-and-workplace-intelligence--insights"></a>People and workplace intelligence | Insights
Use more [granular privacy control](insights-customize-item-insights-privacy.md) over the availability and display of [item insights](/graph/api/resources/iteminsights?view=graph-rest-beta&preserve-view=true) in Microsoft 365. These insights represent the relationships between a user and documents in OneDrive for Business, calculated using advanced analytics and machine learning techniques. 

### <a name="people-and-workplace-intelligence--profile-card-customization"></a>People and workplace intelligence | Profile card customization
Administrators can [customize the properties exposed on the profile card for their organizations](add-properties-profilecard.md) by using the API for [profile card property](/graph/api/resources/profilecardproperty?view=graph-rest-beta&preserve-view=true).

### <a name="sites-and-lists"></a>Sites and lists
Access the SharePoint [term store](/graph/api/resources/termstore-store?view=graph-rest-beta&preserve-view=true) taxonomy, the hierarchy that consists of [group](/graph/api/resources/termstore-group?view=graph-rest-beta&preserve-view=true), [set](/graph/api/resources/termstore-set?view=graph-rest-beta&preserve-view=true), and [term](/graph/api/resources/termstore-term?view=graph-rest-beta&preserve-view=true) resources, and [relation](/graph/api/resources/termstore-relation?view=graph-rest-beta&preserve-view=true) resources between terms.

### <a name="workbooks-and-charts"></a>Workbooks and charts
[Get the status and any result](/graph/api/workbookoperation-get?view=graph-rest-beta&preserve-view=true) of a long running [operation](/graph/api/resources/workbookoperation?view=graph-rest-beta&preserve-view=true) in a [workbook](/graph/api/resources/workbook?view=graph-rest-beta&preserve-view=true).



## <a name="june-2020-new-and-generally-available"></a>June 2020: New and generally available

### <a name="cloud-communications--online-meeting"></a>Cloud communications | Online meeting
- Use the `Accept-Language` HTTP header when [creating an online meeting](/graph/api/application-post-onlinemeetings?view=graph-rest-1.0&preserve-view=true&preserve-view=true) to provide locale-based join information.
- Use [createOrGet](/graph/api/onlinemeeting-createorget?view=graph-rest-1.0&preserve-view=true&preserve-view=true) to return an online meeting that has a specified **externalId** value, or create one if none already exists, to streamline embedding the resultant meeting in a third-party calendar.

### <a name="files"></a>Files
- Enhanced synchronization support:
  - Use the **pendingOperations** property to identify any [operations](/graph/api/resources/pendingoperations) that might update the binary content of a [driveItem](/graph/api/resources/driveitem) file, that are pending completion.
  - [Restore](/graph/api/driveitem-restore) a **driveItem** that has been deleted and is in the recycle bin on OneDrive Personal.
- Get or set the orientation of a [photo](/graph/api/resources/photo). Setting is supported on OneDrive Personal.
- Use Secure Hash Algorithm (SHA-256) to enhance [file](/graph/api/resources/file) data security and integrity.
- Use the `deferCommit` parameter to defer final creation when [uploading typically a large file](/graph/api/driveitem-createuploadsession) to OneDrive for Business, until an app makes a request to complete the upload.
- Use the **fileSize** property to provide as part of the **item** parameter an estimate, so to do a quota check prior to [uploading a file](/graph/api/driveitem-createuploadsession) on OneDrive Personal.
- Find [storagePlanInformation](/graph/api/resources/storageplaninformation) through the **quota** property of a [drive](/graph/api/resources/drive) resource to see if there are higher storage quota plans available.

### <a name="groups"></a>Groups
Use application permissions `Group.Read.All` and `Group.ReadWrite.All` to get group [conversation](/graph/api/resources/conversation) and [conversation thread](/graph/api/resources/conversationthread) resources.

### <a name="identity-and-access"></a>Identity and access 
- GA of two sets of API for [identity protection](/graph/api/resources/identityprotectionroot): [risk detection](/graph/api/resources/riskdetection) and [risky user](/graph/api/resources/riskyuser) APIs.

### <a name="security"></a>Security
- Track the following as properties of an [alert](/graph/api/resources/alert?view=graph-rest-1.0&preserve-view=true&preserve-view=true):
  - IDs of incidents related to the alert.
  - Identify a [resource](/graph/api/resources/securityResource?view=graph-rest-1.0&preserve-view=true#securityresourcetype-values) as attacked or as a related resource in the alert.
  - Specify the source and destination locations of a [network connection](/graph/api/resources/networkconnection?view=graph-rest-1.0&preserve-view=true) related to the alert.

### <a name="sites-and-lists"></a>Sites and lists
Specify geolocation data in a [column definition](/graph/api/resources/columndefinition) for a SharePoint [list](/graph/api/resources/list) resource.

### <a name="teamwork"></a>Teamwork
- Use the delegated permission [AppCatalog.Read.All](./permissions-reference.md#appcatalog-resource-permissions) to list [apps](/graph/api/resources/teamsapp?view=graph-rest-1.0&preserve-view=true) from the Microsoft Teams app catalog.
- [Get information about the folder](/graph/api/channel-get-filesfolder) that maps to the **Files** tab of a Teams [channel](/graph/api/resources/channel).
- [Get the default channel](/graph/api/team-get-primarychannel), labelled as **General**, of a [team](/graph/api/resources/team).


## <a name="june-2020-new-in-preview-only"></a>June 2020: New in preview only

### <a name="calendar"></a>Calendar
In addition to tracking incremental changes on events in a **calendarView** (collection or events delimited by start _and_ end dates), use the [delta](/graph/api/event-delta?view=graph-rest-beta&preserve-view=true) function on events in a user mailbox, or events in a specific user calendar.

### <a name="cloud-communications--presence"></a>Cloud communications | Presence
[Get the presence status](/graph/api/presence-get?view=graph-rest-beta&preserve-view=true) of all the users in an organization, or a specific user in the organization.

### <a name="devices-and-apps--cloud-printing"></a>Devices and apps | Cloud printing
- Specify [print margins](/graph/api/resources/printmargin?view=graph-rest-beta&preserve-view=true) when configuring a [document for printing](/graph/api/resources/printdocument?view=graph-rest-beta&preserve-view=true).
- Support for the following [printer capabilities](/graph/api/resources/printercapabilities?view=graph-rest-beta&preserve-view=true):
  - feed directions
  - printing page ranges
  - print resolution in DPI
  - maximum print job queue size in bytes
  - input bins
  - margins
  - collation
  - document scaling
- Support for print resolution (DPI) and document scaling as part of [default printer settings](/graph/api/resources/printerdefaults?view=graph-rest-beta&preserve-view=true).
- Support for the following [document configuration](/graph/api/resources/printerdocumentconfiguration?view=graph-rest-beta&preserve-view=true) settings:
  - input bins
  - output bins
  - media sizes
  - margins
  - media types
  - finishings such as stapling or binding
  - pages per sheet
  - multi-page layout specifying the direction to lay out pages per sheet
  - collation
  - scaling
- Expand documents when [listing pring jobs](/graph/api/printer-list-jobs?view=graph-rest-beta&preserve-view=true).
- [Register a printer]() and use the [printerCreateOperation](/graph/api/resources/printercreateoperation?view=graph-rest-beta&preserve-view=true) resource to track and verify the registration of the printer.
- [Get long-running printer registration operation](/graph/api/printoperation-get?view=graph-rest-beta&preserve-view=true) within current user or app's tenant.
- A few renaming of properties and enum types - see details in the [June](changelog.md#june-2020) changelog updates for cloud printing.

### <a name="devices-and-apps--corporate-management"></a>Devices and apps | Corporate management
Intune [June](changelog.md#june-2020) updates in beta.

### <a name="education"></a>Education
- Can use delegated permissions `EduRoster.ReadBasic` to [get](/graph/api/educationuser-get?view=graph-rest-beta&preserve-view=true) the ID of a [teacher](/graph/api/resources/educationteacher?view=graph-rest-beta&preserve-view=true) or [student](/graph/api/resources/educationstudent?view=graph-rest-beta&preserve-view=true) in an external source program, as the **externalId** property.
- Use the **externalSource** property to track the value `lms` if an education [organization](/graph/api/resources/educationorganization?view=graph-rest-beta&preserve-view=true) or [class](/graph/api/resources/educationclass?view=graph-rest-beta&preserve-view=true) is created from a learning management system (LMS).

### <a name="identity-and-access"></a>Identity and access
- IT professionals can use [connector](/graph/api/resources/connector?view=graph-rest-beta&preserve-view=true) resources that are lightweight agents to connect to [Azure AD Application Proxy](/azure/active-directory/manage-apps/what-is-application-proxy), and [publish on-premises web applications apps externally](/graph/api/resources/onpremisespublishing?view=graph-rest-beta&preserve-view=true), so that remote users of their organizations can access these apps in a secure manner.
- Manage an [authentication policy](/graph/api/resources/authenticationflowspolicy?view=graph-rest-beta&preserve-view=true) at a tenant level, to enable or disable [self-service sign-up](/graph/api/resources/selfservicesignupauthenticationflowconfiguration?view=graph-rest-beta&preserve-view=true) of external users.
- [Provision a user account on demand](/graph/api/synchronization-synchronizationjob-provision-on-demand?view=graph-rest-beta&preserve-view=true), and be able to specify the objects to provision and synchronization rules to execute.

### <a name="search"></a>Search
- Make use of enhancements on a [property](/graph/api/resources/property?view=graph-rest-beta&preserve-view=true) in a [schema](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true): **isRefinable** to enable filtering of search results and for a more refined control of the search experience, and **aliases** and **labels** for better relevance.
- Be able to specify up to 128 **property** resources in a **schema**.
- Use [get externalItem](/graph/api/externalitem-get?view=graph-rest-beta&preserve-view=true) for diagnostic purposes.

### <a name="users"></a>Users
- Use the **userPurpose** property of [mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-beta&preserve-view=true) to identify and differentiate a mailbox for a single user from a shared mailbox and equipment mailbox in Exchange Online. 
- Use [user settings](/graph/api/resources/usersettings?view=graph-rest-beta&preserve-view=true) to [get](/graph/api/regionalandlanguagesettings-get?view=graph-rest-beta&preserve-view=true) or [update](/graph/api/regionalandlanguagesettings-update?view=graph-rest-beta&preserve-view=true) [preferred languaes and regional settings](/graph/api/resources/regionalandlanguagesettings?view=graph-rest-beta&preserve-view=true).
- User settings is a relationship accessible through [user](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true) that enables a consistent user experience across apps, by tapping into the Azure AD user profile to reflect the same user preferences. See [how user settings differentiate from mailbox settings](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true#user-preferences-for-languages-and-regional-formats).


## <a name="may-2020-new-and-generally-available"></a>May 2020: New and generally available

### <a name="calendar--place"></a>Calendar | Place
GA of the [places API](/graph/api/resources/place) in v1.0 - use this API in production apps to get, update, or delete a [room](/graph/api/resources/room) or [room list](/graph/api/resources/roomlist) in a tenant. [Find out more](outlook-calendar-concept-overview.md#build-apps-with-location-awareness-and-provide-intelligent-context) about the places API.

### <a name="change-notifications"></a>Change notifications
- Subscribe to change notifications in Microsoft Cloud for US Government.

### <a name="cloud-communications--call-records"></a>Cloud communications | Call records
- GA of the [call records API](/graph/api/resources/callrecords-api-overview?view=graph-rest-1.0&preserve-view=true) - use the [callRecord](/graph/api/resources/callrecord?view=graph-rest-1.0&preserve-view=true) resource to get the metadata of calls and online meetings on Microsoft Teams and Skype.
- Subscribe to [change notifications](./webhooks.md) for changes to all **callRecord** resources in an organization.
- [List sessions](/graph/api/callrecords-session-list?view=graph-rest-1.0&preserve-view=true) in a **callRecord**, and optionally [expand each session to list segments](/graph/api/callrecords-session-list?view=graph-rest-1.0&preserve-view=true#example-2-get-session-list-with-segments) in the call record.
- Support for 60-GHz (`frequency60GHz`) and `unknownFutureValue` WiFi band values of a media endpoint in a segment.
- Support for voice mail as a possible type of service-side end point in a communication [segment](/graph/api/resources/callrecords-segment).

### <a name="devices-and-apps--corporate-management"></a>Devices and apps | Corporate management
Intune [May](changelog.md#may-2020) updates in v1.0.

### <a name="graph-explorer"></a>Graph Explorer
Use the many new features of [Graph Explorer](https://developer.microsoft.com/pt-BR/graph/graph-explorer) that enhance learning and prototyping in the sandbox. For example:
- View code snippets that correspond to the REST API query you entered, in C#, Java, JavaScript, and Objective C.
- Signed in with a tenant, view and copy an access token to your favorite REST client application.

See [New Graph Explorer is now GA](https://developer.microsoft.com/graph/blogs/new-graph-explorer-is-now-ga/) for more details.

### <a name="groups"></a>Groups
- Synchronizing on-premises directory to Azure Active Directory via Azure AD Connect now returns the **onPremisesDomainName**, **onPremisesNetBiosName** and **onPremisesSamAccountName** properties as part of the [group](/graph/api/resources/group?view=graph-rest-1.0&preserve-view=true) resource.
- Subscribe to change notifications for [group](/graph/api/resources/group) resources in Microsoft Cloud China operated by 21Vianet.

### <a name="identity-and-access"></a>Identity and access
- GA of the service principals API in v1.0 - use the [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0&preserve-view=true) resource in production apps to programmatically manage instances of applications and control what an application can do within your tenant. You can control who can use an application, what resources the application has access to, such as adding password credentials, rolling expiring certificates, and managing delegated permission grants and application role assignments.
- GA of the [appRoleAssignment](/graph/api/resources/appRoleAssignment?view=graph-rest-1.0&preserve-view=true) API, which records the assignment of an [appRole](/graph/api/resources/approle?view=graph-rest-1.0&preserve-view=true) (representing the `roles` claim in ID tokens and access tokens) to a [user](/graph/api/resources/user?view=graph-rest-1.0&preserve-view=true), [group](/graph/api/resources/group?view=graph-rest-1.0&preserve-view=true), or [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0&preserve-view=true).
- Use Facebook as an identity provider on Azure Active Directory.
- Use the delegated or application permission of `AppRoleAssignment.ReadWrite.All` to allow an app to manage grants for application permissions to any API (including Microsoft Graph) and application assignments for any app, respectively with or without the signed-in user.


### <a name="microsoft-graph-sdks"></a>Microsoft Graph SDKs
See new SDK guidance on the following:
- [Paging](./sdks/paging.md)
- [Batching](./sdks/batch-requests.md)
- [Uploading large files on OneDrive](./sdks/large-file-upload.md)
- [Customizing SDK service client through HTTP middleware components](./sdks/customize-client.md).

### <a name="teamwork"></a>Teamwork
- If your scenario involves online meetings on Teams, see new guidance on [how to choose](choose-online-meeting-api.md) between the [calendar API](outlook-calendar-online-meetings.md) and [cloud communications API](cloud-communications-online-meetings.md) to create and join online meetings.
- [Send](/graph/api/channel-post-messages?view=graph-rest-1.0&preserve-view=true) and [reply](/graph/api/channel-post-messagereply?view=graph-rest-1.0&preserve-view=true) to messages in a [channel](/graph/api/resources/channel?view=graph-rest-1.0&preserve-view=true).
- Get the OneDrive for Business location of the files for a [channel](/graph/api/resources/channel?view=graph-rest-1.0&preserve-view=true), by using the **fileFolder** navigation property.

### <a name="teamwork--shifts"></a>Teamwork | Shifts
GA of the [shifts API](/graph/api/resources/shift?view=graph-rest-1.0&preserve-view=true) in v1.0 - use this API in production apps to create, update, and manage schedules of firstline workers, to let them stay in touch and collaborate effectively.

### <a name="users"></a>Users
- Subscribe to change notifications for [user](/graph/api/resources/user) resources in Microsoft Cloud China operated by 21Vianet.
- Track the status and date/time of the last status change of an external user, who has been [invited](/graph/api/invitation-post?view=graph-rest-1.0&preserve-view=true) to join the organization, by using the **externalUserState** and **externalUserStateChangeDateTime** properties of the **user** resource.

## <a name="may-2020-new-in-preview-only"></a>May 2020: New in preview only

### <a name="change-notifications"></a>Change notifications
- Use formally schematized types [changeNotification](/graph/api/resources/changenotification?view=graph-rest-beta&preserve-view=true) and [changeNotificationCollection](/graph/api/resources/changenotificationcollection?view=graph-rest-beta&preserve-view=true) to process resource change notifications. 
- Track if notifications are in sequence or if a notification is missing by using the **sequenceNumber** property on the **changeNotification** resource.

### <a name="devices-and-apps--cloud-printing"></a>Devices and apps | Cloud printing
- The [printer](/graph/api/resources/printer?view=graph-rest-beta&preserve-view=true) and [printerShare](/graph/api/resources/printershare?view=graph-rest-beta&preserve-view=true) resources are now in parity and have the same properties as each other.
- Some property and type name clean-up around printer shares:
  - Use the **shared** navigation property of [print](/graph/api/resources/print?view=graph-rest-beta&preserve-view=true) to get the list of printer shares registered in the tenant. 
  - See details in the [May](changelog.md#may-2020) changelog.

### <a name="devices-and-apps--corporate-management"></a>Devices and apps | Corporate management
Intune [May](changelog.md#may-2020) updates in beta.

### <a name="groups"></a>Groups
- [Evaluate](/graph/api/group-evaluatedynamicmembership?view=graph-rest-beta&preserve-view=true) whether a user or device is or would be a member of a dynamic group, using the existing rule for the [group](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) or a specified rule. [Rule-based dynamic membership](/azure/active-directory/users-groups-roles/groups-dynamic-membership) reduces administrative overhead of adding and removing members.
- When creating a Microsoft 365 [group](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true), configure the behaviors of the group by specifying them in the **resourceBehaviorOptions** property. For example, allow members to post, subscribe new members to conversation, disable welcome email, and hide the group in Outlook experiences.
- Specify the resources to provision in the **resourceProvisioningOptions** property that are normally not part of the default [group](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) creation. Currently supported is provisioning a group as a [team](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true) with Microsoft Teams capabilities.

### <a name="identity-and-access"></a>Identity and access
- Apply OData system query options (`$count`, `$filter`, `$search`) when getting collections of entities that are derived from [directoryObject](/graph/api/resources/directoryObject). You can [search for specific tokens](/graph/search-query-parameter#using-search-on-directory-object-collections) in the **displayName** and **description** properties of these entities, and use OData cast to trim **directoryObject** results to certain derived types. See more details in [Build advanced queries in Microsoft Graph with $count, $filter, $search, and $orderby](https://developer.microsoft.com/pt-BR/graph/blogs/build-advanced-queries-with-count-filter-search-and-orderby/).
- As part of the [identity protection API](/graph/api/resources/identityprotection-root?view=graph-rest-beta&preserve-view=true), use the **riskEventType** property to [get the type of risk detected](/graph/api/riskdetection-get?view=graph-rest-beta&preserve-view=true), or [get the type of risk in a user's history](/graph/api/riskyuser-list-history?view=graph-rest-beta&preserve-view=true). Do not use the **riskType** property as it has been deprecated.
- Specify client application types in the **clientAppTypes** property of the [condition set](/graph/api/resources/conditionalaccessconditionset?view=graph-rest-beta&preserve-view=true) for a [conditional access policy](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true).
- Use the delegated permission of `EntitlementManagement.Read.All` to allow an app to read access packages and related entitlement management resources on behalf of the signed-in user.
- Use the delegated or application permissions of `Application.Read.All` and `Application.ReadWrite.All` to [list applications](/graph/api/application-list?view=graph-rest-beta&preserve-view=true) in an organization.
- Control authorization settings in Azure AD using the [authorizationPolicy](/graph/api/resources/authorizationpolicy?view=graph-rest-beta&preserve-view=true) resource type.

### <a name="teamwork"></a>Teamwork
- Teams apps that [support single sign-on (SSO)](/microsoftteams/platform/tabs/how-to/authentication/auth-aad-sso) can specify the `WebApplicationInfo.id` from the Teams app manifest, in the **azureADAppId** property of the [teamsAppDefinition](/graph/api/resources/teamsappdefinition?view=graph-rest-beta&preserve-view=true).
- Use [finer grained permissions](./permissions-reference.md#team-resource-specific-consent-permissions) to access [team](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true) and [channel](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true) resources.


## <a name="april-2020-new-and-generally-available"></a>April 2020: New and generally available

### <a name="calendar"></a>Calendar
- [Share or delegate calendars](outlook-share-or-delegate-calendar.md) programmatically, in closer parity with the Outlook user experience. In addition to tracking the current user's permissions and sharing status for a calendar:
  - For each [calendar](/graph/api/resources/calendar?view=graph-rest-1.0&preserve-view=true), you can now manage the [permissions](/graph/api/resources/calendarpermission?view=graph-rest-1.0&preserve-view=true) of each user with whom the calendar is shared. 
  - For each [mailbox](/graph/api/resources/mailboxsettings?view=graph-rest-1.0&preserve-view=true), you can now specify whether a delegate, mailbox owner, or both receive meeting messages and meeting responses. 
- [Create or update an event as an online meeting](outlook-calendar-online-meetings.md):
  - For each **calendar**, specify the allowed and the default online meeting providers.
  - Create or update an [event](/graph/api/resources/event?view=graph-rest-1.0&preserve-view=true) to be available online, and provide details for attendees to join the meeting online. 
  - In particular, use the new **onlineMeetingProvider** and **onlineMeeting** properties of **event** to set or identify Microsoft Teams as an online meeting provider, a workaround for a [known issue](known-issues.md#onlinemeetingurl-property-support-for-microsoft-teams) with the **onlineMeetingUrl** property.
- Add [file attachments up to 150MB](outlook-large-attachments.md) to an [event](/graph/api/resources/event?view=graph-rest-1.0&preserve-view=true).

### <a name="files"></a>Files
- [Check out](/graph/api/driveitem-checkout?view=graph-rest-1.0&preserve-view=true) or [check in](/graph/api/driveitem-checkin?view=graph-rest-1.0&preserve-view=true) a file to OneDrive to manage updating the file and making updates available to others when the updates are ready.
- Apply optional password and expiration date/time as parameters of the [invite](/graph/api/driveitem-invite?view=graph-rest-1.0&preserve-view=true) and [create sharing link](/graph/api/driveitem-createlink?view=graph-rest-1.0&preserve-view=true) actions to share a [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0&preserve-view=true).
- Get or set password and expiration date/time of a [permission](/graph/api/resources/permission?view=graph-rest-1.0&preserve-view=true), and track the [identitySet](/graph/api/resources/identityset?view=graph-rest-1.0&preserve-view=true) of users granted the permission to share a **driveItem**.
- Get the [permission](/graph/api/resources/permission?view=graph-rest-1.0&preserve-view=true) of a [shared drive item](/graph/api/resources/shareddriveitem?view=graph-rest-1.0&preserve-view=true) by using the **permission** navigation property.
- Limit users with a [sharing link](/graph/api/resources/sharinglink?view=graph-rest-1.0&preserve-view=true) to only view and may not download the contents of a shared **driveItem** on OneDrive for Business or SharePoint.

### <a name="identity-and-access"></a>Identity and access
- To manage roles and assign access to resources in role-based access control (RBAC) providers such as Microsoft Intune, use [unifiedRoleAssignmentMultiple](/graph/api/resources/unifiedroleassignmentmultiple?view=graph-rest-1.0&preserve-view=true). The **unifiedRoleAssignmentMultiple** resource supports defining a single role over an array of scopes, and assigning the role to multiple principals (such as users).
- Access specific types of [policies for an organization](/graph/api/resources/policy-overview?view=graph-rest-1.0&preserve-view=true) using the `/policies` URL segment and specifying the policy type. For example, an organization can enforce a policy to automatically sign a user out from a web session after a period of inactivity; see CRUD operations for instances of [activityBasedTimeoutPolicy](/graph/api/resources/activitybasedtimeoutpolicy?view=graph-rest-1.0&preserve-view=true). This is a [breaking change](https://developer.microsoft.com/identity/blogs/breaking-changes-policy-api-microsoft-graph-1.0/) to make it easier to discover all policies, by grouping all typed policies under the `/policies` segment. Access other typed policies in a similar approach: [claimsMappingPolicy](/graph/api/resources/claimsmappingpolicy?view=graph-rest-1.0&preserve-view=true), [homeRealmDiscoveryPolicy](/graph/api/resources/homerealmdiscoverypolicy?view=graph-rest-1.0&preserve-view=true), [tokenLifetimePolicy](/graph/api/resources/tokenlifetimepolicy?view=graph-rest-1.0&preserve-view=true), and [tokenIssuancePolicy](/graph/api/resources/tokenissuancetimepolicy?view=graph-rest-1.0&preserve-view=true). 

### <a name="mail"></a>Mail
Add [file attachments up to 150MB](outlook-large-attachments.md) to a [message](/graph/api/resources/message?view=graph-rest-1.0&preserve-view=true).

### <a name="sites-and-lists"></a>Sites and lists
- [List sites](/graph/api/sites-list-followed?view=graph-rest-1.0&preserve-view=true) that the signed-in user has followed.
- Identify the geographic region of a [site collection](/graph/api/resources/sitecollection?view=graph-rest-1.0&preserve-view=true) by using the **dataLocationCode** property.
- Identify the tenant of a file, folder, or other item on SharePoint by accessing the **tenantId** property that is part of the **sharepointIds** of a [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0&preserve-view=true).

## <a name="april-2020-new-in-preview-only"></a>April 2020: New in preview only

### <a name="devices-and-apps--cloud-printing"></a>Devices and apps | Cloud printing

Designate allowed users and groups to use specific [printer shares](/graph/api/resources/printershare?view=graph-rest-beta&preserve-view=true) on Universal Print, the Microsoft 365 cloud-based print infrastructure. To experience robust and centralized print management capabilities, and offer a simple yet rich and secure print experience for print users, see the [Universal Print announcement](https://techcommunity.microsoft.com/t5/windows-it-pro-blog/announcing-universal-print-a-cloud-based-print-solution/ba-p/1204775) and join their preview program.

### <a name="devices-and-apps--corporate-management"></a>Devices and apps | Corporate management
Intune [April](changelog.md#april-2020) updates.

### <a name="groups"></a>Groups
Identify the app that created a [group](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) by its app ID.

### <a name="identity-and-access"></a>Identity and access
- [Track changes](/graph/api/administrativeunit-delta?view=graph-rest-beta&preserve-view=true) for [administrative units](/graph/api/resources/administrativeunit?view=graph-rest-beta&preserve-view=true).
- [Track changes](/graph/api/oauth2permissiongrant-delta?view=graph-rest-beta&preserve-view=true) for [oAuth2PermissionGrant](/graph/api/resources/oauth2permissiongrant?view=graph-rest-beta&preserve-view=true).
- [Manage](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta&preserve-view=true) a user's [authentication methods](/graph/api/resources/authenticationmethod?view=graph-rest-beta&preserve-view=true) which include [password](/graph/api/resources/passwordauthenticationmethod?view=graph-rest-beta&preserve-view=true) or [phone](/graph/api/resources/phoneauthenticationmethod?view=graph-rest-beta&preserve-view=true). For example, [reset a user password](/graph/api/passwordauthenticationmethod-resetpassword?view=graph-rest-beta&preserve-view=true) and [get the reset status](/graph/api/authenticationoperation-get?view=graph-rest-beta&preserve-view=true), or [add a phone number](/graph/api/authentication-post-phonemethods?view=graph-rest-beta&preserve-view=true) for a user for SMS or voice call authentication, if the policy is enabled for the user.

### <a name="reports--identity-and-access-reports"></a>Reports | Identity and access reports
[List](/graph/api/relyingpartydetailedsummary-list?view=graph-rest-beta&preserve-view=true) [relying parties](/windows-server/identity/ad-fs/technical-reference/understanding-key-ad-fs-concepts) configured in Active Directory Federation Services.

### <a name="reports--microsoft-365-usage-reports"></a>Reports | Microsoft 365 usage reports
View **Meeting Created** and **Meeting Interacted** data in CSV reports for [email activity counts](/graph/api/reportroot-getemailactivitycounts?view=graph-rest-beta&preserve-view=true), [email activity user counts](/graph/api/reportroot-getemailactivityusercounts?view=graph-rest-beta&preserve-view=true), and [email activity user detail](/graph/api/reportroot-getemailactivityuserdetail?view=graph-rest-beta&preserve-view=true).


## <a name="march-2020-new-and-generally-available"></a>March 2020: New and generally available

### <a name="cloud-communications"></a>Cloud communications
- Get the call routing and incoming context of a [call](/graph/api/resources/call?view=graph-rest-1.0&preserve-view=true).
- [Update the recording status](/graph/api/call-updaterecordingstatus?view=graph-rest-1.0&preserve-view=true) of a call.
- Specify recording information for a [participant](/graph/api/resources/participant?view=graph-rest-1.0&preserve-view=true), including the initiator and status of the recording.
- Uniquely identify participants in a conference or participant-to-participant [call](/graph/api/resources/call?view=graph-rest-1.0&preserve-view=true) using the **callChainId** property.
- Identify as part of [participantInfo](/graph/api/resources/participantinfo?view=graph-rest-1.0&preserve-view=true) the country code and endpoint type (such as Skype for Business, or Skype for Business VOIP) of the participant.
- Third-party video teleconferencing (VTC) device partners can log and provide media quality data for their video teleconferencing devices through a Cloud Video Interop (CVI) bot and using the [logTeleconferenceDeviceQuality](/graph/api/call-logteleconferencedevicequality?view=graph-rest-1.0&preserve-view=true) function. Media quality includes open-type data for [audio](/graph/api/resources/teleconferencedeviceaudioquality?view=graph-rest-1.0&preserve-view=true), [video](/graph/api/resources/teleconferencedevicevideoquality?view=graph-rest-1.0&preserve-view=true), and [screen-sharing](/graph/api/resources/teleconferencedevicescreensharingquality?view=graph-rest-1.0&preserve-view=true).

### <a name="files"></a>Files
- [Remote items](/graph/api/resources/remoteitem?view=graph-rest-1.0&preserve-view=true) that are shared with a user, added to the user's OneDrive, or returned as a search result can contain metadata for an image or video.
- [Follow](/graph/api/driveitem-follow?view=graph-rest-1.0&preserve-view=true) a [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0&preserve-view=true) for convenient access, or for faciliating actions such as move, copy, and save-as. Use [unfollow](/graph/api/driveitem-unfollow?view=graph-rest-1.0&preserve-view=true) to stop following the drive item.
- [Grant](/graph/api/permission-grant?view=graph-rest-1.0&preserve-view=true) permissions to users to access a sharing link, in order to share the corresponding drive item.

### <a name="identity-and-access"></a>Identity and access
- [Track changes](/graph/api/orgcontact-delta?view=graph-rest-1.0&preserve-view=true) for [organizational contacts](/graph/api/resources/orgcontact?view=graph-rest-1.0&preserve-view=true).
- Use the **riskEventTypes_v2** property to get the risk event types associated with a [sign-in](/graph/api/resources/signin?view=graph-rest-1.0&preserve-view=true).
- Use the `User.ManageIdentities.All` delegated permission to allow an app to read, update, or delete identities that are associated with a user's account, that the signed-in user has access to. Use that permission at the application-level without a signed-in user present. This allows the app to [manage](/graph/api/user-update?view=graph-rest-1.0&preserve-view=true) which identities a user can sign-in with.

### <a name="reports"></a>Reports
Use Teams Service Administrator and Teams Communications Administrator as accepted user roles to allow apps to read Microsoft 365 service usage reports on behalf of a user, as [forms of user-delegated authorization](reportroot-authorization.md). 

### <a name="sites"></a>Sites
- Let users [follow](/graph/api/site-follow?view=graph-rest-1.0&preserve-view=true) or [unfollow](/graph/api/site-unfollow?view=graph-rest-1.0&preserve-view=true) SharePoint sites.
- [Subscribe to change notifications](/graph/api/resources/subscription?view=graph-rest-1.0&preserve-view=true) for a SharePoint [list](/graph/api/resources/list?view=graph-rest-1.0&preserve-view=true).

## <a name="march-2020-new-in-preview-only"></a>March 2020: New in preview only

### <a name="calendar"></a>Calendar
- Use the **calendarGroupId** property to get the [calendar group](/graph/api/resources/calendargroup?view=graph-rest-beta&preserve-view=true) in which a [calendar](/graph/api/resources/calendar?view=graph-rest-beta&preserve-view=true) has been created.
- Use the **isDraft** property to identify an [event](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true) as a meeting that the user has updated in Outlook but has not sent to update attendees.

### <a name="cloud-communications"></a>Cloud communications
- Use [createOrGet](/graph/api/onlinemeeting-createorget?view=graph-rest-beta&preserve-view=true) to get an [online meeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) instance by a custom external ID, and create one when none already exists.
- Have the option to use the **externalId** property to identify an online meeting with the custom external ID.
- Use the optional `Accept-Language` HTTP request header to [create](/graph/api/application-post-onlinemeetings?view=graph-rest-beta&preserve-view=true) or [get](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true) an instance of online meeting, so that the successful operation displays the content of the **joinInformation** property in the specified language and locale variant.

### <a name="devices-and-apps"></a>Devices and apps
Intune [March](changelog.md#march-2020) updates.

### <a name="identity-and-access"></a>Identity and access
- Use the `AuditLog.Read.All` permission to list the [sign-in activity](/graph/api/resources/signinactivity?view=graph-rest-beta&preserve-view=true) of a [user](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true).
- Use the `PrivilegedAccess.Read.AzureResources` application-level permission for [Privileged Identity Management (PIM) of Azure resources](/graph/api/resources/privilegedidentitymanagement-resources?view=graph-rest-beta&preserve-view=true), to set up just-in-time access workflow for Azure infrastructure roles at a management group, subscription, resource group, or resource level.
- Use the [identitySecurityDefaultsEnforcementPolicy](/graph/api/resources/identitysecuritydefaultsenforcementpolicy?view=graph-rest-beta&preserve-view=true) entity to [get](/graph/api/identitysecuritydefaultsenforcementpolicy-get?view=graph-rest-beta&preserve-view=true) or [update](/graph/api/identitysecuritydefaultsenforcementpolicy-update?view=graph-rest-beta&preserve-view=true) pre-configured default security settings that protect organizations against common attacks.
- Use an `identity` segment when calling the conditional access APIs. For example, to [get](/graph/api/conditionalaccesspolicy-get?view=graph-rest-beta&preserve-view=true) a [conditional access policy](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true): `GET https://graph.microsoft.com/beta/identity/conditionalAccess/policies/{id}`.
- Use the **authenticationRequirement** property to get the highest level of authentication that is needed through all the sign-in steps in order for [sign-in](/graph/api/resources/signin?view=graph-rest-beta&preserve-view=true) to succeed.
- Use pagination when [listing provisioning events](/graph/api/provisioningobjectsummary-list?view=graph-rest-beta&preserve-view=true) that occurred in your tenant.

### <a name="search"></a>Search
- To add data in a file to search results, index the data simply as an [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true). The **externalFile** type has been deprecated.
- [Update](/graph/api/externalitem-update?view=graph-rest-beta&preserve-view=true) an [item in the index](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true), by specifically updating the plain-text representation of the item (represented by the **content** property), or the properties bag of the item (represented by the **properties** property). Updating any property in the properties bag overwrites the entire properties bag, so make sure to explicitly include all the properties of the item in the update.
- Check for `HTTP 429` and the `Retry-After` response header after calling the [create](/graph/api/externalconnection-put-items?view=graph-rest-beta&preserve-view=true), [update](/graph/api/externalitem-update?view=graph-rest-beta&preserve-view=true), or [delete](/graph/api/externalitem-delete?view=graph-rest-beta&preserve-view=true) operation of **externalItem**. Backing off requests using the `Retry-After` delay is the fastest way to recover from [throttling](throttling.md#best-practices-to-handle-throttling).

### <a name="teamwork"></a>Teamwork
Use the `ChannelMessage.Read.All` application-level permission to read [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta&preserve-view=true) instances in channels without a signed-in user.

### <a name="universal-print"></a>Universal Print
Debut of the [Universal Print API](universal-print-concept-overview.md) which allows users to print on the web or from an app. The API lets IT administrators manage user and group access to printers in the Microsoft 365 cloud, remote printer sharing to maintain availability, monitor printer status, and report on archived print jobs and usage. 

Note that as of March 2020, the Universal Print _service_ is in private preview. See [Announcing Universal Print: a cloud-based print solution](https://aka.ms/announcinguniversalprint) for information regarding participation.


## <a name="february-2020-new-and-generally-available"></a>February 2020: New and generally available

### <a name="calendar"></a>Calendar
Walk through an example of [creating an event in a shared or delegated calendar](outlook-create-event-in-shared-delegated-calendar.md), and the actions and properties available to the delegate, invitees, and calendar owner during this process.

### <a name="identity-and-access"></a>Identity and access
- To improve security when subscribing to [change notifications of user data](webhooks.md), [enforce Transport Layer Security (TLS) 1.2](/configmgr/core/plan-design/security/enable-tls-1-2) or higher on clients and site servers used in the notification process. The new requirement is rolled out in stages starting February 15 2020. By May 15, 2020, all notification endpoints must meet the new TLS requirement. [Find out the stages of the rollout](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) and if necessary, use the new **latestSupportedTlsVersion** property as a temporary workaround to avoid subscription failures, before completing the TLS upgrade.
- Use respective types of [threat assessment request](/graph/api/resources/threatAssessmentRequest?view=graph-rest-1.0&preserve-view=true) to track threats from [mail](/graph/api/resources/mailassessmentrequest?view=graph-rest-1.0&preserve-view=true), an [email message file](/graph/api/resources/emailfileassessmentrequest?view=graph-rest-1.0&preserve-view=true) (.EML file), [email attachment file](/graph/api/resources/fileassessmentrequest?view=graph-rest-1.0&preserve-view=true) (text, Word, or binary file), or [URL](/graph/api/resources/urlassessmentrequest?view=graph-rest-1.0&preserve-view=true).

### <a name="users"></a>Users
[Reprocess](/graph/api/user-reprocesslicenseassignment?view=graph-rest-1.0&preserve-view=true) all group-based license assignments for a [user](/graph/api/resources/user?view=graph-rest-1.0&preserve-view=true).


## <a name="february-2020-new-in-preview-only"></a>February 2020: New in preview only

### <a name="calendar"></a>Calendar
See [tasks supported by preview APIs that manage calendar sharing and delegation](outlook-share-or-delegate-calendar.md).

### <a name="cloud-communications"></a>Cloud communications

- Use the new [call records](/graph/api/resources/callrecord?view=graph-rest-beta&preserve-view=true) resource to get metadata of calls and online meetings on Microsoft Teams and Skype for Business for an organization.
- For a participant in a meeting, use the **initiator** property to get the identity information of the initiator of a [recording](/graph/api/resources/recordinginfo?view=graph-rest-beta&preserve-view=true), if there is one.

### <a name="devices-and-apps"></a>Devices and apps
Intune [February](changelog.md#february-2020) updates.

### <a name="groups"></a>Groups
Use the [assignLicense](/graph/api/group-assignlicense?view=graph-rest-beta&preserve-view=true) method to assign licences for products, such as Microsoft 365 or Enterprise Mobility + Security, to a group. Since Azure AD ensures licences are assigned to members of the group, members joining or leaving a group no longer requires licence management at the individual level.

### <a name="identity-and-access"></a>Identity and access
- Set requestor, approval, and review settings when creating an [access package assignment policy](/graph/api/resources/accesspackageassignmentpolicy?view=graph-rest-beta&preserve-view=true).
- Access specific types of [policies for an organization](/graph/api/resources/policy-overview?view=graph-rest-beta&preserve-view=true) using the `/policies` URL segment and specifying the policy type. For example, an organization can enforce a policy to automatically sign a user out from a web session after a period of inactivity; see CRUD operations for instances of [activityBasedTimeoutPolicy](/graph/api/resources/activitybasedtimeoutpolicy?view=graph-rest-beta&preserve-view=true). This is a [breaking change](https://developer.microsoft.com/identity/blogs/breaking-changes-policy-api-microsoft-graph-beta/) to make it easier to discover all policies, by grouping all typed policies under the `/policies` segment. Access other typed policies in a similar approach: [claimsMappingPolicy](/graph/api/resources/claimsmappingpolicy?view=graph-rest-beta&preserve-view=true), [homeRealmDiscoveryPolicy](/graph/api/resources/homerealmdiscoverypolicy?view=graph-rest-beta&preserve-view=true), [tokenLifetimePolicy](/graph/api/resources/tokenlifetimepolicy?view=graph-rest-beta&preserve-view=true), and [tokenIssuancePolicy](/graph/api/resources/tokenissuancetimepolicy?view=graph-rest-beta&preserve-view=true). 
- Use application-level and delegated `Policy.ReadWrite.ApplicationConfiguration` permission for read and write operations on application configuration [policies](/graph/api/resources/policy-overview?view=graph-rest-beta&preserve-view=true) mentioned in the preceding item.

### <a name="teamwork"></a>Teamwork
- Use [change notifications](/graph/api/resources/webhooks?view=graph-rest-beta&preserve-view=true) on all channel messages or all chat messages in an organization.
- [Decline](/graph/api/swapshiftschangerequest-decline?view=graph-rest-beta&preserve-view=true) a [request to swap shifts](/graph/api/resources/swapshiftschangerequest?view=graph-rest-beta&preserve-view=true) with another user in a [team](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true).

## <a name="january-2020-new-and-generally-available"></a>January 2020: New and generally available

### <a name="security"></a>Security
As part of customer alert management, use the [update alert](/graph/api/alert-update?view=graph-rest-1.0&preserve-view=true) method and update the **comments** field as either `Closed in IPC` or `Closed in MCAS`.

### <a name="teamwork"></a>Teamwork
Use the **primaryChannel** navigation property of a [team](/graph/api/resources/team?view=graph-rest-1.0&preserve-view=true) to access its default channel, **General**.

### <a name="users"></a>Users
Use the **identities** property to access one or more identities that a [user](/graph/api/resources/user?view=graph-rest-1.0&preserve-view=true) can use to sign in to an Azure AD user account. The identities can be provided by Microsoft, organizations, or social identity providers such as Facebook, Google, or Microsoft. This property allows the user to sign in to the user account with any of these identities.

## <a name="january-2020-new-in-preview"></a>January 2020: New in preview

### <a name="devices-and-apps"></a>Devices and apps
Intune [January](changelog.md#january-2020) updates.


## <a name="december-2019-new-and-generally-available"></a>December 2019: New and generally available

### <a name="cloud-communications"></a>Cloud communications
The cloud communications API has GA'd and APIs for [call](/graph/api/resources/call?view=graph-rest-1.0&preserve-view=true) and [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-1.0&preserve-view=true) are [available in v1.0](/graph/api/resources/communications-api-overview?view=graph-rest-1.0&preserve-view=true).

### <a name="education"></a>Education
Use the **classSettings** property to manage class-specific settings, such as enabling the sending of weekly assignment digests. This property is available on the [team](/graph/api/resources/team?view=graph-rest-1.0&preserve-view=true) resource when the team represents an [education class](/graph/api/resources/educationclass?view=graph-rest-1.0&preserve-view=true).

### <a name="identity-and-access"></a>Identity and access 
[Attempting to get container objects with limited permissions returns partial data](permissions-reference.md#limited-information-returned-for-inaccessible-member-objects). An example is a [group](/graph/api/resources/group?view=graph-rest-1.0&preserve-view=true) instance that's associated with a [user](/graph/api/resources/user?view=graph-rest-1.0&preserve-view=true), another **group**, and a [device](/graph/api/resources/device?view=graph-rest-1.0&preserve-view=true). An app having only the permissions User.Read.All and Group.Read.All and attempting to access this **group** instance would get the **user** and **group** objects, but limited data for the **device** object (only data type and object ID and not property values).

### <a name="people-and-workplace-intelligence"></a>People and workplace intelligence
The insights API has GA'd. Use the API in production apps to identify the most relevant documents that are:

- [Trending around](/graph/api/insights-list-trending?view=graph-rest-1.0&preserve-view=true) a user
- [Used by](/graph/api/insights-list-used?view=graph-rest-1.0&preserve-view=true) a user
- [Shared with or shared by](/graph/api/insights-list-shared?view=graph-rest-1.0&preserve-view=true) a user

### <a name="reports"></a>Reports
To get Microsoft 365 usage reports using permissions delegated by a user, administrators must have assigned the user an Azure AD limited administrator role. This can be one of the following roles: company administrator, Exchange administrator, SharePoint administrator, Lync administrator, global reader, or reports reader. See [Authorization for APIs to read Microsoft 365 usage reports](reportroot-authorization.md) for details.

### <a name="toolkit"></a>Toolkit
Microsoft Graph Toolkit v1.1 has released. For a list of enhancements and bug fixes, see the [December 2019 section](changelog.md#december-2019) of the changelog.

## <a name="december-2019-new-in-preview"></a>December 2019: New in preview

### <a name="cloud-communications"></a>Cloud communications
- Use the new [presence](/graph/api/resources/presence?view=graph-rest-beta&preserve-view=true) resource to get information about the availability and current activity of one or more users.
- [Delete](/graph/api/onlinemeeting-delete?view=graph-rest-beta&preserve-view=true) an instance of an [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true).
- See the [December 2019 section](changelog.md#december-2019) of the changelog for the renaming and removal of a few members of the [call](/graph/api/resources/call?view=graph-rest-beta&preserve-view=true) and [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) resources, to be in parity with the v1 version of these resources.

### <a name="devices-and-apps"></a>Devices and apps
Intune [December](changelog.md#december-2019) updates

### <a name="identity-and-access"></a>Identity and access 
- Behavior fix to the **appRoleAssignments** and **appRoleAssignedTo** relationships on [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true).
- Use [accessPackageResourceRequest](/graph/api/resources/accesspackageresourcerequest?view=graph-rest-beta&preserve-view=true) in [Azure AD entitlement management](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta&preserve-view=true) to request adding a resource to a [catalog](/graph/api/resources/accesspackagecatalog?view=graph-rest-beta&preserve-view=true), so that the roles of that resource can be used in an [access package](/graph/api/resources/accesspackage?view=graph-rest-beta&preserve-view=true).
- Use the [threat assessment API](/graph/api/resources/threatassessment-api-overview?view=graph-rest-beta&preserve-view=true) to empower administrators to report suspicious emails, phishing URLs, email attachments, or other files. The thread scanning verdict can then inform them to adjust organizational policy appropriately.

### <a name="teamwork"></a>Teamwork
- [Set up change notifications that include resource data](webhooks-with-resource-data.md) for [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta&preserve-view=true) resources in Microsoft Teams channels and chats.
- [Subscribe to notifications](/graph/api/resources/subscription?view=graph-rest-beta&preserve-view=true) for new or modified [channel messages or chat messages](/graph/api/resources/chatmessage?view=graph-rest-beta&preserve-view=true).
- Use the [shiftPreferences](/graph/api/resources/shiftpreferences?view=graph-rest-beta&preserve-view=true) resource to enable specifying a user's availability to be assigned shifts in a [schedule](/graph/api/resources/schedule?view=graph-rest-beta&preserve-view=true). Get or set this as part of the user's [settings](/graph/api/resources/usersettings?view=graph-rest-beta&preserve-view=true).


## <a name="november-2019-new-and-generally-available"></a>November 2019: New and generally available

### <a name="groups"></a>Groups
- Use delegated or application permissions, GroupMember.Read.All and GroupMember.ReadWrite.All, to list groups, read basic group properties, read (and update if read/write permission) the membership of the groups the app has access to.
- Use the application permission, Group.Create, to create groups without a signed-in user.
- For a specified [group](/graph/api/resources/group?view=graph-rest-1.0&preserve-view=true), [check for membership](/graph/api/group-checkmemberobjects?view=graph-rest-1.0&preserve-view=true) in other groups or directory roles.

### <a name="identity-and-access"></a>Identity and access
- Register [applications](/graph/api/resources/application?view=graph-rest-1.0&preserve-view=true) that authenticate with Azure Active Directory (Azure AD). Use delegated [permissions](./permissions-reference.md#application-resource-permissions), Application.Read.All and Application.ReadWrite.All, or application permission, Application.Read.All, as appropriate.
- For a specified [device](/graph/api/resources/device?view=graph-rest-1.0&preserve-view=true), [check for membership](/graph/api/device-checkmemberobjects?view=graph-rest-1.0&preserve-view=true) in other groups or directory roles.

### <a name="mail"></a>Mail
- Use the **conversationIndex** property to get the position of a message in an Outlook email conversation.
- Use the delegated permission, Mail.ReadBasic, and application permission, Mail.ReadBasic.All, to get [message](/graph/api/resources/message?view=graph-rest-1.0&preserve-view=true) or [mail folder](/graph/api/resources/mailfolder?view=graph-rest-1.0&preserve-view=true) resources, track their changes, and manage [subscriptions](/graph/api/resources/subscription?view=graph-rest-1.0&preserve-view=true) for change notifications on messages.

### <a name="users"></a>Users
- [Check for group memberships](/graph/api/user-checkmemberobjects?view=graph-rest-1.0&preserve-view=true) for a specified [user](/graph/api/resources/user?view=graph-rest-1.0&preserve-view=true).
- Use the **creationType** property to find how a user account was created, for example, whether the account was created as a regular school or work account or as an external account, etc.

## <a name="november-2019-new-in-preview"></a>November 2019: New in preview

### <a name="calendar"></a>Calendar
- [Use Outlook to organize or attend meetings online](outlook-calendar-online-meetings.md).
- [Set properties](/graph/api/place-update?view=graph-rest-beta&preserve-view=true) for the rich location types of [room](/graph/api/resources/room?view=graph-rest-beta&preserve-view=true) and [room list](/graph/api/resources/roomlist?view=graph-rest-beta&preserve-view=true).

### <a name="cloud-communication"></a>Cloud communication
The [call](/graph/api/resources/call?view=graph-rest-beta&preserve-view=true) resource type supports the following additional features:

- The [context of an incoming call](/graph/api/resources/incomingcontext?view=graph-rest-beta&preserve-view=true)
- The type of endpoint for a participant, such as voice mail or Skype for Business
- The ability to [update](/graph/api/call-updaterecordingstatus?view=graph-rest-beta&preserve-view=true) the [recording information](/graph/api/resources/recordinginfo?view=graph-rest-beta&preserve-view=true) for a [participant](/graph/api/resources/participant?view=graph-rest-beta&preserve-view=true)

### <a name="devices-and-apps"></a>Devices and apps
Intune [November](changelog.md#november-2019) updates

### <a name="education"></a>Education
Administrators can enable class-wide settings through the **classSettings** property of the [team](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true) associated with the [class](/graph/api/resources/educationclass?view=graph-rest-beta&preserve-view=true). Currently, there is a setting to notify guardians about weekly assignments.

### <a name="identity-and-access"></a>Identity and access
- Use the application permission, Policy.Read.All, to read all your organization's conditional access policies and named locations, without a signed-in user present.
- Allow a [conditional access policy](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true) to be in a report-only state, `enabledForReportingButNotEnforced`.
- Use the delegated permission, ThreatAssessment.ReadWrite.All, or application permission, ThreatAssessment.Read.All, to read (or create, if read/write permission) requests to assess threats in an organization.

### <a name="mail"></a>Mail
Use the delegated permission, Mail.ReadBasic, and application permission, Mail.ReadBasic.All, to manage [subscriptions](/graph/api/resources/subscription?view=graph-rest-beta&preserve-view=true) for change notifications on the [message](/graph/api/resources/message?view=graph-rest-beta&preserve-view=true) resource.

### <a name="notifications"></a>Notifications
Use the new light-weight notifications [web SDK](https://aka.ms/GNSDK) in place of the [Project Rome SDK](https://github.com/Microsoft/project-rome), to take advantage of an improved authentication model and support for web apps using web push. 

### <a name="people-and-workplace-intelligence"></a>People and workplace intelligence
Debut of the [profile](/graph/api/resources/profile?view=graph-rest-beta&preserve-view=true) resource which is a rich representation of the next generation of people entities in Microsoft services. This resource relates to common and practical people attributes, including information for any meaningful dates such as [anniversaries](/graph/api/resources/personanniversary?view=graph-rest-beta&preserve-view=true), [education](/graph/api/resources/educationalactivity?view=graph-rest-beta&preserve-view=true), [employment positions](/graph/api/resources/workposition?view=graph-rest-beta&preserve-view=true), [interests](/graph/api/resources/personinterest?view=graph-rest-beta&preserve-view=true), [language](/graph/api/resources/languageproficiency?view=graph-rest-beta&preserve-view=true) and [skill](/graph/api/resources/skillproficiency?view=graph-rest-beta&preserve-view=true) proficiencies, [project participation](/graph/api/resources/projectparticipation?view=graph-rest-beta&preserve-view=true), [web site association](/graph/api/resources/personwebsite?view=graph-rest-beta&preserve-view=true), and other [account](/graph/api/resources/useraccountinformation?view=graph-rest-beta&preserve-view=true) and contact information.

### <a name="search"></a>Search
Debut of the [Microsoft Search API](search-concept-overview.md) which allows app users to get more up-to-date, personalized, and relevant search results powered by Microsoft Graph. Use the [query](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) capability that by default, searches Outlook messages and events, and OneDrive and SharePoint files in the Microsoft cloud. Use [connectors](/microsoftsearch/connectors-overview), available in the [Microsoft Graph connectors gallery](/microsoftsearch/connectors-gallery), to include search data outside of the Microsoft cloud. Alternatively, [build your own connectors](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true#common-use-cases), index external custom items and files, and query specific external data sources.

### <a name="teamwork"></a>Teamwork
Get the [file](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true) resources associated with a [team](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true) and [channel](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true) by using the following HTTP request syntax:

```http
GET /teams/{teamId}/channels/{channelId}/filesFolder
```

### <a name="users"></a>Users
Use the **creationType** property to find how a user account was created, for example, whether the account was created as a regular school or work account or as an external account, etc.


## <a name="october-2019-new-and-generally-available"></a>October 2019: New and generally available

### <a name="identity-and-access"></a>Identity and access
- Use [organization contacts](/graph/api/resources/orgcontact?view=graph-rest-1.0&preserve-view=true) in production apps. Organization contacts are managed by organization administrators, synchronized either from an on-premises Active Directory or from Exchange Online.
- Configure [certificate-based authentication](/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started) in an [organization](/graph/api/resources/organization?view=graph-rest-1.0&preserve-view=true).
- Add and remove [password credentials](/graph/api/resources/passwordcredential?view=graph-rest-1.0&preserve-view=true) for [applications](/graph/api/resources/application?view=graph-rest-1.0&preserve-view=true).

### <a name="mail"></a>Mail
Use the new **message** parameter to update any writeable [message](/graph/api/resources/message?view=graph-rest-1.0&preserve-view=true) properties when [replying](/graph/api/message-reply?view=graph-rest-1.0&preserve-view=true) to a message, for example, [adding a recipient to the reply](/graph/api/message-reply#example?view=graph-rest-1.0&preserve-view=true).

### <a name="microsoft-graph-data-connect"></a>Microsoft Graph data connect
Developers and data scientists can now use [tools to translate Office 365 data into Common Data Model format](https://github.com/OfficeDev/MS-Graph-Data-Connect/blob/master/Common-Data-Model/README.md), making it schematically consistent with other Open Data Initiative (ODI)-ready datasets. 


### <a name="microsoft-graph-sdks"></a>Microsoft Graph SDKs
- Use chaos handlers in the JavaScript SDK to verify if an app is resilient to server failures that are tricky to initiate.
- Read about [making API calls using the SDKs](./sdks/create-requests.md).

### <a name="users"></a>Users
- [Get](/graph/api/user-get-mailboxsettings?view=graph-rest-1.0&preserve-view=true) or [set](/graph/api/user-update-mailboxsettings?view=graph-rest-1.0&preserve-view=true) a user's preferred date and time format [settings for the user's mailbox](/graph/api/resources/mailboxsettings?view=graph-rest-1.0&preserve-view=true). 
- Track the date/time of the last password change on a [user](/graph/api/resources/user?view=graph-rest-1.0&preserve-view=true).

## <a name="october-2019-new-in-preview"></a>October 2019: New in preview

### <a name="calendar"></a>Calendar
- Meeting organizers can [allow invitees to propose alternate meeting times](outlook-calendar-meeting-proposals.md). When receiving a meeting response that includes a proposed alternate time, the organizer can decide to accept the proposal and [update](/graph/api/event-update?view=graph-rest-beta&preserve-view=true) the meeting time.
- Programmatic calendar sharing is in closer parity with the Outlook user experience. In addition to tracking the current user's permissions and sharing status for a calendar:
  - For each [calendar](/graph/api/resources/calendar?view=graph-rest-beta&preserve-view=true), you can now manage the [permissions](/graph/api/resources/calendarpermission?view=graph-rest-beta&preserve-view=true) of each user with whom the calendar is shared. 
  - For each [mailbox](/graph/api/resources/mailboxsettings?view=graph-rest-beta&preserve-view=true), you can now specify whether a delegate, mailbox owner, or both receive meeting messages and meeting responses. 
- Additional online meeting support:
  - For each **calendar**, specify the allowed and the default online meeting providers.
  - Create or update an [event](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true) to be available online, and provide details for attendees to join the meeting online. 
  - In particular, use the new **onlineMeetingProvider** and **onlineMeeting** properties of **event** to set or identify Microsoft Teams as an online meeting provider, a workaround for a [known issue](known-issues.md#onlinemeetingurl-property-support-for-microsoft-teams) with the **onlineMeetingUrl** property.

### <a name="devices-and-apps"></a>Devices and apps
Intune [October](changelog.md#october-2019) updates

### <a name="graph-explorer"></a>Graph Explorer
Try the [next version of Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/preview) and see handy contextual information such as permissions, access tokens, and SDK code snippets in the new **Permissions**, **Auth**, and **Snippets** tabs. Use the **Preview** slider to switch between the [production](https://developer.microsoft.com/graph/graph-explorer) and new preview version of Graph Explorer.

### <a name="groups"></a>Groups
- Use the **hideFromAddressLists** and **hideFromOutlookClients** properties to control the visibility of a [group](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) in certain parts of the Outlook user interface or in an Outlook client.
- [Assign](/graph/api/group-assignlicense?view=graph-rest-beta&preserve-view=true) or remove licenses on users in a [group](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access"></a>Identity and access
- Use [conditional access policies](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true) to customize access rules for an organization. These rules consider signals about a user or a device identity, such as user or group membership, IP location, and behaviors such as attempts to access specific applications, and risky sign-in behaviors.
- Use [entitlement management](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta&preserve-view=true) to manage access to groups, applications, and SharePoint Online sites for users in and outside of an organization.
- Add and remove [password credentials](/graph/api/resources/passwordcredential?view=graph-rest-beta&preserve-view=true) for [applications](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true) and [service principals](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true).
- Manage Azure AD B2C [trust framework policy keys](/graph/api/resources/trustframeworkkeyset?view=graph-rest-beta&preserve-view=true).
- Define Azure AD B2C [user flow](/graph/api/resources/identityuserflow?view=graph-rest-beta&preserve-view=true) policies for sign in, sign up, combined sign up and sign in, password reset, and profile update.
- Configure [information protection labels](/graph/api/resources/informationprotectionlabel?view=graph-rest-beta&preserve-view=true) to classify sensitivity for a user or tenant.
- Existing apps using APIs for [identity risk events](/graph/api/resources/identityriskevent?view=graph-rest-beta&preserve-view=true) should transition to those for [risk detection](/graph/api/resources/riskdetection?view=graph-rest-beta&preserve-view=true) in Azure AD Identity Protection. See the related [blog post](https://developer.microsoft.com/graph/blogs/deprecatation-of-the-identityriskevents-api/) for more details and deprecation timeline.


### <a name="mail"></a>Mail
[Attach large files up to 150MB](outlook-large-attachments.md) to a [message](/graph/api/resources/message?view=graph-rest-beta&preserve-view=true) instance, by creating an [upload session](/graph/api/resources/uploadsession?view=graph-rest-beta&preserve-view=true), and iteratively uploading ranges of the file until all the bytes of the file have been uploaded. 

### <a name="microsoft-graph-security-api"></a>Microsoft Graph Security API
- Preview integration with RSA NetWitness, ServiceNow, and Splunk, to correlate and synchronize [alerts](/graph/api/resources/security-api-overview?view=graph-rest-beta&preserve-view=true#alerts), and improve threat protection and response.
- New triggers added to the [Microsoft Graph security connector](/connectors/microsoftgraphsecurity/) and [playbooks](/azure/security-center/security-center-playbooks) for Logic Apps and Flow. See [playbook examples](https://github.com/microsoftgraph/security-api-solutions/tree/master/Playbooks).
- Support for sending [threat indicators](/graph/api/resources/security-api-overview?view=graph-rest-beta&preserve-view=true#threat-indicators-preview) to Microsoft Defender ATP to block or alert on threats using their own intelligence sources. Integrations with partners like ThreatConnect enable customers to send indicators directly from threat intelligence and automation solutions. 

### <a name="notifications"></a>Notifications
- [Create and send notifications](/graph/api/user-post-notifications?view=graph-rest-beta&preserve-view=true) to all app clients on all device endpoints that a user is signed in to, without having to manage user-delegated permissions.
- Use [target policy endpoints](/graph/api/resources/targetpolicyendpoints?view=graph-rest-beta&preserve-view=true) on user [notifications](/graph/api/resources/notification?view=graph-rest-beta&preserve-view=true) to specifically target notifications for the Windows, iOS, Android, or WebPush platform.
- Specify a [fall back policy](/graph/api/resources/fallbackpolicy?view=graph-rest-beta&preserve-view=true) on notifications for iOS endpoints, to send high-priority raw notifications that might not be delivered to devices otherwise due to platform specific restrictions, such as battery saver mode.

 
### <a name="powershell-sdk"></a>PowerShell SDK 
Developers and IT professionals can note the coming of the [Microsoft Graph Powershell SDK](https://github.com/microsoftgraph/msgraph-sdk-powershell), which will generate modules that contain cmdlets to make Microsoft Graph REST API requests.

## <a name="september-2019-new-and-generally-available"></a>September 2019: New and generally available

### <a name="calendar-mail-and-group"></a>Calendar, mail, and group
[Get the raw content of a file, or the MIME content of an item](/graph/api/attachment-get?view=graph-rest-1.0&preserve-view=true#get-the-raw-contents-of-a-file-or-item-attachment) that has been added as an [attachment](/graph/api/resources/attachment?view=graph-rest-1.0&preserve-view=true) to an [event](/graph/api/resources/event?view=graph-rest-1.0&preserve-view=true), [message](/graph/api/resources/message?view=graph-rest-1.0&preserve-view=true), or group [post](/graph/api/resources/post?view=graph-rest-1.0&preserve-view=true).

### <a name="calendar-mail-outlook-task-personal-contact"></a>Calendar, mail, Outlook task, personal contact
Use the [translateExchangeId](/graph/api/user-translateexchangeids?view=graph-rest-1.0&preserve-view=true) function to convert an Outlook item ID between supported [formats](/graph/api/user-translateexchangeids?view=graph-rest-1.0&preserve-view=true#exchangeidformat-values), including the Microsoft Graph default ID format and immutable ID format. 

The following resources support ID format conversion:

- [attachment](/graph/api/resources/attachment?view=graph-rest-1.0&preserve-view=true)
- [contact](/graph/api/resources/contact?view=graph-rest-1.0&preserve-view=true)
- [event](/graph/api/resources/event?view=graph-rest-1.0&preserve-view=true)
- [eventMessage](/graph/api/resources/eventmessage?view=graph-rest-1.0&preserve-view=true)
- [message](/graph/api/resources/message?view=graph-rest-1.0&preserve-view=true)
- [outlookTask](/graph/api/resources/outlooktask?view=graph-rest-1.0&preserve-view=true)

### <a name="mail"></a>Mail
[Get the MIME content of a message](outlook-get-mime-message.md).

### <a name="microsoft-graph-toolkit"></a>Microsoft Graph Toolkit
Use the [Microsoft Graph Toolkit](toolkit/overview.md) to develop production apps that offer a consistent Microsoft 365 look-and-feel, and save time in authenticating and accessing data from Microsoft Graph.

## <a name="september-2019-new-in-preview"></a>September 2019: New in preview

> [!IMPORTANT]
> Features, including APIs and tools, in _preview_ status may change without notice, and some may never be promoted to GA status. Do not use them in production apps.

### <a name="devices-and-apps"></a>Devices and apps
Intune [September](changelog.md#september-2019) updates

### <a name="files"></a>Files
- Enhanced synchronization support:

  - Use the new **pendingOperations** property to identify operations that may affect the binary content of a [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true).
  - [Restore](/graph/api/driveitem-restore?view=graph-rest-beta&preserve-view=true) a deleted **driveItem**. 
- Use Secure Hash Algorithm (SHA-256) to enhance [file](/graph/api/resources/file?view=graph-rest-beta&preserve-view=true) data security and integrity.
- Get or set the orientation of a [photo](/graph/api/resources/photo?view=graph-rest-beta&preserve-view=true). Setting is supported on OneDrive Personal.

### <a name="identity-and-access"></a>Identity and access
- Use the new **identities** property and get the identities that a [user](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true) can use to sign in to an account. Identities can be provided by organizations, or social identity providers such as Facebook, Google, and Microsoft.
- Incremental enhancements for [synchronizing identities](/graph/api/resources/synchronization-overview?view=graph-rest-beta&preserve-view=true) in a cloud application for a tenant:

  - Store settings for a [synchronization job](/graph/api/resources/synchronization-synchronizationjob?view=graph-rest-beta&preserve-view=true)
  - Specify a reason to impose [quarantine](/graph/api/resources/synchronization-quarantine?view=graph-rest-beta&preserve-view=true) on a synchronization job

### <a name="teamwork"></a>Teamwork
Use the **General** channel of a [team](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true), or customize [member settings](/graph/api/resources/teammembersettings?view=graph-rest-beta&preserve-view=true) to let team members create private channels in the **team**.

### <a name="users"></a>Users
- Get or update the identities with which a [user](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true) can sign in to an account. These identities can be provided by business organizations, or by social identity providers such as Facebook, Google, and Microsoft.
- Get or update a user's preferred date and time format [settings for the mailbox](/graph/api/resources/mailboxsettings?view=graph-rest-beta&preserve-view=true).


## <a name="august-2019-new-and-generally-available"></a>August 2019: New and generally available 

### <a name="reports"></a>Reports
- Get additional [mailbox usage data](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-1.0&preserve-view=true) about deleted item count and size.
- Track Microsoft 365 group IDs when [getting group activity details](/graph/api/reportroot-getoffice365groupsactivitydetail?view=graph-rest-1.0&preserve-view=true).
- Track the owner principal name when getting [OneDrive usage account detail](/graph/api/reportroot-getonedriveusageaccountdetail?view=graph-rest-1.0&preserve-view=true) and [SharePoint site usaged detail](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-1.0&preserve-view=true).
- Get the number of active and inactive users on Microsoft 365, when [getting a report on user counts per Microsoft 365 service](/graph/api/reportroot-getoffice365servicesusercounts?view=graph-rest-1.0&preserve-view=true).

### <a name="security"></a>Security
- Use the new [Microsoft Graph security API add-on for Splunk](https://aka.ms/graphsecuritysplunkaddon) to stream security alerts and insights from many partner products into Splunk, enabling easier real-time correlation of their security data. See the [announcement](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Introducing-the-new-Microsoft-Graph-Security-API-add-on-for/ba-p/815972) for more information. 
- [See a list of other solutions and connectors](security-integration.md) built by Microsoft or by Microsoft partners that connect with the security API and let you work with data in a unified format.


## <a name="august-2019-new-in-preview"></a>August 2019: New in preview

> [!IMPORTANT]
> Features, including APIs and tools, in _preview_ status may change without notice, and some may never be promoted to GA status. Do not use them in production apps.

### <a name="devices-and-apps"></a>Devices and apps
Intune [August](changelog.md#august-2019) updates

### <a name="education"></a>Education
- Associate a [teacher](/graph/api/resources/educationuser?view=graph-rest-beta&preserve-view=true) or [assignment](/graph/api/resources/educationassignment?view=graph-rest-beta&preserve-view=true) with a [grading rubric](/graph/api/resources/educationrubric?view=graph-rest-beta&preserve-view=true) to account for specific qualities and levels in assignments. An example of a quality is spelling and grammar, and examples of levels are "good" and "poor". You can further associate points and weights to the rubric. For more information, see [education rubric overview](education-rubric-overview.md).
- Evaluate an assignment and present the results in terms of [feedback](/graph/api/resources/educationfeedbackoutcome?view=graph-rest-beta&preserve-view=true), a [numeric grade](/graph/api/resources/educationpointsoutcome?view=graph-rest-beta&preserve-view=true), or [rubric](/graph/api/resources/educationrubricoutcome?view=graph-rest-beta&preserve-view=true).

### <a name="files"></a>Files
Up till this point, you have been able to [follow](/graph/api/driveitem-follow?view=graph-rest-beta&preserve-view=true) a [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true) for convenient access, or for faciliating actions such as move, copy, and save-as. You can now use the [unfollow](/graph/api/driveitem-unfollow?view=graph-rest-beta&preserve-view=true) action to stop following such drive items.

### <a name="identity-and-access"></a>Identity and access
- Providers of role-based access control (RBAC) can [manage roles](/graph/api/resources/rolemanagement?view=graph-rest-beta&preserve-view=true) in Azure Active Directory, by [defining role actions](/graph/api/resources/unifiedroledefinition?view=graph-rest-beta&preserve-view=true) that can be performed on specific resources, and [assigning roles](/graph/api/resources/unifiedroleassignment?view=graph-rest-beta&preserve-view=true) to users based on such role definitions, giving them the corresponding access to those resources.
- Administrators can [list access reviews](/graph/api/accessreview-list?view=graph-rest-beta&preserve-view=true) to efficiently facilitate reviewing group memberships, access to enterprise applications, and role assignments. Regular access reviews make sure only the appropriate people have continued access to resources in specific ways.

### <a name="social-and-workplace-intelligence"></a>Social and workplace intelligence
End users have been able to use the Microsoft 365 [MyAnalytics](social-intel-concept-overview.md#why-integrate-with-document-based-insights) app to get insights on managing time, collaboration at work, and work-life balance. Now, you can use the [analytics API](/graph/api/resources/social-overview?view=graph-rest-beta&preserve-view=true#help-users-gain-insights-into-their-work-patterns) to integrate data on time spent on work activities such as calls, chats, and email, to help improve a user's productivity and wellbeing. 


## <a name="july-2019-new-and-generally-available"></a>July 2019: New and generally available 

### <a name="example-code-snippets"></a>Example code snippets
There are now Objective-C code snippets in all API topics in the v1.0 and beta references. See the Objective-C example for [getting an event](/graph/api/event-get?view=graph-rest-1.0&preserve-view=true&tabs=objective-c#example).

### <a name="group"></a>Group
- Use the [validateProperties](/graph/api/group-validateproperties?view=graph-rest-1.0&preserve-view=true) function to make sure the display name or mail nickname of an existing Microsoft 365 group complies with naming policies.
- Alternatively, before creating the group, you can use the [validateProperties](/graph/api/directoryobject-validateproperties?view=graph-rest-1.0&preserve-view=true) function for a [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0&preserve-view=true) to validate the names first.

### <a name="identity-and-access"></a>Identity and access
- Use [new delegated and application permissions](permissions-reference.md#organization-permissions), _Organization.Read.All_ and _Organization.ReadWrite.All_, to access an [organization](/graph/api/resources/organization?view=graph-rest-1.0&preserve-view=true) and related resources such as [subscribed SKUs](/graph/api/resources/subscribedsku?view=graph-rest-1.0&preserve-view=true).
- Use [new delegated and application permissions](permissions-reference.md#role-management-permissions), _RoleManagement.Read.Directory_ and _RoleManagement.ReadWrite.Directory_, for role-based access control (RBAC) for your company's directory:

  - Use the read/write permission to first [activate](/graph/api/directoryrole-post-directoryroles?view=graph-rest-1.0&preserve-view=true) a directory role. 
  - With the role activated, you can use the read permission to [read directory roles](/graph/api/directoryrole-list?view=graph-rest-1.0&preserve-view=true), [list role members](/graph/api/directoryrole-list-members?view=graph-rest-1.0&preserve-view=true), and [list directory role templates](/graph/api/directoryroletemplate-list?view=graph-rest-1.0&preserve-view=true). 
  - You can also use the read/write permission to [add](/graph/api/directoryrole-post-members?view=graph-rest-1.0&preserve-view=true) and [remove](/graph/api/directoryrole-delete-member?view=graph-rest-1.0&preserve-view=true) role members.


## <a name="july-2019-new-in-preview"></a>July 2019: New in preview

> [!IMPORTANT]
> Features, including APIs and tools, in _preview_ status may change without notice, and some may never be promoted to GA status. Do not use them in production apps.

### <a name="calendar"></a>Calendar 
Use the new [places API](/graph/api/resources/place?view=graph-rest-beta&preserve-view=true) to make use of rich location types such as [room](/graph/api/resources/room?view=graph-rest-beta&preserve-view=true) and [room list](/graph/api/resources/roomlist?view=graph-rest-beta&preserve-view=true), as set up by Exchange Online administrators.

### <a name="devices-and-apps"></a>Devices and apps
Intune [July](changelog.md#july-2019) updates

### <a name="files"></a>Files 
Apply expiration date/time or password when [creating a sharing link](/graph/api/driveitem-createlink?view=graph-rest-beta&preserve-view=true) to a file, folder, or some other [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access"></a>Identity and access
- Use [new application permission](./permissions-reference.md#access-reviews-permissions) _AccessReview.ReadWrite.Membership_ for CRUD operations on [access reviews](/graph/api/resources/accessreviews-root?view=graph-rest-beta&preserve-view=true). 
- Use [new delegated and application permissions](permissions-reference.md#administrative-units-permissions), _AdministrativeUnit.Read.All_ and _AdministrativeUnit.ReadWrite.All_, to respectively read or write (including create, update, delete, or manage membership) [administrative unit](/graph/api/resources/administrativeunit?view=graph-rest-beta&preserve-view=true) resources.
- Use [new delegated and application permissions](permissions-reference.md#organization-permissions), _Organization.Read.All_ and _Organization.ReadWrite.All_, to access an [organization](/graph/api/resources/organization?view=graph-rest-beta&preserve-view=true) and related resources such as a [subscribed SKU](/graph/api/resources/subscribedsku?view=graph-rest-beta&preserve-view=true).
- Use the new [discover](/graph/api/directorydefinition-discover?view=graph-rest-beta&preserve-view=true) function to find the latest directory [synchronization schema](/graph/api/resources/synchronization-synchronizationschema?view=graph-rest-beta&preserve-view=true), so as to sync directory objects, attributes, and their types to an app.
- Use [feature rollout policy](/graph/api/resources/featureRolloutPolicy?view=graph-rest-beta&preserve-view=true) to help tenant administrators to pilot features to specific groups before enabling them for entire organization.

### <a name="mail"></a>Mail
Use more granular application permission, _Mail.ReadBasic.All_, to read a user's mailbox except for any message body, preview body, attachments, and extended properties, and except for searching the mailbox. Now applicable to [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-beta&preserve-view=true) and [change tracking](delta-query-overview.md) for [message](/graph/api/resources/message?view=graph-rest-beta&preserve-view=true) and **mailFolder**.

### <a name="reports"></a>Reports
- Get additional [mailbox usage data](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-beta&preserve-view=true) about deleted item count and size.

### <a name="teamwork"></a>Teamwork
- [Install](/graph/api/user-add-teamsappinstallation?view=graph-rest-beta&preserve-view=true), [uninstall](/graph/api/user-delete-teamsappinstallation?view=graph-rest-beta&preserve-view=true), [upgrade](/graph/api/user-upgrade-teamsappinstallation?view=graph-rest-beta&preserve-view=true), and [list installed Microsoft Teams apps](/graph/api/user-list-teamsappinstallation?view=graph-rest-beta&preserve-view=true) for a user.
- Use app-only access to read channel messages, replies to channel messages, and messages in a chat. [Request and get approval](teams-protected-apis.md) for such access.

## <a name="may---june-2019-new-and-generally-available"></a>May - June, 2019: New and generally available

### <a name="calendar-mail-and-personal-contacts"></a>Calendar, mail, and personal contacts
Exchange administrators can grant application permissions to an app and [limit the app to access only a subset of mailboxes](auth-limit-mailbox-access.md), instead of the default which is access to all mailboxes in the organization. Such restricted access would apply to any application permissions granted to the app for [calendars](permissions-reference.md#calendars-permissions), [contacts](permissions-reference.md#contacts-permissions), and [mail and mailbox settings](permissions-reference.md#mail-permissions). See related [blog announcement](https://developer.microsoft.com/graph/blogs/scoping-microsoft-graph-application-permissions-to-specific-exchange-online-mailboxes/).

### <a name="mail"></a>Mail
Use [mail search folders](/graph/api/resources/mailsearchfolder?view=graph-rest-1.0&preserve-view=true) API to search messages and access Outlook email search results. See related [blog announcement](https://developer.microsoft.com/graph/blogs/mail-search-folder-support-for-microsoft-graph-apis/).

### <a name="postman"></a>Postman
As an alternative to Graph Explorer, try the Microsoft Graph API on the [Microsoft Graph Postman collection](use-postman.md) to learn the API behavior and speed up app development.

### <a name="tutorials"></a>Tutorials
Try the new [tutorial to build a Java console app](/graph/tutorials/java) to get information about a user calendar.

### <a name="user"></a>User
Administrators or users can [revoke](/graph/api/user-revokesigninsessions?view=graph-rest-1.0&preserve-view=true) all issued refresh tokens for a user. This is usually used to prevent apps on a lost or stolen device from accessing an organization's data.


## <a name="may---june-2019-new-in-preview"></a>May - June, 2019: New in preview

> [!IMPORTANT]
> Features, including APIs and tools, in _preview_ status may change without notice, and some may never be promoted to GA status. Do not use them in production apps.

### <a name="devices-and-apps"></a>Devices and apps
- Intune [May](changelog.md#may-2019) updates 
- Intune [June](changelog.md#june-2019) updates

### <a name="education"></a>Education
- Delta query for [educationSchool](/graph/api/resources/educationschool?view=graph-rest-beta&preserve-view=true).
- Delta query and property additions for [educationClass](/graph/api/resources/educationclass?view=graph-rest-beta&preserve-view=true) and [educationUser](/graph/api/resources/educationuser?view=graph-rest-beta&preserve-view=true).

### <a name="group"></a>Group
Get [sensitivity labels](/graph/api/resources/assignedlabel?view=graph-rest-beta&preserve-view=true) to help protect sensitive data of a Microsoft 365 group and meet compliance policies. These labels are [assignedLabel](/graph/api/resources/assignedlabel?view=graph-rest-beta&preserve-view=true) objects, published by administrators in Microsoft 365 Security & Compliance Center, as part of Microsoft Information Protection capabilities. 

### <a name="identity-and-access"></a>Identity and access
- Get an instance of an [application](/graph/api/resources/applicationtemplate?view=graph-rest-beta&preserve-view=true), or add an instance from the Azure AD application gallery into your directory as a template.
- Get a log of all directory [provisioning events](/graph/api/resources/provisioningobjectsummary?view=graph-rest-beta&preserve-view=true) in a tenant.
- Get information about [detected user or sign-in risks](/graph/api/resources/riskdetection?view=graph-rest-beta&preserve-view=true) in an Azure AD environment. This risk detection functionality is part of Azure AD Identity Protection.

### <a name="mail"></a>Mail
Use more granular delegated permission, _Mail.ReadBasic_, to read a user's mailbox except for any message body, preview body, attachments, and extended properties, and except for searching the mailbox. Available to read methods of [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-beta&preserve-view=true), and [change tracking](delta-query-overview.md) for [message](/graph/api/resources/message?view=graph-rest-beta&preserve-view=true) and **mailFolder**.

### <a name="microsoft-graph-toolkit"></a>Microsoft Graph toolkit
The [Microsoft Graph toolkit](./toolkit/overview.md) is a set of framework-agnostic web components and helpers that provides convenience to authenticate and access data in Microsoft Graph. Because the Microsoft Graph toolkit is in preview status, use toolkit providers and components in only non-production apps.

### <a name="reports"></a>Reports
- Get [reports on the authentication methods](/graph/api/resources/authenticationmethods-usage-insights-overview?view=graph-rest-beta&preserve-view=true) adopted by users in an organization, such as self-service password rest and multi-factor authentication (MFA).

### <a name="sites"></a>Sites
Let users [follow](/graph/api/site-follow?view=graph-rest-beta&preserve-view=true) or [unfollow](/graph/api/site-unfollow?view=graph-rest-beta&preserve-view=true) SharePoint sites.

### <a name="teamwork"></a>Teamwork
- Host [images](/graph/api/resources/chatmessagehostedimage?view=graph-rest-beta&preserve-view=true) in Microsoft Teams [chat messages](/graph/api/resources/chatmessage?view=graph-rest-beta&preserve-view=true).
- Support [configuring](/graph/api/resources/teamdiscoverysettings?view=graph-rest-beta&preserve-view=true) how a private team can be discovered.


## <a name="january---april-2019-new-and-generally-available"></a>January - April, 2019: New and generally available

[Microsoft Graph data connect](data-connect-concept-overview.md)

### <a name="calendar"></a>Calendar
[Get free-busy schedule](outlook-get-free-busy-schedule.md)

### <a name="identity-and-access"></a>Identity and access
[Identity providers](/graph/api/resources/identityprovider?view=graph-rest-1.0&preserve-view=true)
[Improved auth guides](./auth/index.yml)
[Migrating apps from Azure AD Graph to Microsoft Graph](migrate-azure-ad-graph-planning-checklist.md)

### <a name="sdks"></a>SDKs
[SDK guides](/sdks/sdks-overview.md) API snippets ([example](/graph/api/user-get?view=graph-rest-1.0&preserve-view=true&tabs=cs#sdk-sample-code))

### <a name="security"></a>Security
[Tenant secure score](/graph/api/resources/securescore?view=graph-rest-1.0&preserve-view=true)

## <a name="january---april-2019-new-in-preview"></a>January - April, 2019: New in preview

### <a name="calendar-group-mail-to-do-tasks"></a>Calendar, group, mail, to-do tasks
[Get raw/MIME content of file or item attachments](/graph/api/attachment-get?view=graph-rest-beta&preserve-view=true#get-the-raw-contents-of-a-file-or-item-attachment) in an event, message, Outlook task, or group post

### <a name="change-notifications"></a>Change notifications
[Reduce missing change notifications](webhooks-lifecycle.md)

### <a name="devices-and-apps"></a>Devices and apps
- Intune [January](changelog.md#january-2019) updates 
- Intune [February](changelog.md#february-2019) updates
- Intune [March](changelog.md#march-2019) updates
- Intune [April](changelog.md#april-2019) updates

### <a name="files"></a>Files
[Sharing invitation](/graph/api/driveitem-invite?view=graph-rest-beta&preserve-view=true) includes expiration and password

### <a name="financials"></a>Financials
[Dynamics 365 Business Central](dynamics-business-central-concept-overview.md)

### <a name="identity-and-access"></a>Identity and access
[Access reviews](/graph/api/resources/accessreviews-root?view=graph-rest-beta&preserve-view=true) support application permissions [Audit and sign-in logs](/graph/api/resources/azure-ad-auditlog-overview?view=graph-rest-beta&preserve-view=true)
[Custom sign-in and sign-up in Azure AD B2C](/graph/api/resources/trustframeworkpolicy?view=graph-rest-beta&preserve-view=true)
[Risky user](/graph/api/resources/riskyuser?view=graph-rest-beta&preserve-view=true) and [history](/graph/api/resources/riskyuserhistoryitem?view=graph-rest-beta&preserve-view=true)

### <a name="mail"></a>Mail
[Get MIME content of messages](outlook-get-mime-message.md)

### <a name="reports"></a>Reports
[Application sign-in reports](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta&preserve-view=true)

### <a name="security"></a>Security
[Security actions](/graph/api/resources/securityaction?view=graph-rest-beta&preserve-view=true)
[Threat indicators](/graph/api/resources/tiindicator?view=graph-rest-beta&preserve-view=true)

### <a name="teamwork"></a>Teamwork
[1:1 chats](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true)
[Shifts management](/graph/api/resources/shift?view=graph-rest-beta&preserve-view=true)

## <a name="see-also"></a>See also
- See [what's currently new](whats-new-overview.md) in Microsoft Graph.
- Check out the [Microsoft Graph developer blog](https://developer.microsoft.com/graph/blogs/) periodically for release announcements and helpful resources.
- Browse details of Microsoft Graph API additions, and API behavior updates in the [changelog](changelog.md).
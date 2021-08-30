---
title: Trabalhar com relatórios de uso do Microsoft 365 no Microsoft Graph
description: Com o Microsoft Graph, você pode acessar recursos de relatórios de uso do Microsoft 365 para obter informações sobre como as pessoas em sua empresa estão usando os serviços Microsoft 365. Por exemplo, você pode identificar quem está usando muito um serviço e atingindo cotas, ou quem pode não precisar de uma licença do Microsoft 365.
ms.localizationpriority: high
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 3636ec84468368c098753c58e7c1f8965c21a39b
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696292"
---
# <a name="working-with-microsoft-365-usage-reports-in-microsoft-graph"></a>Trabalhar com relatórios de uso do Microsoft 365 no Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Com o Microsoft Graph, você pode acessar recursos de relatórios de uso do Microsoft 365 para obter informações sobre como as pessoas em sua empresa estão usando os serviços Microsoft 365. Por exemplo, você pode identificar quem está usando muito um serviço e atingindo cotas, ou quem pode não precisar de uma licença do Microsoft 365.

## <a name="authorization"></a>Autorização

O Microsoft Graph controla o acesso a recursos por meio de permissões. Você deve especificar as permissões necessárias para acessar os recursos dos Relatórios. Normalmente, você deve especificar permissões no portal do Azure Active Directory (Azure AD). Para saber mais, veja [Referência de permissões do Microsoft Graph](/graph/permissions-reference) e[Permissões de relatórios](/graph/permissions-reference#reports-permissions).

## <a name="changes-to-the-reports-apis"></a>Alterações em APIs de relatórios

As APIs originais de relatórios foram atualizadas para que você possa chamar a API para o modo de exibição específico desejado em vez de passar um parâmetro de modo de exibição. É recomendável que você comece a usar as novas APIs nos aplicativos assim que possível. A tabela a seguir lista as novas APIs que foram removidas e as novas APIs que as substituíram.

| API original            | Nova API                                  |
| :---------------------- | :--------------------------------------- |
| EmailActivity           | <ul><li>[getEmailActivityUserDetail](../api/reportroot-getemailactivityuserdetail.md)</li><li>[getEmailActivityCounts](../api/reportroot-getemailactivitycounts.md)</li><li>[getEmailActivityUserCounts](../api/reportroot-getemailactivityusercounts.md)</li></ul> |
| EmailAppUsage           | <ul><li>[getEmailAppUsageUserDetail](../api/reportroot-getemailappusageuserdetail.md)</li><li>[getEmailAppUsageAppsUserCounts](../api/reportroot-getemailappusageappsusercounts.md)</li><li>[getEmailAppUsageUserCounts](../api/reportroot-getemailappusageusercounts.md)</li><li>[getEmailAppUsageVersionsUserCounts](../api/reportroot-getemailappusageversionsusercounts.md)</li></ul> |
| MailboxUsage            | <ul><li>[getMailboxUsageDetail](../api/reportroot-getmailboxusagedetail.md)</li><li>[getMailboxUsageMailboxCounts](../api/reportroot-getmailboxusagemailboxcounts.md)</li><li>[getMailboxUsageQuotaStatusMailboxCounts](../api/reportroot-getmailboxusagequotastatusmailboxcounts.md)</li><li>[getMailboxUsageStorage](../api/reportroot-getmailboxusagestorage.md)</li></ul> |
| Office365Activations    | <ul><li>[getOffice365ActivationsUserDetail](../api/reportroot-getoffice365activationsuserdetail.md)</li><li>[getOffice365ActivationCounts](../api/reportroot-getoffice365activationcounts.md)</li><li>[getOffice365ActivationsUserCounts](../api/reportroot-getoffice365activationsusercounts.md)</li></ul> |
| Office365ActiveUser     | <ul><li>[getOffice365ActiveUserDetail](../api/reportroot-getoffice365activeuserdetail.md)</li><li>[getOffice365ActiveUserCounts](../api/reportroot-getoffice365activeusercounts.md)</li><li>[getOffice365ServicesUserCounts](../api/reportroot-getoffice365servicesusercounts.md)</li></ul> |
| Office365GroupsActivity | <ul><li>[getOffice365GroupsActivityDetail](../api/reportroot-getoffice365groupsactivitydetail.md)</li><li>[getOffice365GroupsActivityCounts](../api/reportroot-getoffice365groupsactivitycounts.md)</li><li>[getOffice365GroupsActivityGroupCounts](../api/reportroot-getoffice365groupsactivitygroupcounts.md)</li><li>[getOffice365GroupsActivityStorage](../api/reportroot-getoffice365groupsactivitystorage.md)</li><li>[getOffice365GroupsActivityFileCounts](../api/reportroot-getoffice365groupsactivityfilecounts.md)</li></ul> |
| OneDriveActivity        | <ul><li>[getOneDriveActivityUserDetail](../api/reportroot-getonedriveactivityuserdetail.md)</li><li>[getOneDriveActivityUserCounts](../api/reportroot-getonedriveactivityusercounts.md)</li><li>[getOneDriveActivityFileCounts](../api/reportroot-getonedriveactivityfilecounts.md)</li></ul> |
| OneDriveUsage           | <ul><li>[getOneDriveUsageAccountDetail](../api/reportroot-getonedriveusageaccountdetail.md)</li><li>[getOneDriveUsageAccountCounts](../api/reportroot-getonedriveusageaccountcounts.md)</li><li>[getOneDriveUsageFileCounts](../api/reportroot-getonedriveusagefilecounts.md)</li><li>[getOneDriveUsageStorage](../api/reportroot-getonedriveusagestorage.md)</li></ul> |
| SharePointActivity      | <ul><li>[getSharePointActivityUserDetail](../api/reportroot-getsharepointactivityuserdetail.md)</li><li>[getSharePointActivityFileCounts](../api/reportroot-getsharepointactivityfilecounts.md)</li><li>[getSharePointActivityUserCounts](../api/reportroot-getsharepointactivityusercounts.md)</li><li>[getSharePointActivityPages](../api/reportroot-getsharepointactivitypages.md)</li></ul> |
| SharePointSiteUsage     | <ul><li>[getSharePointSiteUsageDetail](../api/reportroot-getsharepointsiteusagedetail.md)</li><li>[getSharePointSiteUsageFileCounts](../api/reportroot-getsharepointsiteusagefilecounts.md)</li><li>[getSharePointSiteUsageSiteCounts](../api/reportroot-getsharepointsiteusagesitecounts.md)</li><li>[getSharePointSiteUsageStorage](../api/reportroot-getsharepointsiteusagestorage.md)</li><li>[getSharePointSiteUsagePages](../api/reportroot-getsharepointsiteusagepages.md)</li></ul> |
| SfbActivity             | <ul><li>[getSkypeForBusinessActivityUserDetail](../api/reportroot-getskypeforbusinessactivityuserdetail.md)</li><li>[getSkypeForBusinessActivityCounts](../api/reportroot-getskypeforbusinessactivitycounts.md)</li><li>[getSkypeForBusinessActivityUserCounts](../api/reportroot-getskypeforbusinessactivityusercounts.md)</li></ul> |
| SfbDeviceUsage          | <ul><li>[getSkypeForBusinessDeviceUsageUserDetail](../api/reportroot-getskypeforbusinessdeviceusageuserdetail.md)</li><li>[getSkypeForBusinessDeviceUsageDistributionUserCounts](../api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts.md)</li><li>[getSkypeForBusinessDeviceUsageUserCounts](../api/reportroot-getskypeforbusinessdeviceusageusercounts.md)</li></ul> |
| SfbOrganizerActivity    | <ul><li>[getSkypeForBusinessOrganizerActivityCounts](../api/reportroot-getskypeforbusinessorganizeractivitycounts.md)</li><li>[getSkypeForBusinessOrganizerActivityUserCounts](../api/reportroot-getskypeforbusinessorganizeractivityusercounts.md)</li><li>[getSkypeForBusinessOrganizerActivityMinuteCounts](../api/reportroot-getskypeforbusinessorganizeractivityminutecounts.md)</li></ul> |
| SfbParticipantActivity  | <ul><li>[getSkypeForBusinessParticipantActivityCounts](../api/reportroot-getskypeforbusinessparticipantactivitycounts.md)</li><li>[getSkypeForBusinessParticipantActivityUserCounts](../api/reportroot-getskypeforbusinessparticipantactivityusercounts.md)</li><li>[getSkypeForBusinessParticipantActivityMinuteCounts](../api/reportroot-getskypeforbusinessparticipantactivityminutecounts.md)</li></ul> |
| SfbP2PActivity          | <ul><li>[getSkypeForBusinessPeerToPeerActivityCounts](../api/reportroot-getskypeforbusinesspeertopeeractivitycounts.md)</li><li>[getSkypeForBusinessPeerToPeerActivityUserCounts](../api/reportroot-getskypeforbusinesspeertopeeractivityusercounts.md)</li><li>[getSkypeForBusinessPeerToPeerActivityMinuteCounts](../api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts.md)</li></ul> |
| YammerActivity          | <ul><li>[getYammerActivityUserDetail](../api/reportroot-getyammeractivityuserdetail.md)</li><li>[getYammerActivityCounts](../api/reportroot-getyammeractivitycounts.md)</li><li>[getYammerActivityUserCounts](../api/reportroot-getyammeractivityusercounts.md)</li></ul> |
| YammerDeviceUsage       | <ul><li>[getYammerDeviceUsageUserDetail](../api/reportroot-getyammerdeviceusageuserdetail.md)</li><li>[getYammerDeviceUsageDistributionUserCounts](../api/reportroot-getyammerdeviceusagedistributionusercounts.md)</li><li>[getYammerDeviceUsageUserCounts](../api/reportroot-getyammerdeviceusageusercounts.md)</li></ul> |
| YammerGroupsActivity    | <ul><li>[getYammerGroupsActivityDetail](../api/reportroot-getyammergroupsactivitydetail.md)</li><li>[getYammerGroupsActivityGroupCounts](../api/reportroot-getyammergroupsactivitygroupcounts.md)</li><li>[getYammerGroupsActivityCounts](../api/reportroot-getyammergroupsactivitycounts.md)</li></ul> |

## <a name="whats-new"></a>O que há de novo
Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.

## <a name="next-steps"></a>Próximas etapas

APIs e recursos de relatório podem criar novas maneiras de se relacionar com os usuários e gerenciar as experiências deles com o Microsoft Graph. Para saber mais:

- Examine os métodos e as propriedades dos recursos mais úteis para o seu cenário.
- Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).

Precisa de mais ideias? Veja [como alguns de nossos parceiros usam o Microsoft Graph](https://developer.microsoft.com/graph/partners).



---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 25b31cad074a3ed71db984b40b2145e4bd34137c395ecfe78dc8c386a85ae331
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899210"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Team team = new Team();
team.additionalDataManager().put("template@odata.bind", new JsonPrimitive("https://graph.microsoft.com/v1.0/teamsTemplates('standard')"));
team.additionalDataManager().put("group@odata.bind", new JsonPrimitive("https://graph.microsoft.com/v1.0/groups('dbd8de4f-5d47-48da-87f1-594bed003375')"));
LinkedList<Channel> channelsList = new LinkedList<Channel>();
Channel channels = new Channel();
channels.displayName = "Class Announcements 📢";
channels.isFavoriteByDefault = true;
channelsList.add(channels);
Channel channels1 = new Channel();
channels1.displayName = "Homework 🏋️";
channels1.isFavoriteByDefault = true;
channelsList.add(channels1);
ChannelCollectionResponse channelCollectionResponse = new ChannelCollectionResponse();
channelCollectionResponse.value = channelsList;
ChannelCollectionPage channelCollectionPage = new ChannelCollectionPage(channelCollectionResponse, null);
team.channels = channelCollectionPage;
TeamMemberSettings memberSettings = new TeamMemberSettings();
memberSettings.allowCreateUpdateChannels = false;
memberSettings.allowDeleteChannels = false;
memberSettings.allowAddRemoveApps = false;
memberSettings.allowCreateUpdateRemoveTabs = false;
memberSettings.allowCreateUpdateRemoveConnectors = false;
team.memberSettings = memberSettings;
LinkedList<TeamsAppInstallation> installedAppsList = new LinkedList<TeamsAppInstallation>();
TeamsAppInstallation installedApps = new TeamsAppInstallation();
installedApps.additionalDataManager().put("teamsApp@odata.bind", new JsonPrimitive("https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.vsts')"));
installedAppsList.add(installedApps);
TeamsAppInstallation installedApps1 = new TeamsAppInstallation();
installedApps1.additionalDataManager().put("teamsApp@odata.bind", new JsonPrimitive("https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('1542629c-01b3-4a6d-8f76-1938b779e48d')"));
installedAppsList.add(installedApps1);
TeamsAppInstallationCollectionResponse teamsAppInstallationCollectionResponse = new TeamsAppInstallationCollectionResponse();
teamsAppInstallationCollectionResponse.value = installedAppsList;
TeamsAppInstallationCollectionPage teamsAppInstallationCollectionPage = new TeamsAppInstallationCollectionPage(teamsAppInstallationCollectionResponse, null);
team.installedApps = teamsAppInstallationCollectionPage;

graphClient.teams()
    .buildRequest()
    .post(team);

```
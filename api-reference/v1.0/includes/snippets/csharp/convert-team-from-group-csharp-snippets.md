---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5356ff305f86e7325348f155f4470745f20f2a3c
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524663"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var team = new Team
{
    Channels = (ITeamChannelsCollectionPage)new List<Channel>()
    {
        new Channel
        {
            DisplayName = "Class Announcements 📢",
            IsFavoriteByDefault = true
        },
        new Channel
        {
            DisplayName = "Homework 🏋️",
            IsFavoriteByDefault = true
        }
    },
    MemberSettings = new TeamMemberSettings
    {
        AllowCreateUpdateChannels = false,
        AllowDeleteChannels = false,
        AllowAddRemoveApps = false,
        AllowCreateUpdateRemoveTabs = false,
        AllowCreateUpdateRemoveConnectors = false
    },
    InstalledApps = (ITeamInstalledAppsCollectionPage)new List<TeamsAppInstallation>()
    {
        new TeamsAppInstallation
        {
            AdditionalData = new Dictionary<string, object>()
            {
                {"teamsApp@odata.bind", "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.vsts')"}
            }
        },
        new TeamsAppInstallation
        {
            AdditionalData = new Dictionary<string, object>()
            {
                {"teamsApp@odata.bind", "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('1542629c-01b3-4a6d-8f76-1938b779e48d')"}
            }
        }
    },
    AdditionalData = new Dictionary<string, object>()
    {
        {"template@odata.bind", "https://graph.microsoft.com/v1.0/teamsTemplates('standard')"},
        {"group@odata.bind", "https://graph.microsoft.com/v1.0/groups('groupId')"}
    }
};

await graphClient.Teams
    .Request()
    .AddAsync(team);

```
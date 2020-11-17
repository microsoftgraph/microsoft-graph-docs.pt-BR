---
description: Automatically generated file. DO NOT MODIFY
ms.openlocfilehash: 55e2c34e59a801c25ecfccd8314f3587c6f94b58
ms.sourcegitcommit: 01f73b4dce6f885da18d62fe800b387c286c7a8e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/09/2020
ms.locfileid: "47414032"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var team = new Team
{
    MemberSettings = new TeamMemberSettings
    {
        AllowCreatePrivateChannels = true,
        AllowCreateUpdateChannels = true
    },
    MessagingSettings = new TeamMessagingSettings
    {
        AllowUserEditMessages = true,
        AllowUserDeleteMessages = true
    },
    FunSettings = new TeamFunSettings
    {
        AllowGiphy = true,
        GiphyContentRating = GiphyRatingType.Strict
    }
};

await graphClient.Groups["{id}"].Team
    .Request()
    .PutAsync(team);

```
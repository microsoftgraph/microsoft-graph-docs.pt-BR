---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 029470d7a3a8328340d919de51d1d021a707bfcc
ms.sourcegitcommit: a0a5690ad9c109149e0b8c8baba164648ff5c226
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/08/2021
ms.locfileid: "49785209"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var team = new Team
{
    MemberSettings = new TeamMemberSettings
    {
        AllowCreatePrivateChannels = true,
        AllowCreateUpdateChannels = true,
        ODataType = null
    },
    MessagingSettings = new TeamMessagingSettings
    {
        AllowUserEditMessages = true,
        AllowUserDeleteMessages = true,
        ODataType = null
    },
    FunSettings = new TeamFunSettings
    {
        AllowGiphy = true,
        GiphyContentRating = GiphyRatingType.Strict,
        ODataType = null
    },
    ODataType = null
};

await graphClient.Groups["{id}"].Team
    .Request()
    .PutAsync(team);

```

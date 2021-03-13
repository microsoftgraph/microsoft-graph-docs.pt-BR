---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d9dd1f6b17717955613a9702c22c2fba72560556
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793253"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var channel = new Channel
{
    DisplayName = "Architecture Discussion",
    Description = "This channel is where we debate all future architecture plans",
    MembershipType = ChannelMembershipType.Standard
};

await graphClient.Teams["{team-id}"].Channels
    .Request()
    .AddAsync(channel);

```
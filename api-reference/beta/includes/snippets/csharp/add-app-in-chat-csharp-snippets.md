---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 134b163cd5b113a7b08c3ad8e0a5d2d755cd02eb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775679"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamsAppInstallation = new TeamsAppInstallation
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"teamsApp@odata.bind", "https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"}
    }
};

await graphClient.Chats["{chat-id}"].InstalledApps
    .Request()
    .AddAsync(teamsAppInstallation);

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b82c388ffd1115e26c59f52f16390e8a7b24d63c
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689800"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamsTab = new TeamsTab
{
    DisplayName = "My Contoso Tab - updated again"
};

await graphClient.Chats["19:d65713bc498c4a428c71ef9353e6ce20@thread.v2"].Tabs["794f0e4e-4d10-4bb5-9079-3a465a629eff"]
    .Request()
    .UpdateAsync(teamsTab);

```
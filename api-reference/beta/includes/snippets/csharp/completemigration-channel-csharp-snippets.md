---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cc08959d0de509dac105bb4a7333bca96bb1fc92
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782159"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{team-id}"].Channels["{channel-id}"]
    .CompleteMigration()
    .Request()
    .PostAsync();

```
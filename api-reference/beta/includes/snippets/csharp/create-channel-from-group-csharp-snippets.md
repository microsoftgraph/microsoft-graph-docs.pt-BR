---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cac770ea5ab74c855869e626b57a9828b1205ac5
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708533"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var channel = new Channel
{
    DisplayName = "Architecture Discussion",
    Description = "This channel is where we debate all future architecture plans"
};

await graphClient.Teams["{id}"].Channels
    .Request()
    .AddAsync(channel);

```
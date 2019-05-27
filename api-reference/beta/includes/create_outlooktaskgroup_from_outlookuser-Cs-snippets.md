---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: af60d1a2fe413e0cfec526e39d17116425aa6c8c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34440062"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookTaskGroup = new OutlookTaskGroup
{
    Name = "Leisure tasks"
};

await graphClient.Me.Outlook.TaskGroups
    .Request()
    .AddAsync(outlookTaskGroup);

```
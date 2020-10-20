---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: af60d1a2fe413e0cfec526e39d17116425aa6c8c
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614681"
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
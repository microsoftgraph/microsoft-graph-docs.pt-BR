---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 72e3e725faee0c5c290934643010ce9b57d28c73
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944235"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = new Group
{
    AssignedLabels = new List<AssignedLabel>()
    {
        new AssignedLabel
        {
            LabelId = "45cd0c48-c540-4358-ad79-a3658cdc5b88"
        }
    }
};

await graphClient.Groups["{group-id}"]
    .Request()
    .UpdateAsync(group);

```
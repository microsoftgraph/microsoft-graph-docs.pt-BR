---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3fecfda40625bd4f6ab3fd1653b2dd532d4bbee3
ms.sourcegitcommit: 43f7800894857a29f02fffaf4a50ad6386b5bf59
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44524486"
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

await graphClient.Groups["{id}"]
    .Request()
    .UpdateAsync(group);

```
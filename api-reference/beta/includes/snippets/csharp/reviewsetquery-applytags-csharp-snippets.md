---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d54ae2f7239813285c38259091f21de0935726e7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772812"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tagsToAdd = new List<Microsoft.Graph.Ediscovery.Tag>()
{
    new Microsoft.Graph.Ediscovery.Tag
    {
        Id = "b4798d14-748d-468e-a1ec-96a2b1d49677"
    }
};

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].ReviewSets["{ediscovery.reviewSet-id}"].Queries["{ediscovery.reviewSetQuery-id}"]
    .ApplyTags(tagsToAdd,null)
    .Request()
    .PostAsync();

```
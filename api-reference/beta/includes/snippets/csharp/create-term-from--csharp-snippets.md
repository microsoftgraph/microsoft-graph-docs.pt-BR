---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8fc51834eaae93804572cdae51ec34f4f6e78a5e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793250"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var term = new Microsoft.Graph.TermStore.Term
{
    Labels = new List<Microsoft.Graph.TermStore.LocalizedLabel>()
    {
        new Microsoft.Graph.TermStore.LocalizedLabel
        {
            LanguageTag = "en-US",
            Name = "Car",
            IsDefault = true
        }
    }
};

await graphClient.TermStore.Sets["{termStore.set-id}"].Terms
    .Request()
    .AddAsync(term);

```
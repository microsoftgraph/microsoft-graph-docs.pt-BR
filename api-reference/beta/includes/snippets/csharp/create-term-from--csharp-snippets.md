---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ffcb43099fb6063a91ba2c94c7e51d584867f4a5c0e37b69cc3fc7b23a1e3582
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099492"
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
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5687728abca99fd671a91b7b208c5fa846a03fae
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59094560"
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

await graphClient.Sites["{site-id}"].TermStore.Sets["{termStore.set-id}"].Terms
    .Request()
    .AddAsync(term);

```
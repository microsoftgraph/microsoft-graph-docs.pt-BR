---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ec5f046a9dbe7cc61f49c2bddad962c57106f20d
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48462616"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var term = new Microsoft.Graph.TermStore.Term
{
    Labels = new List<Microsoft.Graph.TermStore.LocalizedLabel>()
    {
        new Microsoft.Graph.TermStore.LocalizedLabel
        {
            Name = "changedLabel",
            LanguageTag = "en-US",
            IsDefault = true
        }
    }
};

await graphClient.TermStore.Sets["{setId}"].Terms["{termId}"]
    .Request()
    .UpdateAsync(term);

```
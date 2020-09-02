---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1d96ba7802ef63277cf509cdddd3a12e07fe74d4
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/02/2020
ms.locfileid: "47330196"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var term = new Term
{
    Labels = new List<LocalizedLabel>()
    {
        new LocalizedLabel
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
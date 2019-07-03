---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d28ed4a9b659ee6675de1490dfd0eeca9cc02ebc
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35476430"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var value = new List<TiIndicator>()
{
    new TiIndicator
    {
        Id = "c6fb948b-89c5-3bba-a2cd-a9d9a1e430e4",
        AdditionalInformation = "mytest"
    },
    new TiIndicator
    {
        Id = "e58c072b-c9bb-a5c4-34ce-eb69af44fb1e",
        AdditionalInformation = "test again"
    }
};

await graphClient.Security.TiIndicators
    .UpdateTiIndicators(value)
    .Request()
    .PostAsync();

```
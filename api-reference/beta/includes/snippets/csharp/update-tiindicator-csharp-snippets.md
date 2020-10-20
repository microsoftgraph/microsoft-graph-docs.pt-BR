---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2d3094d8f23eb96ce9f00dddbc4302cb7142ea3e
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48615764"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tiIndicator = new TiIndicator
{
    AdditionalInformation = "additionalInformation-after-update",
    Confidence = 42,
    Description = "description-after-update"
};

await graphClient.Security.TiIndicators["{id}"]
    .Request()
    .Header("Prefer","return=representation")
    .UpdateAsync(tiIndicator);

```
---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fbc5035978c76008a82ba35158c015cd2612c6a4
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659069"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var siteSource = new SiteSource
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"site@odata.bind", "https://graph.microsoft.com/v1.0/sites/{siteId}"}
    }
};

await graphClient.Compliance.Ediscovery.Cases["4c8f8f70-7785-4bd4-b296-c98376a2c5e1"].Custodians["2192ca408ea2410eba3bec8ae873be6b"].SiteSources
    .Request()
    .AddAsync(siteSource);

```
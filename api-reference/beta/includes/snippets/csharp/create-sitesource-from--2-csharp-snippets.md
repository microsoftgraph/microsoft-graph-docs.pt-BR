---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6f5ab0a7b09adba47487467b7a656c55b702a272
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "60945618"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var siteSource = new Microsoft.Graph.Ediscovery.SiteSource
{
    Site = new Site
    {
        WebUrl = "https://contoso.sharepoint.com/sites/SecretSite"
    }
};

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].LegalHolds["{ediscovery.legalHold-id}"].SiteSources
    .Request()
    .AddAsync(siteSource);

```
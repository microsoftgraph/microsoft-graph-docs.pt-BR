---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b9dfe29aa36d38429cb08a121978e1cd32c608d5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "60934636"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var siteSource = new Microsoft.Graph.Ediscovery.SiteSource
{
    Site = new Site
    {
        WebUrl = "https://contoso.sharepoint.com/sites/HumanResources"
    }
};

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Custodians["{ediscovery.custodian-id}"].SiteSources
    .Request()
    .AddAsync(siteSource);

```
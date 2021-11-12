---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 316c8fe4b9de3c25316724d17627a0f365531284
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "60946234"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedGroupSource = new Microsoft.Graph.Ediscovery.UnifiedGroupSource
{
    Group = new Group
    {
        Mail = "SecretGroup@contoso.com"
    },
    IncludedSources = Microsoft.Graph.Ediscovery.SourceType.Mailbox | Microsoft.Graph.Ediscovery.SourceType.Site
};

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Custodians["{ediscovery.custodian-id}"].UnifiedGroupSources
    .Request()
    .AddAsync(unifiedGroupSource);

```
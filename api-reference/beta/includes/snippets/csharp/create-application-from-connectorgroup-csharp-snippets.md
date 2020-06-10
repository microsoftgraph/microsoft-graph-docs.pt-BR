---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f0c715c20c0138f55302e5011b6343eda1cbf541
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681261"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var application = new Application
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/beta/applications/{id}"}
    }
};

await graphClient.OnPremisesPublishingProfiles["applicationProxy"].ConnectorGroups["{id}"].Applications
    .Request()
    .AddAsync(application);

```